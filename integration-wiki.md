---
layout: default
title: RisqueCV.fr - Intégration logiciels tiers
permalink: /integration-wiki/
---
<style>
    @import url('https://fonts.googleapis.com/css2?family=Inter:ital,opsz,wght@0,14..32,100..900;1,14..32,100..900&family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');

    * { font-family: 'Inter', sans-serif; }

    h1, h2, h3 { font-family: 'Montserrat', sans-serif; }

    .logo-risquecv {
        display: flex;
        align-items: center;
        gap: 10px;
        font-size: 30px;
        line-height: 1.2;
        margin-bottom: 1rem;
    }

    .logo-risquecv img {
        width: 40px;
        height: 40px;
        flex: 0 0 auto;
    }

    .logo-risquecv-text {
        font-weight: 730;
        font-family: 'Montserrat', sans-serif;
    }

    .bleu { color: #1b2b7f; font-family: 'Montserrat', sans-serif; }
    .rouge { color: #a41835; font-family: 'Montserrat', sans-serif; }

    body > div > h1:nth-child(1) { display: none; }

    @import url(https://fonts.googleapis.com/css?family=Fira+Mono);
/*
 * Thème Prism pour RisqueCV.fr
 * Basé sur une version modifiée de :
 * Hopscotch
 * by Jan T. Sott
 * https://github.com/idleberg/Hopscotch
 *
 * This work is licensed under the Creative Commons CC0 1.0 Universal License
 */

code[class*="language-"],
pre[class*="language-"] {
	font-family: "Fira Mono", Menlo, Monaco, "Lucida Console", "Courier New", Courier, monospace;
	font-size: 16px;
	line-height: 1.375;
	direction: ltr;
	text-align: left;
	word-spacing: normal;
	-moz-tab-size: 4;
	-o-tab-size: 4;
	tab-size: 4;
	-webkit-hyphens: none;
	-moz-hyphens: none;
	-ms-hyphens: none;
	hyphens: none;
	white-space: pre;
	white-space: pre-wrap;
	word-break: break-all;
	word-wrap: break-word;
	background: #b819401c;
	color: #b81940;
}

pre > code[class*="language-"] {
	font-size: 1em;
}

/* Code blocks */
pre[class*="language-"] {
	padding: 1em;
	margin: .5em 0;
	overflow: auto;
}

/* Inline code */
:not(pre) > code[class*="language-"] {
	padding: .1em;
	border-radius: .3em;
}

.token.comment,
.token.prolog,
.token.doctype,
.token.cdata {
	color: #72aa5b;
}

.token.punctuation {
	color: #ffd700;
}

.namespace {
	opacity: .7;
}

.token.null,
.token.operator,
.token.boolean,
.token.number {
	color: #ffffff;
}

.token.property {
	color: #94cff0;
}

.token.tag {
	color: #1290bf;
}

.token.string {
	color: #ce9178;
}

.token.selector {
	color: #c85e7c;
}

.token.attr-name {
	color: #fd8b19;
}

.token.entity,
.token.url,
.language-css .token.string,
.style .token.string {
	color: #149b93;
}

.token.attr-value,
.token.keyword,
.token.control,
.token.directive,
.token.unit {
	color: #5498cf;
}

.token.statement,
.token.regex,
.token.atrule {
	color: #149b93;
}

.token.placeholder,
.token.variable {
	color: #1290bf;
}

.token.important {
	color: #dd464c;
	font-weight: bold;
}

.token.entity {
	cursor: help;
}

pre > code.highlight {
	outline: .4em solid red;
	outline-offset: .4em;
}

code.language-javascript {
    color: #4ec1ff;
}

span.token.function {
    color: #dcdca9;
}

language-javascript {}

span.token.number {
    color: #b3cba6;
}

span.token.boolean {
    color: #4ea0e2;
}
</style>

<h1 class="logo-risquecv">
<img src="https://risquecv.fr/wp-content/uploads/2025/04/icone-photoshop-v3-TROU.png" alt="Logo RisqueCV">
  <span class="logo-risquecv-text">
<span class="bleu">Risque</span><span class="rouge">CV</span><span class="bleu">.fr</span> - Intégration logiciels tiers
</span>
</h1>

Cette page décrit le **protocole de communication bidirectionnel** entre RisqueCV et ses partenaires.

RisqueCV.fr est un outil d'aide à la décision pour la prévention cardiovasculaire. Il permet d'**évaluer le risque cardiovasculaire d'un patient** et de **générer un rapport PDF**.

100% des calculs sont effectués côté client (Typescript), **aucun envoi de données ni aucun calcul vers le serveur de RisqueCV.fr.** 

L'absence de serveur de calcul est **un choix délibéré pour garantir la confidentialité des données des patients.** Cette architecture rend impossible la mise à disposition d'une API REST ou SMART on FHIR.

L'intégration de RisqueCV.fr à un logicier métier repose donc sur l'API Standard `window.postMessage`, permettant un **échange sécurisé** des données cliniques. Ce protocole permet l'ouverture de RisqueCV.fr, le transfert de données cliniques du logiciel métier vers la fenêtre de RisqueCV.fr (sans transfert des données sur internet), la génération du PDF des résultats en local (librairie JS) et l'envoi du rapport PDF de RisqueCV.fr vers le logiciel métier sans transfert des données sur internet.

La méthode `window.postMessage` permet au médecin en consultation de préremplir les données cliniques et d'utiliser l'interface de RisqueCV.fr (courbes, graphiques, conseils, etc.) comme un outil d'**aide à la décision**.

---

## 🏗 Architecture du Protocole (Spécifications)

L'intégration repose sur un protocole d'échange de messages asynchrones via `window.postMessage` :

### 1. Ouverture
RisqueCV est conçu pour être ouvert depuis votre application via :

- **WebView (recommandé)** : RisqueCV détecte automatiquement son parent (`window.parent`) pour initier le dialogue.
- **Fenêtre Popup** : `window.open('https://risquecv.fr/slug-partenaire/')`. Cela permet une communication bilatérale fluide via la référence `window.opener`.
- **Iframe**  (compatible mais non recommandé)

### 2. Établissement de la Connexion (Handshake)

Le protocole suit une machine à états stricte pour garantir la sécurité des données :

1.  **Phase d'Écoute** : Dès l'ouverture, votre application doit se mettre à l'écoute de l'événement `message` global.
2.  **Signal "Ready" (RisqueCV ➡️ Partenaire)** : Une fois chargé, RisqueCV émet un message `risquecv:ready` pour vous informer que le tunnel de communication est ouvert et vous transmettre un `sessionId` unique.
    - *Obligation* : Vous devez renvoyer le `sessionId` reçu lors de toutes les étapes suivantes.
3.  **Injection "Prefill" (Partenaire ➡️ RisqueCV)** : En réponse au `ready`, vous devez envoyer vos données patient via un message `risquecv:prefill`.
4.  **Verrouillage de Session (Channel Locking)** : À la réception de votre premier message valide, RisqueCV **verrouille le canal**. Pour le reste de la session, RisqueCV n'acceptera plus aucun message provenant d'une autre origine ou d'une autre fenêtre que la vôtre.

### 3. Traitement des Données
L'algorithme de RisqueCV ne se contente pas de recevoir vos données, il assure leur intégrité :

- **Validation des Bornes** : Si vous envoyez une valeur cliniquement aberrante (ex: age = 300), le champ est ignoré pour protéger la cohérence médicale.
- **Accusé de Réception (`ack`)** : RisqueCV vous renvoie systématiquement un message `risquecv:prefill:ack`. Il contient la liste des clés acceptées et celles ignorées (clés inconnues ou valeurs hors-bornes).
- **Mise à jour Atomique** : L'injection des données dans l'interface de RisqueCV est immédiate et globale. Tous les scores et graphiques se recalculent en une seule passe dès réception de votre `prefill`.

### 4. UI adaptée au partenaire
- Bouton "Retour au Logiciel" (texte personnalisable, ex "Retour à Doctolib")
- Bouton PDF "Envoyer vers Logiciel" (texte personnalisable, ex "Envoyer vers Doctolib")

### 5. Récupération du Rapport (PDF)
Lorsque le médecin a terminé son évaluation sur RisqueCV :
1. En cliquant sur le bouton "Envoyer vers Logiciel", RisqueCV génère le rapport PDF localement dans le navigateur via la librairie `pdfmake` (aucune donnée n'est envoyée à nos serveurs).
2. Il vous transmet le PDF via un message `risquecv:pdf`.
3. Le payload contient le fichier encodé en **Base64**.

---

## 🔒 Garanties de Sécurité et Confidentialité

Ce protocole a été conçu pour répondre aux exigences les plus strictes de confidentialité (RGPD / HDS) :

- **Zéro Transit Internet** : Les données patient circulent exclusivement entre votre fenêtre et celle de RisqueCV dans la mémoire vive de l'ordinateur du médecin.
- **Zéro Persistance** : RisqueCV n'enregistre absolument rien concernant les données injectées (ni base de données, ni localstorage, ni cookies). Une fois la fenêtre fermée, les données sont définitivement purgées.
- **Isolation des Origines** : RisqueCV rejette tout message dont l'`event.origin` ne correspond pas strictement à un liste blanche de partenaires.
- **Pas de cookies** : RisqueCV n'utilise aucun cookie.
- **Pas de publicité** : RisqueCV n'affiche aucune publicité.

---

## 📖 Dictionnaire des Caractéristiques

Le `payload` peut contenir n'importe quelle combinaison des clés ci-dessous. Toutes les valeurs sont optionnelles (`null` ou omission pour ignorer). Toute clé inconnue sera ignorée.

### ⚠️ ATTENTION, ERREURS FREQUENTES :
<div style="background-color: #d4353560; padding: 10px; border-radius: 5px;">
- Respecter la <span style="font-weight: bold;">casse des clés</span> (ex: <code>PAS</code> et non <code>pas</code>, <code>HbA1c</code> et non <code>hba1c</code>, <code>age</code> et non <code>Age</code>, etc.).<br>
- Respecter les <span style="font-weight: bold;">unités mentionnées</span> (notamment <code>mmol/L</code> pour le cholestérol, <code>%</code> pour l'HbA1c).<br>
- Respecter le <span style="font-weight: bold;">typage des données</span>, il faut envoyer des nombres pour les nombres, des booléens pour les booléens, etc.<br>
- Ne pas envoyer de <span style="font-weight: bold;">données nominatives</span> (même si elles seront ignorées et non traitées).<br>
</div>




### 1. Les 4 premières questions systématiques de RisqueCV.fr
Ces booléens pilotent les 4 premières questions du formulaire.
Les mettre à `false` permet de sauter les questions de tri initiales.

| Clé | Type | Description | True si... |
| :--- | :--- | :--- | :--- |
| `atcd` | `boolean` | Antécédents de maladie cardiovasculaire avérée. | Maladie coronaire (angor, IDM, SCA revascularisation), AVC, AIT, AOMI, anévrisme de l'aorte abdominale (voir la liste complète sur le site, sous le titre "Antécédents cardiovasculaires") |
| `diabete` | `boolean` | Présence d'un diabète (Type 1 ou 2). | Diabète type 1 ou 2 |
| `MRC` | `boolean` | Maladie Rénale Chronique (DFG < 60 ou albuminurie). | DFG < 60 ou albuminurie ou "Maladie rénale chronique" |
| `autrepb` | `boolean` | Autres situations (HyperCHO familiale, HTA secondaire, etc.). | Hypercholestérolémie familiale hétérozygote, grossesse, etc. (voir la liste complète sur le site, sous le titre "Autre situation particulière ?") |

### 2. Valeurs numériques

| Clé | Type | Unité | Description |
| :--- | :--- | :--- | :--- |
| `age` | `number` | ans | Âge du patient |
| `PAS` | `number` | mmHg | Pression Artérielle Systolique (mesurée ce jour si possible). |
| `CT` | `number` | mmol/L | Cholestérol Total |
| `HDL` | `number` | mmol/L | Cholestérol HDL |
| `LDL` | `number` | mmol/L | Cholestérol LDL |
| `DFG` | `number` | mL/min | Débit de Filtration Glomérulaire |
| `HbA1c` | `number` | % | Hémoglobine glyquée |
| `crp` | `number` | mg/L | Protéine C-réactive ultra-sensible (hs-CRP) (attention pas la CRP standard) |
| `imc` | `number` | kg/m² | Indice de Masse Corporelle |
| `agediabete` | `number` | ans | Âge lors du diagnostic du diabète |
| `age_atcd` | `number` | ans | Âge lors du premier événement cardiovasculaire (AVC, AIT, SCA, IDM, AOMI, anévrisme de l'aorte abdominale) |

### 3. Valeurs de type `string`

| Clé | Type | Valeurs autorisées |
| :--- | :--- | :--- |
| `sexe` | `string` | `"homme"`, `"femme"` |
| `typediabete` | `string` | `"type1"`, `"type2"`, `"autre"` |
| `albuminurie` | `string` | `"non"`, `"micro"`, `"oui"` |
| `pays` | `string` | `"france"` |

### 4. Booléens

| Clé | Type | Description |
| :--- | :--- | :--- |
| `tabac` | `boolean` | Tabagisme actif actuel. |
| `aspirine` | `boolean` | Traitement antiagrégant plaquettaire en cours. |
| `insuline` | `boolean` | Diabète traité par insuline. |
| `hyperCHOfamille`| `boolean` | Hypercholestérolémie familiale hétérozygote connue. |
| `retinopathie` | `boolean` | Présence d'une rétinopathie diabétique. |

---

## 🛠 Exemple JS d'intégration côté partenaire

```javascript
// 1. Ouvrir la popup
const popup = window.open('https://risquecv.fr/srp-test/', 'RisqueCV');

// 2. Écouter les messages
window.addEventListener('message', (event) => {
    // Toujours vérifier l'origine !
    if (event.origin !== 'https://risquecv.fr') return;

    const version = 1;
    const msg = event.data;

    if (msg.type === 'risquecv:ready') {
        // 3. Envoyer les données patient
        popup.postMessage({
            type: 'risquecv:prefill',
            version: version,
            partner: msg.partner,
            sessionId: msg.sessionId,
            payload: { /* ...vos données... */ }
        }, event.origin);
    }

    if (msg.type === 'risquecv:pdf') {
        console.log("PDF reçu :", msg.filename);
        // Traitement du base64...
    }
});
```

---

## 📋 Catalogue des messages

Tous les messages partagent une structure de base : `type`, `version` (fixée à `1`) et `partner`.

### Étape 1 : Le Signal de Départ
#### 🟢 `risquecv:ready` (RisqueCV ➡️ Votre Logiciel)
Envoyé dès que RisqueCV est prêt à recevoir des données. Ce message contient le `sessionId` requis pour la suite.

```json
{
  "type": "risquecv:ready",
  "version": 1, // Il s'agit de la version du protocole d'intégration RisqueCV
  "partner": "votre-slug", // ex : "weda", "doctolib", "medistory", etc.
  "sessionId": "uuid-genere-par-risquecv", // Identifiant unique de la session
  "capabilities": {
    "prefill": true, // Indique que le partenaire est capable de pré-remplir les données
    "pdfReturn": "base64" // Indique que le partenaire est capable de recevoir le PDF en base64
  }
}
```

### Étape 2 : L'Injection des Données
#### 📝 `risquecv:prefill` (Votre Logiciel ➡️ RisqueCV)
Message de réponse au `ready`. Permet d'injecter le contexte patient.

```json
{
  "type": "risquecv:prefill",
  "version": 1,
  "partner": "votre-slug",
  "sessionId": "L_ID_RECU_DANS_READY",
  "payload": {
    "age": 55,
    "sexe": "femme",
    "tabac": false,
    "PAS": 142, // pour les valeurs numériques, il faut envoyer des nombres (pas d'unités)
    "atcd": true,
    // ... voir dictionnaire des clés ci-dessous
  }
}
```

### Étape 3 : La Confirmation
#### ✅ `risquecv:prefill:ack` (RisqueCV ➡️ Votre Logiciel)
Envoyé après réception du `prefill`. Confirme quelles données ont été validées et injectées.

```json
{
  "type": "risquecv:prefill:ack", // acknowledge
  "version": 1,
  "partner": "votre-slug",
  "sessionId": "L_ID_RECU_DANS_READY",
  "status": "ok", // "ok" ou "partial"
  "acceptedKeys": ["age", "sexe", "tabac", "atcd"],
  "ignoredKeys": ["cleInconnue"] 
}
```

### Étape 4 : Le Résultat (Finalisation)
#### 📄 `risquecv:pdf` (RisqueCV ➡️ Votre Logiciel)
Envoyé lorsque le médecin clique sur le bouton de transfert dans RisqueCV. Contient le document final.

```json
{
  "type": "risquecv:pdf",
  "version": 1,
  "partner": "votre-slug",
  "sessionId": "L_ID_RECU_DANS_READY",
  "filename": "RisqueCV_NomPatient.pdf",
  "mimeType": "application/pdf",
  "encoding": "base64",
  "data": "JVBERi..." // Flux binaire converti en string Base64 (environ 50kB)
}
```

---

### Cas Particulier : Gestion d'Erreur
#### 🛑 `risquecv:error` (RisqueCV ➡️ Votre Logiciel)
Envoyé en cas de rupture du protocole ou d'erreur critique de session.

| Code | Signification |
| :--- | :--- |
| `INVALID_ENVELOPE` | Le JSON ne respecte pas la structure de base. |
| `UNSUPPORTED_VERSION`| La version du protocole est différente de celle de RisqueCV. |
| `INVALID_SESSION` | Le `sessionId` est manquant ou incorrect. |
| `INVALID_PAYLOAD` | Le `payload` n'est pas un objet JSON plat. |
| `PREFILL_ALREADY_APPLIED` | Un `prefill` a déjà été appliqué pour cette session. |
| `INVALID_PARTNER` | Le slug partenaire ne correspond pas à l'URL ouverte. |

---

## 🛠 Débogage de l'intégration

Si vous rencontrez des difficultés (pas de réponse au handshake, données non injectées, etc.), vous pouvez activer le **Mode Verbeux** de RisqueCV.

Ajoutez simplement le paramètre `debug_integration=1` à l'URL :  
- `https://risquecv.fr/votre-slug/?debug_integration=1`


### Ce que le mode debug affiche dans votre console :

1.  **Confirmation d'Initialisation** :
    - `[RisqueCV] Initialisation intégration pour partenaire : votre-slug`
    - Valide que votre route d'intégration est correctement reconnue par WordPress.

2.  **Erreurs de Sécurité (Rejets silencieux)** :
    - `[RisqueCV] Origine non autorisée : https://votre-url-test.com` (Si votre domaine n'est pas dans notre liste blanche).
    - `[RisqueCV] Source de message non attendue.` (Si le message ne provient pas de l'objet `window` ayant ouvert RisqueCV).

3.  **Erreurs Protocolaires (Messages corrompus)** :
    - Chaque code d'erreur (`INVALID_SESSION`, `UNSUPPORTED_VERSION`, etc.) est journalisé avec une explication textuelle détaillée.
    - Facilite le débogage de vos payloads JSON sans avoir à inspecter manuellement chaque `event.data`.

<script src="https://cdnjs.cloudflare.com/ajax/libs/prism/1.29.0/prism.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/prism/1.29.0/components/prism-json.min.js"></script>