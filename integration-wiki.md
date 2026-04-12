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
        color: #1b2b7f;
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

    .warning {
        background-color: #d435352e;
        padding: 10px 15px;
        border-radius: 8px;
        color: #622525;
        line-height: 1.6;
    }

    @import url(https://fonts.googleapis.com/css?family=Fira+Mono);
/*
 * Thème Prism pour RisqueCV.fr
 * Couleurs VS Code Dark
 */

code[class*="language-"],
pre[class*="language-"] {
	font-family: "Fira Mono", Menlo, Monaco, "Lucida Console", "Courier New", Courier, monospace;
	font-size: 0.9em;
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
	word-break: keep-all;
	word-wrap: break-word;
	background: #b819401c;
	color: #b81940;
}


pre[class*="language-"]::selection,
code[class*="language-"]::selection,
pre[class*="language-"] *::selection,
code[class*="language-"] *::selection {
	text-shadow: none;
	background: #264F78;
}

@media print {
	pre[class*="language-"],
	code[class*="language-"] {
		text-shadow: none;
	}
}

pre[class*="language-"] {
	padding: 1em;
	margin: .5em 0;
	overflow: auto;
	background: #1e1e1e;
}

/*********************************************************
* Tokens
*/
.namespace {
	opacity: .7;
}

.token.doctype .token.doctype-tag {
	color: #569CD6;
}

.token.doctype .token.name {
	color: #9cdcfe;
}

.token.comment,
.token.prolog {
	color: #6a9955;
}

.token.punctuation,
.language-html .language-css .token.punctuation,
.language-html .language-javascript .token.punctuation {
	color: #d4d4d4;
}

.token.property,
.token.tag,
.token.boolean,
.token.number,
.token.constant,
.token.symbol,
.token.inserted,
.token.unit {
	color: #b5cea8;
}

.token.selector,
.token.attr-name,
.token.string,
.token.char,
.token.builtin,
.token.deleted {
	color: #ce9178;
}

.language-css .token.string.url {
	text-decoration: underline;
}

.token.operator,
.token.entity {
	color: #d4d4d4;
}

.token.operator.arrow {
	color: #569CD6;
}

.token.atrule {
	color: #ce9178;
}

.token.atrule .token.rule {
	color: #c586c0;
}

.token.atrule .token.url {
	color: #9cdcfe;
}

.token.atrule .token.url .token.function {
	color: #dcdcaa;
}

.token.atrule .token.url .token.punctuation {
	color: #d4d4d4;
}

.token.keyword {
	color: #569CD6;
}

.token.keyword.module,
.token.keyword.control-flow {
	color: #c586c0;
}

.token.function,
.token.function .token.maybe-class-name {
	color: #dcdcaa;
}

.token.regex {
	color: #d16969;
}

.token.important {
	color: #569cd6;
}

.token.italic {
	font-style: italic;
}

.token.constant {
	color: #9cdcfe;
}

.token.class-name,
.token.maybe-class-name {
	color: #4ec9b0;
}

.token.console {
	color: #9cdcfe;
}

.token.parameter {
	color: #9cdcfe;
}

.token.interpolation {
	color: #9cdcfe;
}

.token.punctuation.interpolation-punctuation {
	color: #569cd6;
}

.token.boolean {
	color: #569cd6;
}

.token.property,
.token.variable,
.token.imports .token.maybe-class-name,
.token.exports .token.maybe-class-name {
	color: #9cdcfe;
}

.token.selector {
	color: #d7ba7d;
}

.token.escape {
	color: #d7ba7d;
}

.token.tag {
	color: #569cd6;
}

.token.tag .token.punctuation {
	color: #808080;
}

.token.cdata {
	color: #808080;
}

.token.attr-name {
	color: #9cdcfe;
}

.token.attr-value,
.token.attr-value .token.punctuation {
	color: #ce9178;
}

.token.attr-value .token.punctuation.attr-equals {
	color: #d4d4d4;
}

.token.entity {
	color: #569cd6;
}

.token.namespace {
	color: #4ec9b0;
}
/*********************************************************
* Language Specific
*/

pre[class*="language-javascript"],
code[class*="language-javascript"],
pre[class*="language-jsx"],
code[class*="language-jsx"],
pre[class*="language-typescript"],
code[class*="language-typescript"],
pre[class*="language-tsx"],
code[class*="language-tsx"] {
	color: #9cdcfe;
}

pre[class*="language-css"],
code[class*="language-css"] {
	color: #ce9178;
}

pre[class*="language-html"],
code[class*="language-html"] {
	color: #d4d4d4;
}

.language-regex .token.anchor {
	color: #dcdcaa;
}

.language-html .token.punctuation {
	color: #808080;
}
/*********************************************************
* Line highlighting
*/
pre[class*="language-"] > code[class*="language-"] {
	position: relative;
	z-index: 1;
}

.line-highlight.line-highlight {
	background: #f7ebc6;
	box-shadow: inset 5px 0 0 #f7d87c;
	z-index: 0;
}

.markdown-body .highlight pre, .markdown-body pre {
    padding: 16px;
    overflow: auto;
    font-size: 85%;
    line-height: 1.45;
    background-color: #1f1f1f;
    border-radius: 8px;
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
<div class="warning">
- Respecter la <span style="font-weight: bold;">casse des clés</span> (ex: <code class="language-plaintext">PAS</code> et non <code class="language-plaintext">pas</code>, <code class="language-plaintext">HbA1c</code> et non <code class="language-plaintext">hba1c</code>, <code class="language-plaintext">age</code> et non <code class="language-plaintext">Age</code>, etc.).<br>
- Respecter les <span style="font-weight: bold;">unités mentionnées</span> (notamment <code class="language-plaintext">mmol/L</code> pour le cholestérol, <code class="language-plaintext">%</code> pour l'HbA1c).<br>
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
| `neuropathie` | `boolean` | Présence d'une neuropathie diabétique. |
| `atcd_coronarien` | `boolean` | Antécédent de maladie coronaire (IDM, SCA, revascularisation). |
| `atcd_cerebrovasculaire`| `boolean` | Antécédent d'AVC ou d'AIT. |
| `atcd_aomi` | `boolean` | Antécédent d'Artériopathie Oblitérante des Membres Inférieurs. |
| `atcd_anevrismeAorte`| `boolean` | Antécédent d'anévrisme de l'aorte abdominale. |
| `microangiopathie3sites`| `boolean` | Présence d'une microangiopathie sur ≥3 sites (ex: rétino + neuro + albu). |
| `autreFacteurMajeur` | `boolean` | Présence d'un autre facteur de risque majeur (pour l'HF). |
| `evaluationComplete`| `boolean` | Force l'affichage de l'évaluation complète (tunnel détaillé). |

---

## 🛠 Exemple JS d'intégration côté partenaire

### Avec popup
```javascript
// --- 1. CONFIGURATION ---
const CONFIG = {
    version: 1, // Version du protocole d'intégration RisqueCV
    partnerSlug: 'votre-slug', // Identifiant de votre logiciel (ex : "weda"))
    targetOrigin: 'https://risquecv.fr', // Origine stricte
    popupOptions: 'width=1100,height=800'
};

// --- 2. ÉTAT DE LA SESSION ---
let popupWindow = null;
let messageListener = null;
let pollClosedInterval = null;
let handshakeTimeout = null;

// --- 3. DÉCLENCHEMENT DE L'OUVERTURE ---
document.getElementById('bouton-ouvrir-risquecv').addEventListener('click', () => {
    
    // Anti-spam : ramener la fenêtre au premier plan si elle est déjà ouverte
    if (popupWindow && !popupWindow.closed) {
        popupWindow.focus();
        return; 
    }

    // Nettoyage des anciennes sessions
    cleanupSession();

    // Ouverture de l'interface RisqueCV
    popupWindow = window.open(`${CONFIG.targetOrigin}/${CONFIG.partnerSlug}/`, 'RisqueCV', CONFIG.popupOptions);
    
    if (!popupWindow) {
        alert("Ouverture bloquée. Veuillez autoriser les pop-ups pour utiliser RisqueCV.");
        return;
    }

    // Timeout si le site distant est inaccessible
    handshakeTimeout = setTimeout(() => {
        console.warn("⏳ Délai d'attente dépassé : RisqueCV ne répond pas.");
    }, 5000);

    // Détection de la fermeture manuelle par l'utilisateur
    pollClosedInterval = setInterval(() => {
        if (popupWindow.closed) {
            console.info("ℹ️ Session RisqueCV terminée (fenêtre fermée manuellement).");
            cleanupSession();
        }
    }, 1000);

    // --- 4. GESTION DES MESSAGES ---
    messageListener = (event) => {
        // Ignorer tout message ne provenant pas de RisqueCV
        if (event.origin !== CONFIG.targetOrigin) return;
        
        const msg = event.data;

        switch (msg.type) {
          // Si on reçoit "ready", alors on peut envoyer les données du patient
            case 'risquecv:ready':
                clearTimeout(handshakeTimeout);

                // A. Envoie des données cliniques du patient
                popupWindow.postMessage({
                    type: 'risquecv:prefill',
                    version: CONFIG.version,
                    partner: msg.partner,
                    sessionId: msg.sessionId,
                    payload: { 
                      // Les données doivent être formatées avant l'envoi (ex: "femme" et pas "Femme" ni "F")
                        age: 55, 
                        sexe: "femme", 
                        tabac: false,
                        PAS: 142,
                        CT: 5.2,
                        HDL: 1.3
                        // Ajoutez vos autres variables cliniques ici. Le payload n'a pas besoin d'être exhaustif.
                    }
                }, CONFIG.targetOrigin);
                break;

            // Si on reçoit "ack", alors RisqueCV a bien reçu les données
            case 'risquecv:prefill:ack':
                // Si necessaire pour debug, on peut vérifier l'injection
                if (msg.status === 'partial') {
                    console.warn('⚠️ Données ignorées par RisqueCV (hors-bornes ou inconnues) :', msg.ignoredKeys);
                }
                break;

            // Si on reçoit "pdf", alors on peut sauvegarder le PDF recu dans le dossier du patient
            case 'risquecv:pdf':                
                // Fermeture optionnelle de la popup
                popupWindow.close();

                // Nettoyage des écouteurs
                cleanupSession();

                // Envoi silencieux du Base64 vers votre API
                sauvegarderPdfEnBaseDeDonnees(msg.data, msg.filename);
                break;

            // Si on reçoit "error", alors.... il y a eu une erreur 😁
            case 'risquecv:error':
                console.error(`❌ Erreur RisqueCV [${msg.code}]:`, msg.message);
                break;
        }
    };

    window.addEventListener('message', messageListener);
});

// --- 5. FONCTIONS UTILITAIRES ---

/** Nettoie les écouteurs pour éviter les fuites de mémoire (memory leaks) */
function cleanupSession() {
    if (messageListener) {
        window.removeEventListener('message', messageListener);
        messageListener = null;
    }
    if (pollClosedInterval) {
        clearInterval(pollClosedInterval);
        pollClosedInterval = null;
    }
    if (handshakeTimeout) {
        clearTimeout(handshakeTimeout);
        handshakeTimeout = null;
    }
}

/** Transmet le PDF (Base64) à votre API pour l'enregistrer dans le dossier patient */
async function sauvegarderPdfEnBaseDeDonnees(base64Data, filename) {
    try {
        const response = await fetch('/api/votre-logiciel/patients/12345/documents', {
            method: 'POST',
            headers: { 'Content-Type': 'application/json' },
            body: JSON.stringify({
                nom_fichier: filename,
                contenu_base64: base64Data,
                type_document: 'EVALUATION_RISQUE_CV'
            })
        });

        if (response.ok) {
            console.log("✅ PDF sauvegardé avec succès dans le dossier du patient.");
        } else {
            console.error("❌ Échec de la sauvegarde du PDF côté serveur.");
        }
    } catch (error) {
        console.error("Erreur réseau lors de la sauvegarde du PDF :", error);
    }
}
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
    // ... voir dictionnaire des clés ci-dessus
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
| `UNSUPPORTED_MESSAGE_TYPE`| Le type de message (`type`) n'est pas pris en charge. |
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