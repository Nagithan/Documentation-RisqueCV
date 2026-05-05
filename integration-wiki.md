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

    details summary {
        cursor: pointer;
        line-height: 2.1;
        font-size: 1.1em;
        font-weight: 500;
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

    /* Sandbox Test Button & Status */
    .sandbox-test-container {
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 12px;
        margin: 25px 0;
        flex-wrap: wrap;
    }

    .bouton-sandbox {
        position: relative;
        overflow: hidden;
        font-family: inherit;
        font-weight: 600;
        font-size: 1.13em;
        line-height: 1.15;
        border-radius: 14px;
        padding: 10px 16px;
        cursor: pointer;
        -webkit-user-select: none;
        user-select: none;
        transition: background-color 0.16s ease, border-color 0.16s ease, color 0.16s ease, transform 0.16s ease, box-shadow 0.16s ease;
        display: inline-flex;
        align-items: center;
        gap: 10px;
        border: 1px solid;
    }

    /* Thème Red (Bouton principal) */
    .bouton-sandbox--red {
        background: #7100001F;
        color: #6d1525;
        border-color: #b17b7b;
    }
    .bouton-sandbox--red:hover {
        background: #7e00002e;
        border-color: #a76772;
        color: #5d1020;
    }
    .bouton-sandbox--red:active {
        background: #7100002e;
        border-color: #965564;
        transform: scale(0.98);
    }
    .bouton-sandbox--red:focus-visible {
        border-color: #8f4c5d;
        outline: none;
        box-shadow: 0 0 0 2px rgba(164, 24, 53, 0.18);
    }

    /* Thème LightBlue (Bouton PDF) */
    .bouton-sandbox--lightblue {
        background: #eef2ff;
        color: #1e3a8a;
        border-color: #bacae1;
        display: none; /* Caché par défaut */
        animation: slideIn 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    }
    .bouton-sandbox--lightblue:hover {
        background: #e6effc;
        border-color: #c7d2fe;
        color: #172554;
    }
    .bouton-sandbox--lightblue:active {
        background: #e0ecfc;
        border-color: #bcc2df;
        transform: scale(0.98);
    }
    .bouton-sandbox--lightblue:focus-visible {
        border-color: #a5b4fc;
        outline: none;
        box-shadow: 0 0 0 2px rgba(30, 58, 138, 0.2);
    }

    .status-pill {
        display: none;
        align-items: center;
        gap: 8px;
        padding: 8px 16px;
        border-radius: 20px;
        background: #f8fafc;
        border: 1px solid #e2e8f0;
        font-size: 0.9em;
        font-weight: 600;
        color: #64748b;
        box-shadow: 0 2px 4px rgba(0,0,0,0.02);
        animation: fadeIn 0.3s ease;
    }

    .status-pill.is-active {
        display: flex;
        border-color: #bbf7d0;
        background: #f0fdf4;
        color: #166534;
    }

    .status-pill .dot {
        width: 8px;
        height: 8px;
        border-radius: 50%;
        background: #cbd5e1;
    }

    .status-pill.is-active .dot {
        background: #22c55e;
        box-shadow: 0 0 8px rgba(34, 197, 94, 0.4);
    }

    @keyframes slideIn {
        from { opacity: 0; transform: translateX(15px); }
        to { opacity: 1; transform: translateX(0); }
    }

    /* Journal PostMessage */
    .sandbox-log {
        display: none;
        margin-top: 15px;
        background: #1e1e1e;
        color: #d4d4d4;
        border-radius: 10px;
        padding: 12px;
        font-family: 'Fira Mono', monospace;
        font-size: 0.85em;
        max-height: 300px;
        overflow-y: auto;
        border: 1px solid #333;
        box-shadow: inset 0 2px 10px rgba(0,0,0,0.2);
        animation: fadeIn 0.3s ease;
    }

    .log-entry {
        margin-bottom: 8px;
        padding-bottom: 8px;
        border-bottom: 1px solid #333;
        line-height: 1.4;
    }

    .log-entry:last-child { border-bottom: none; margin-bottom: 0; padding-bottom: 0; }

    .log-header { display: flex; align-items: center; }
    .log-time { color: #888; margin-right: 10px; font-size: 0.8em; }
    .log-dir { font-weight: bold; margin-right: 8px; font-size: 0.9em; }
    .log-in { color: #4ec9b0; }
    .log-out { color: #ce9178; }
    .log-data { color: #9cdcfe; display: block; margin-top: 4px; white-space: pre-wrap; word-break: break-all; font-size: 0.95em; }
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

<div class="sandbox-test-container">
    <button id="sandbox-trigger" class="bouton-sandbox bouton-sandbox--red">
        <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 1024 1024" style="fill: currentColor;"><path d="M960 704a64 64 0 0 0-64 64v64a64 64 0 0 1-64 64H192a64 64 0 0 1-64-64V192a64 64 0 0 1 64-64h64a64 64 0 0 0 0-128h-64C85.96 0 0 85.96 0 192v640c0 106.04 85.96 192 192 192h640c106.04 0 192-85.96 192-192v-64a64 64 0 0 0-64-64"/><path d="M1023.88 51.52c0-1.92 0-3.84-1.6-5.44a64 64 0 0 0-1.92-6.4 64 64 0 0 0-3.2-6.4s0-3.2-2.56-4.8a64 64 0 0 0-17.6-17.6L991.88 8l-6.08-3.2-6.72-1.92h-5.44A64 64 0 0 0 959.88 0h-384a64 64 0 0 0 0 128h229.44L434.76 498.88a64.04 64.04 0 0 0 90.56 90.56l370.56-370.88V448a64 64 0 0 0 128 0V64q.6-6.24 0-12.48"/></svg>
        <span>Tester l'interface d'intégration</span>
    </button>
    <button id="sandbox-pdf" class="bouton-sandbox bouton-sandbox--lightblue">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 256 256" width="18" height="18" style="fill: currentColor;"><path d="M152 32v56h56.008z" opacity=".2"/><path d="M216.008 88a7.97 7.97 0 0 0-2.432-5.738l-55.919-55.918q-.277-.277-.58-.526c-.05-.04-.102-.075-.153-.114a8 8 0 0 0-.477-.353c-.045-.03-.093-.055-.138-.085a8 8 0 0 0-.535-.32q-.05-.024-.103-.049a8 8 0 0 0-.605-.286c-.023-.01-.047-.016-.071-.026a8 8 0 0 0-.664-.238q-.04-.01-.08-.02a8 8 0 0 0-.676-.17c-.066-.013-.133-.019-.199-.03-.19-.034-.382-.067-.577-.087A8 8 0 0 0 152 24H55.992a16.02 16.02 0 0 0-16 16v176a16.02 16.02 0 0 0 16 16H200a16.02 16.02 0 0 0 16-16V88.16c.001-.054.008-.106.008-.16M160 51.314 188.687 80H160ZM200 216H55.992V40H144v48a8 8 0 0 0 8 8h48l.01 120Z"/><path d="M150.343 150.343 136 164.687V120a8 8 0 0 0-16 0v44.687l-14.343-14.344a8 8 0 0 0-11.314 11.314l28 28c.026.026.055.048.081.074q.242.237.504.455c.097.08.2.15.301.225.109.081.215.165.328.24.116.079.237.146.357.218.105.062.207.128.315.185.12.065.244.12.366.177.114.054.227.111.343.16.119.049.24.088.36.13.126.046.25.095.38.134.12.036.241.063.362.093.132.033.263.07.397.097.14.028.28.044.42.064.119.017.234.04.353.051a8 8 0 0 0 1.58 0c.119-.012.234-.034.353-.05.14-.021.28-.037.42-.065.134-.027.265-.064.397-.097.121-.03.243-.057.362-.093.13-.04.254-.088.38-.133.12-.043.241-.082.36-.131.116-.049.229-.106.343-.16.122-.058.246-.112.366-.177.108-.057.21-.123.315-.185.12-.072.24-.14.357-.217.113-.076.22-.16.328-.241.1-.075.204-.145.301-.225q.266-.221.513-.464c.023-.023.049-.042.072-.065l28-28a8 8 0 0 0-11.314-11.314"/></svg>
        <span>Ouvrir le PDF reçu</span>
    </button>
    <div id="sandbox-status" class="status-pill">
        <span class="dot"></span>
        <span class="text">Attente...</span>
    </div>
</div>

<div id="sandbox-log" class="sandbox-log"></div>

<script>
(function() {
    let popup = null;
    let pdfData = null;
    let messageListener = null;
    let pollClosedInterval = null;
    let handshakeTimeout = null;

    const targetUrl = 'https://risquecv.local/test-integration';
    const partnerSlug = 'test-integration';

    const btn = document.getElementById('sandbox-trigger');
    const status = document.getElementById('sandbox-status');
    const pdfPill = document.getElementById('sandbox-pdf');
    const logContainer = document.getElementById('sandbox-log');

    function cleanup() {
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

    function log(dir, data) {
        const entry = document.createElement('div');
        entry.className = 'log-entry';
        const time = new Date().toLocaleTimeString();
        const dirClass = dir === 'IN' ? 'log-in' : 'log-out';
        const dirText = dir === 'IN' ? '← REÇU' : '→ ENVOI';
        if (dir === 'SYSTEM') {
            entry.innerHTML = `<div class="log-header"><span class="log-time">${time}</span><span class="log-dir" style="color:#569cd6">[SYSTEM]</span></div><code class="log-data">${data}</code>`;
        } else {
            entry.innerHTML = `
                <div class="log-header">
                    <span class="log-time">${time}</span>
                    <span class="log-dir ${dirClass}">${dirText}</span>
                </div>
                <code class="log-data">${JSON.stringify(data, null, 2)}</code>
            `;
        }
        logContainer.prepend(entry);
        logContainer.style.display = 'block';
    }

    btn.addEventListener('click', () => {
        // Anti-spam : focus si déjà ouvert
        if (popup && !popup.closed) {
            popup.focus();
            return;
        }

        cleanup();
        logContainer.innerHTML = '';
        pdfPill.style.display = 'none';
        pdfData = null;

        popup = window.open(targetUrl, '_blank');
        if (!popup) {
            alert("L'ouverture de l'onglet de test a été bloquée. Veuillez autoriser les pop-ups.");
            return;
        }

        status.style.display = 'flex';
        status.classList.remove('is-active');
        status.querySelector('.text').textContent = 'Attente connexion...';
        log('SYSTEM', 'Ouverture de RisqueCV...');

        // Détection fermeture manuelle
        pollClosedInterval = setInterval(() => {
            if (popup && popup.closed) {
                status.classList.remove('is-active');
                status.querySelector('.text').textContent = 'Onglet fermé';
                log('SYSTEM', 'L\'onglet a été fermé par l\'utilisateur.');
                cleanup();
            }
        }, 1000);

        // Timeout et Ping
        handshakeTimeout = setTimeout(() => {
            if (popup && !popup.closed) {
                log('SYSTEM', 'Délai dépassé, tentative de Ping...');
                const p = { type: 'risquecv:ping' };
                popup.postMessage(p, new URL(targetUrl).origin);
                log('OUT', p);
            }
        }, 3000);

        messageListener = (e) => {
            let origin;
            try { origin = new URL(targetUrl).origin; } catch(x) { return; }
            if (e.origin !== origin) return;

            const m = e.data;
            log('IN', m);

            if (m.type === 'risquecv:ready') {
                clearTimeout(handshakeTimeout);
                status.classList.add('is-active');
                status.querySelector('.text').textContent = 'Connecté';
                
                setTimeout(() => {
                    const payload = {
                        type: 'risquecv:prefill',
                        version: 1,
                        partner: partnerSlug,
                        sessionId: m.sessionId,
                        payload: {
                            pays: 'France', age: 52, sexe: 'homme', 
                            PAS: 155, CT: 6.2, HDL: 1.1, LDL: 4.1,
                            atcd: false, diabete: false, MRC: false, autrepb: false, tabac: false
                        }
                    };
                    popup.postMessage(payload, origin);
                    log('OUT', payload);
                }, 50);

            } else if (m.type === 'risquecv:pdf') {
                pdfData = m.data;
                pdfPill.style.display = 'flex';
                status.querySelector('.text').textContent = 'PDF REÇU ✅';
            } else if (m.type === 'risquecv:close') {
                if (popup && !popup.closed) popup.close();
                // Le setInterval s'occupera du cleanup
            }
        };

        window.addEventListener('message', messageListener);
    });

    pdfPill.addEventListener('click', () => {
        if (!pdfData) return;
        try {
            const b = atob(pdfData);
            const n = b.length;
            const a = new Uint8Array(n);
            for (let i = 0; i < n; i++) a[i] = b.charCodeAt(i);
            const blob = new Blob([a], { type: 'application/pdf' });
            window.open(URL.createObjectURL(blob), '_blank');
        } catch (err) { console.error(err); }
    });
})();
</script>


---

## 🏗 Architecture du protocole

L'intégration repose sur un protocole d'échange de messages asynchrones via `window.postMessage` :

### 1. Ouverture
RisqueCV est conçu pour être ouvert depuis votre application via :

- **WebView (recommandé)** : RisqueCV détecte automatiquement son parent (`window.parent`) pour initier le dialogue.
- **Fenêtre popup nouvel onglet (recommandé)** : `window.open('https://risquecv.fr/slug-partenaire/', '_blank')`. Cela permet une communication bilatérale fluide via la référence `window.opener`.
- **Iframe** : compatible mais non recommandé pour des raisons d'UI/UX

### 2. Établissement de la connexion ("handshake")

Le protocole suit une machine à états stricte pour garantir la sécurité des données :

1.  **Phase d'écoute** : Dès l'ouverture, votre application doit se mettre à l'écoute de l'événement `message` global.
2.  **Signal "ready" (RisqueCV ➡️ Partenaire)** : Une fois chargé, RisqueCV émet un message `risquecv:ready` pour vous informer que le tunnel de communication est ouvert et vous transmettre un `sessionId` unique.
    - *Obligation* : Vous devez renvoyer le `sessionId` reçu lors de l'étape de prefill.
3.  **Signal "ping" (Partenaire ➡️ RisqueCV)** : Si votre application a manqué le signal initial (chargement asynchrone), vous pouvez envoyer un message `{ "type": "risquecv:ping" }`. RisqueCV renverra immédiatement le signal `ready`.
4.  **Injection "prefill" (Partenaire ➡️ RisqueCV)** : En réponse au `ready`, vous envoyez vos données patient via un message `risquecv:prefill`.
5.  **Verrouillage de session (Channel Locking)** : À la réception de votre premier message de données (**prefill**), RisqueCV **verrouille le canal**. Pour le reste de la session, RisqueCV n'acceptera plus aucun message provenant d'une autre origine ou d'une autre fenêtre que la vôtre.

### 3. Traitement des données
L'algorithme de RisqueCV ne se contente pas de recevoir vos données, il assure leur intégrité :

- **Validation des bornes** : Si vous envoyez une valeur cliniquement aberrante (ex: age = 300), le champ est ignoré pour protéger la cohérence médicale.
- **Accusé de réception (`ack`)** : RisqueCV vous renvoie systématiquement un message `risquecv:prefill:ack`. Il contient la liste des clés acceptées et celles ignorées (clés inconnues ou valeurs hors-bornes).
- **Mise à jour atomique** : L'injection des données dans l'interface de RisqueCV est immédiate et globale. Tous les scores et graphiques se recalculent en une seule passe dès réception de votre `prefill`.

### 4. UI adaptée au partenaire
- Bouton "Retour au Logiciel" (texte personnalisable, ex "Retour à Doctolib")
- Bouton PDF "Envoyer vers Logiciel" (texte personnalisable, ex "Envoyer vers Doctolib")

### 5. Récupération du rapport (PDF)
Lorsque le médecin a terminé son évaluation sur RisqueCV :
1. En cliquant sur le bouton "Envoyer vers Logiciel", RisqueCV génère le rapport PDF localement dans le navigateur via la librairie `pdfmake` (aucune donnée n'est envoyée à nos serveurs).
2. Il vous transmet le PDF via un message `risquecv:pdf`.
3. Le payload contient le fichier encodé en **Base64**.
4. **En cas d'échec** (ex: erreur mémoire), RisqueCV émet un message `risquecv:error` avec le code `PDF_GENERATION_FAILED`.

### 6. Fermeture de session
Lors du clic sur le bouton de retour, RisqueCV émet un signal `risquecv:close`. Voir la section "Résilience" ci-dessous pour la gestion des Iframes.

---

## 🔒 Sécurité et confidentialité

Ce protocole a été conçu pour répondre aux exigences les plus strictes de confidentialité (RGPD / HDS) :

- **Zéro transit Internet** : Les données patient circulent exclusivement entre votre fenêtre et celle de RisqueCV dans la mémoire vive de l'ordinateur du médecin.
- **Zéro persistance** : RisqueCV n'enregistre absolument rien concernant les données injectées (ni base de données, ni localstorage, ni cookies). Une fois la fenêtre fermée, les données sont définitivement purgées.
- **Isolation des origines** : RisqueCV rejette tout message dont l'`event.origin` ne correspond pas strictement à un liste blanche de partenaires.
- **Pas de cookies** : RisqueCV n'utilise aucun cookie.
- **Pas de publicité** : RisqueCV n'affiche aucune publicité.

---

## 🛡️ Résilience et Protocoles de repli

Pour garantir une expérience sans friction, RisqueCV implémente plusieurs mécanismes de sécurité :

### Délai de repli (Handshake Timeout)
Si RisqueCV est ouvert en mode intégration mais ne reçoit **aucun trafic valide** (ni ping, ni prefill) dans les **5 secondes** suivant son chargement, il bascule automatiquement en **Mode Standard** (autonome). Cela évite de bloquer le médecin si votre logiciel métier subit un bug technique.

### Prévention de l'Inception (Iframes)
Rediriger une Iframe vers une URL externe peut provoquer le chargement de votre propre portail à l'intérieur de l'Iframe (Effet Inception). 
- **Dans une Iframe** : RisqueCV émet le message `risquecv:close` et **reste sur sa page**. C'est à votre application de capter ce message pour détruire l'Iframe (pour éviter l'inception)
- **Dans un Nouvel onglet / Popup** : RisqueCV émet le message, tente de s'auto-fermer (`window.close()`), et n'utilise sa redirection de secours (`returnUrl`) qu'en tout dernier recours.

---

## 🌐 Configuration Serveur (CSP)

Pour que votre logiciel puisse intégrer RisqueCV dans une Iframe, le serveur de RisqueCV doit vous y autoriser (`Content-Security-Policy: frame-ancestors`). Si vous constatez une erreur "Clickjacking" ou "Refused to frame", demandez à ce que votre domaine soit bien whitelisté dans nos entêtes.

---

## 📖 Dictionnaire des caractéristiques

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

### 3. Valeurs de type string

| Clé | Type | Valeurs autorisées (exemples) |
| :--- | :--- | :--- |
| `sexe` | `string` | `"homme"`, `"femme"` |
| `typediabete` | `string` | `"type1"`, `"type2"`, `"autre"` |
| `albuminurie` | `string` | `"non"`, `"micro"`, `"oui"` |
| `pays` | `string` | `"France"`, `"region_low"`, `"region_moderate"`, `"region_high"`, `"region_veryhigh"` |

> *Note sur la région/pays :* Nous recommandons d'utiliser directement les codes de stratification européenne du risque (`"region_low"`, `"region_moderate"`, `"region_high"`, `"region_veryhigh"`) si votre logiciel en dispose. À défaut, vous pouvez envoyer le nom du pays européen en toutes lettres (ex: `"France"`, `"Belgique"`), RisqueCV déduira automatiquement la région associée.

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

## 🛠 Exemples JS d'intégration côté partenaire

Voici des exemples prêts à l'emploi selon la méthode de rendu que vous utilisez (WebView ou Popup). N'hésitez pas à les dérouler pour voir le code.

<details class="code-spoiler" markdown="1">
<summary>💻 Exemple d'intégration pour WebView (Electron, React Native...)</summary>

```javascript
// --- 1. CONFIGURATION ---
const CONFIG = {
    version: 1, // Version du protocole d'intégration RisqueCV
    partnerSlug: 'votre-slug', // Identifiant de votre logiciel (ex : "weda")
    targetOrigin: 'https://risquecv.fr' // Origine stricte
};

// --- 2. ÉTAT DE LA SESSION ---
const webview = document.getElementById('risquecv-webview');
let handshakeTimeout = null;

// --- 3. FONCTIONS UTILITAIRES ---
function fermerWebView() {
    webview.style.display = 'none';
    webview.src = 'about:blank';
}

/** Transmet le PDF (Base64) à votre API pour l'enregistrer dans le dossier patient */
async function sauvegarderPdf(base64Data, filename) {
    try {
        console.log(`Enregistrement du PDF ${filename} en cours...`);
        
        // Exemple d'appel API interne à votre logiciel
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
            console.log("✅ PDF sauvegardé avec succès dans le dossier patient.");
        } else {
            console.error("❌ Échec de la sauvegarde côté serveur.");
        }
    } catch (error) {
        console.error("Erreur technique lors de la sauvegarde du PDF :", error);
    }
}

// --- 4. DÉCLENCHEMENT DE L'OUVERTURE ---
document.getElementById('bouton-ouvrir-risquecv').addEventListener('click', () => {
    
    // Charger l'URL d'intégration
    webview.src = `${CONFIG.targetOrigin}/${CONFIG.partnerSlug}/`;
    webview.style.display = 'block'; 
    
    // Sécurité : Timeout si le chargement échoue. On effectue un "Ping" pro-actif.
    handshakeTimeout = setTimeout(() => {
        console.warn("⏳ Délai d'attente dépassé : RisqueCV ne répond pas. Tentative de Ping...");
        // L'envoi dépend de votre framework (ici webview standard HTML5)
        if (webview.contentWindow) {
            webview.contentWindow.postMessage({ type: 'risquecv:ping' }, CONFIG.targetOrigin);
        }
    }, 3000);
});

// --- 5. GESTION DES MESSAGES ---

// L'écouteur dépend de votre pont natif. window.addEventListener (Electron), window.chrome.webview.addEventListener (WebView2), etc.
window.addEventListener('message', (event) => {
    
    // Ignorer tout message ne provenant pas de RisqueCV
    if (event.origin !== CONFIG.targetOrigin) return;
    
    const msg = event.data;

    switch (msg.type) {
        
        // Si on reçoit "ready", alors on peut envoyer les données du patient
        case 'risquecv:ready':
            clearTimeout(handshakeTimeout);

            // Envoi des données cliniques du patient
            const payloadMessage = {
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
            };

            webview.contentWindow.postMessage(payloadMessage, CONFIG.targetOrigin);
            break;

        // Si on reçoit "ack", alors RisqueCV a bien reçu les données
        case 'risquecv:prefill:ack':
            // Si nécessaire pour debug, on peut vérifier l'injection
            if (msg.status === 'partial') {
                console.warn('⚠️ Données ignorées par RisqueCV (hors-bornes ou inconnues) :', msg.ignoredKeys);
            }
            break;

        // Si on reçoit "pdf", alors on peut sauvegarder le PDF recu dans le dossier du patient
        case 'risquecv:pdf':
            fermerWebView();
            sauvegarderPdf(msg.data, msg.filename);
            break;

        // Si le médecin clique sur le bouton "Retour au logiciel", on masque l'interface
        case 'risquecv:close':
            console.log("Fermeture demandée par RisqueCV.");
            fermerWebView();
            break;

        // Si on reçoit "error", il y a eu un problème métier ou protocolaire
        case 'risquecv:error':
            console.error(`❌ Erreur RisqueCV [${msg.code}]:`, msg.message);
            break;
    }
});
```

</details>

<details class="code-spoiler" markdown="1">
<summary>💻 Exemple d'intégration avec fenêtre popup dans un nouvel onglet</summary>

```javascript
// --- 1. CONFIGURATION ---
const CONFIG = {
    version: 1, // Version du protocole d'intégration RisqueCV
    partnerSlug: 'votre-slug', // Identifiant de votre logiciel (ex : "weda"))
    targetOrigin: 'https://risquecv.fr' // Origine stricte
};

// --- 2. ÉTAT DE LA SESSION ---
let popupWindow = null;
let messageListener = null;
let pollClosedInterval = null;
let handshakeTimeout = null;

// --- 3. FONCTIONS UTILITAIRES ---

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
    popupWindow = null;
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

// --- 4. DÉCLENCHEMENT DE L'OUVERTURE ---
document.getElementById('bouton-ouvrir-risquecv').addEventListener('click', () => {
    
    // Anti-spam : ramener la fenêtre au premier plan si elle est déjà ouverte (ne pas relancer le window.open pour éviter de recharger la page et de casser le Handshake)
    if (popupWindow && !popupWindow.closed) {
        popupWindow.focus();
        return; 
    }

    // Nettoyage complet avant ouverture
    cleanupSession();

    // Ouverture de l'interface RisqueCV dans un nouvel onglet
    popupWindow = window.open(`${CONFIG.targetOrigin}/${CONFIG.partnerSlug}/`, '_blank');
    
    if (!popupWindow) {
        alert("Ouverture bloquée. Veuillez autoriser les pop-ups pour utiliser RisqueCV.");
        return;
    }

    // Détection de la fermeture manuelle par l'utilisateur (croix de la fenêtre)
    pollClosedInterval = setInterval(() => {
        if (popupWindow && popupWindow.closed) {
            console.info("ℹ️ Session RisqueCV terminée (fenêtre fermée par l'utilisateur).");
            cleanupSession();
        }
    }, 1000);

    // Timeout si le site distant est inaccessible. On effectue un "Ping" pro-actif.
    handshakeTimeout = setTimeout(() => {
        console.warn("⏳ Délai d'attente dépassé : RisqueCV ne répond pas. Tentative de Ping...");
        if (popupWindow && !popupWindow.closed) {
            popupWindow.postMessage({ type: 'risquecv:ping' }, CONFIG.targetOrigin);
        }
    }, 3000);

    // --- 5. GESTION DES MESSAGES ---
    messageListener = (event) => {
        // Ignorer tout message ne provenant pas de RisqueCV
        if (event.origin !== CONFIG.targetOrigin) return;
        
        const msg = event.data;

        switch (msg.type) {
          // Si on reçoit "ready", alors on peut envoyer les données du patient
            case 'risquecv:ready':
                clearTimeout(handshakeTimeout);

                // Envoi des données cliniques du patient
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
                // Si nécessaire pour debug, on peut vérifier l'injection
                if (msg.status === 'partial') {
                    console.warn('⚠️ Données ignorées par RisqueCV (hors-bornes ou inconnues) :', msg.ignoredKeys);
                }
                break;

            // Si on reçoit "pdf", alors on peut sauvegarder le PDF recu dans le dossier du patient
            case 'risquecv:pdf':                
                // Fermeture propre de la popup
                if (popupWindow) popupWindow.close();
                cleanupSession();

                // Enregistrement du PDF dans le dossier du patient (Base64)
                sauvegarderPdfEnBaseDeDonnees(msg.data, msg.filename);
                break;
                
            // Si le médecin clique sur le bouton "Retour au logiciel"
            case 'risquecv:close':
                console.log("Fermeture demandée par RisqueCV.");
                if (popupWindow) popupWindow.close();
                cleanupSession();
                break;

            // En cas d'erreur métier ou protocolaire
            case 'risquecv:error':
                console.error(`❌ Erreur RisqueCV [${msg.code}]:`, msg.message);
                break;
        }
    };

    window.addEventListener('message', messageListener);
});
```

</details>

---

## 📋 Catalogue des messages

Tous les messages partagent une structure de base : `type`, `version` (fixée à `1`) et `partner`.

### Étape 1 : Le signal de départ
#### 🟢 `risquecv:ready` (RisqueCV ➡️ Votre Logiciel)
Envoyé dès que RisqueCV est prêt à recevoir des données. Ce message contient le `sessionId` requis pour la suite.

```json
{
  "type": "risquecv:ready",
  "version": 1, // Il s'agit de la version du protocole d'intégration RisqueCV
  "partner": "votre-slug", // ex : "weda", "doctolib", "medistory", etc.
  "sessionId": "uuid-genere-par-risquecv", // Identifiant unique de la session
  "capabilities": {
    "prefill": true, // Indique que RisqueCV accepte le pré-remplissage
    "pdfReturn": "base64" // Indique que RisqueCV peut renvoyer le PDF en base64
  }
}
```

#### 🔄 `risquecv:ping` (Votre Logiciel ➡️ RisqueCV)
Permet de solliciter le renvoi du signal `ready`.

```json
{
  "type": "risquecv:ping"
}
```

### Étape 2 : L'injection des données du patient
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

### Étape 3 : La confirmation de réception
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

### Étape 4 : La récupération du résultat en PDF
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
> **Note technique :** La propriété `data` contient la chaîne Base64 brute du PDF (ex: `JVBERi0...`). Elle **ne contient pas** l'en-tête Data URI. Si vous souhaitez générer un lien de téléchargement ou l'afficher, vous devez concaténer la chaîne ainsi en Javascript :
```javascript
const pdfUrl = "data:application/pdf;base64," + msg.data;
```

### Étape 5 : Signal de fermeture
#### 🏁 `risquecv:close` (RisqueCV ➡️ Votre Logiciel)
Envoyé lorsque l'utilisateur clique sur le bouton de retour. Indique que l'hôte doit fermer l'interface d'intégration.

```json
{
  "type": "risquecv:close",
  "version": 1,
  "partner": "votre-slug",
  "sessionId": "L_ID_RECU_DANS_READY"
}
```

---

### Cas particulier : message d'erreur
#### 🛑 `risquecv:error` (RisqueCV ➡️ Votre Logiciel)
Envoyé en cas de rupture du protocole ou d'erreur critique de session.


```json
{
  "type": "risquecv:error",
  "version": 1,
  "partner": "votre-slug",
  "sessionId": "L_ID_RECU_DANS_READY", // Optionnel selon le type d'erreur
  "code": "INVALID_SESSION",
  "message": "La session d integration ne correspond pas a la page ouverte."
}
```

| Code | Signification |
| :--- | :--- |
| `INVALID_MESSAGE_FORMAT` | Le JSON ne respecte pas la structure de base. |
| `UNSUPPORTED_VERSION`| La version du protocole est différente de celle utilisée par le backend de RisqueCV. |
| `UNSUPPORTED_MESSAGE_TYPE`| Le `type` de message n'est pas pris en charge. |
| `INVALID_SESSION` | Le `sessionId` est manquant ou incorrect. |
| `PAYLOAD_NOT_A_FLAT_OBJECT` | Le `payload` n'est pas un objet JSON plat. |
| `VALID_BUT_EMPTY_PAYLOAD` | Aucune donnée clinique valide n'a été trouvée dans le payload (objet vide ou toutes les clés sont inconnues). |
| `INVALID_PARTNER` | Le slug partenaire ne correspond pas à l'URL ouverte. |
| `PDF_GENERATION_FAILED` | La génération du PDF a échoué. |
| `PREFILL_ALREADY_APPLIED` | Un `prefill` a déjà été appliqué pour cette session. |

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