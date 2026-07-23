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

    .page-update-card {
        display: flex;
        align-items: center;
		justify-content: center;
        gap: 12px;
        margin: 0 0 1.25rem;
        padding: 12px 15px;
        color: #1b2b7f;
        background: linear-gradient(135deg, #eef3ff 0%, #f8faff 100%);
        border: 1px solid #cbd8f5;
        border-radius: 10px;
        box-shadow: 0 4px 14px rgba(27, 43, 127, 0.08);
    }

    .page-update-card svg {
        width: 22px;
        height: 22px;
        flex: 0 0 auto;
    }

    .page-update-card-content {
        display: flex;
        flex-wrap: wrap;
        align-items: baseline;
        gap: 4px 8px;
    }

    .page-update-card-label { font-weight: 700; }

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
        height: 43px;
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

<div class="page-update-card" aria-label="Date de dernière mise à jour de cette documentation">
  <svg aria-hidden="true" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round">
    <path d="M7 3v3M17 3v3M4 9h16M5 5h14a1 1 0 0 1 1 1v13a1 1 0 0 1-1 1H5a1 1 0 0 1-1-1V6a1 1 0 0 1 1-1Z"/>
    <path d="m9 15 2 2 4-4"/>
  </svg>
  <div class="page-update-card-content">
    <span class="page-update-card-label">Dernière mise à jour de cette documentation :</span>
    <time datetime="{{ site.time | date_to_xmlschema }}">{{ site.time | date: "%d/%m/%Y" }}</time>
  </div>
</div>

Cette page décrit le **protocole de communication bidirectionnel** entre RisqueCV et ses partenaires.

RisqueCV.fr est un outil d'aide à la décision pour la prévention cardiovasculaire. Il permet d'**évaluer le risque cardiovasculaire d'un patient** et de **générer un rapport PDF**.

100% des calculs sont effectués côté client (Typescript), **aucun envoi de données ni aucun calcul vers le serveur de RisqueCV.fr.** 

L'absence de serveur de calcul est **un choix délibéré pour garantir la confidentialité des données des patients.** Cette architecture rend impossible la mise à disposition d'une API REST ou SMART on FHIR.

L'intégration de RisqueCV.fr à un logiciel métier repose donc sur l'API Standard `window.postMessage`, permettant un **échange sécurisé** des données cliniques. Ce protocole permet l'ouverture de RisqueCV.fr, le transfert de données cliniques du logiciel métier vers la fenêtre de RisqueCV.fr (sans transfert des données sur internet), la génération du PDF des résultats en local (librairie JS) et l'envoi du rapport PDF de RisqueCV.fr vers le logiciel métier sans transfert des données sur internet.

La méthode `window.postMessage` permet au médecin en consultation de préremplir les données cliniques et d'utiliser l'interface de RisqueCV.fr (courbes, graphiques, conseils, etc.) comme un outil d'**aide à la décision**.

<div class="sandbox-test-container">
    <button id="sandbox-trigger" class="bouton-sandbox bouton-sandbox--red">
        <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 1024 1024" style="fill: currentColor;"><path d="M960 704a64 64 0 0 0-64 64v64a64 64 0 0 1-64 64H192a64 64 0 0 1-64-64V192a64 64 0 0 1 64-64h64a64 64 0 0 0 0-128h-64C85.96 0 0 85.96 0 192v640c0 106.04 85.96 192 192 192h640c106.04 0 192-85.96 192-192v-64a64 64 0 0 0-64-64"/><path d="M1023.88 51.52c0-1.92 0-3.84-1.6-5.44a64 64 0 0 0-1.92-6.4 64 64 0 0 0-3.2-6.4s0-3.2-2.56-4.8a64 64 0 0 0-17.6-17.6L991.88 8l-6.08-3.2-6.72-1.92h-5.44A64 64 0 0 0 959.88 0h-384a64 64 0 0 0 0 128h229.44L434.76 498.88a64.04 64.04 0 0 0 90.56 90.56l370.56-370.88V448a64 64 0 0 0 128 0V64q.6-6.24 0-12.48"/></svg>
        <span>Tester l'interface d'intégration</span>
    </button>
    <button id="sandbox-pdf" class="bouton-sandbox bouton-sandbox--lightblue">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 256 256" width="22" height="22" style="fill: currentColor;"><path d="M152 32v56h56.008z" opacity=".2"></path><path d="M216.008 88a7.97 7.97 0 0 0-2.432-5.738l-55.919-55.918q-.277-.277-.58-.526c-.05-.04-.102-.075-.153-.114a8 8 0 0 0-.477-.353c-.045-.03-.093-.055-.138-.085a8 8 0 0 0-.535-.32q-.05-.024-.103-.049a8 8 0 0 0-.605-.286c-.023-.01-.047-.016-.071-.026a8 8 0 0 0-.664-.238q-.04-.01-.08-.02a8 8 0 0 0-.676-.17c-.066-.013-.133-.019-.199-.03-.19-.034-.382-.067-.577-.087A8 8 0 0 0 152 24H55.992a16.02 16.02 0 0 0-16 16v176a16.02 16.02 0 0 0 16 16H200a16.02 16.02 0 0 0 16-16V88.16c.001-.054.008-.106.008-.16M160 51.314 188.687 80H160ZM200 216H55.992V40H144v48a8 8 0 0 0 8 8h48l.01 120Z"></path><path d="M150.343 150.343 136 164.687V120a8 8 0 0 0-16 0v44.687l-14.343-14.344a8 8 0 0 0-11.314 11.314l28 28c.026.026.055.048.081.074q.242.237.504.455c.097.08.2.15.301.225.109.081.215.165.328.24.116.079.237.146.357.218.105.062.207.128.315.185.12.065.244.12.366.177.114.054.227.111.343.16.119.049.24.088.36.13.126.046.25.095.38.134.12.036.241.063.362.093.132.033.263.07.397.097.14.028.28.044.42.064.119.017.234.04.353.051a8 8 0 0 0 1.58 0c.119-.012.234-.034.353-.05.14-.021.28-.037.42-.065.134-.027.265-.064.397-.097.121-.03.243-.057.362-.093.13-.04.254-.088.38-.133.12-.043.241-.082.36-.131.116-.049.229-.106.343-.16.122-.058.246-.112.366-.177.108-.057.21-.123.315-.185.12-.072.24-.14.357-.217.113-.076.22-.16.328-.241.1-.075.204-.145.301-.225q.266-.221.513-.464c.023-.023.049-.042.072-.065l28-28a8 8 0 0 0-11.314-11.314"></path></svg>
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

    const targetUrl = 'https://risquecv.fr/test-integration';
    const partnerSlug = 'test-integration';
    const skipOnboardingReglagesParam = 'skip_onboarding_reglages';

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

    function buildSandboxUrl(baseUrl) {
        const url = new URL(baseUrl);
        url.searchParams.set(skipOnboardingReglagesParam, '1');
        return url.toString();
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

    btn.addEventListener('click', (event) => {
        // Anti-spam : focus si déjà ouvert
        if (popup && !popup.closed) {
            popup.focus();
            return;
        }

        cleanup();
        logContainer.innerHTML = '';
        pdfPill.style.display = 'none';
        pdfData = null;

        // Si la touche Option (macOS) / Alt est enfoncée, on bascule sur l'environnement local en HTTPS
        const currentTargetUrl = buildSandboxUrl(event.altKey ? 'https://risquecv.local/test-integration' : targetUrl);

        popup = window.open(currentTargetUrl, '_blank');
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
                popup.postMessage(p, new URL(currentTargetUrl).origin);
                log('OUT', p);
            }
        }, 3000);

        messageListener = (e) => {
            let origin;
            try { origin = new URL(currentTargetUrl).origin; } catch(x) { return; }
			if (e.origin !== origin || e.source !== popup) return;

            const m = e.data;
            log('IN', m);

            if (m.type === 'risquecv:ready') {
                clearTimeout(handshakeTimeout);
                status.classList.add('is-active');
                status.querySelector('.text').textContent = 'Connecté';
				const correlationId = crypto.randomUUID(); // Démonstration : en production, le lier côté métier au patient et à la consultation avant l'ouverture.
                
                setTimeout(() => {
					const payload = {
						type: 'risquecv:prefill',
						version: 1,
						partner: partnerSlug,
						sessionId: m.sessionId,
						correlationId,
						options: { pdfAck: true },
						payload: {
                            pays: 'FR', age: 52, sexe: 'homme', 
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
				status.querySelector('.text').textContent = 'PDF ENREGISTRÉ ✅';
				// Démonstration uniquement : le PDF reste en mémoire dans cette page.
				// En production, n'envoyez cet accusé de réception qu'après son enregistrement durable côté serveur.
				const ack = {
					type: 'risquecv:pdf:ack',
					version: 1,
					partner: partnerSlug,
					sessionId: m.sessionId,
					correlationId: m.correlationId,
					pdfId: m.pdfId,
					status: 'ok'
				};
				popup.postMessage(ack, origin);
				log('OUT', ack);
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

## 🎯 Ce que permet RisqueCV.fr

### Utilisation standard

- **Évaluer le risque cardiovasculaire** d'un patient (risque faible, modéré, élevé...) à partir des données cliniques saisies par le médecin (cholestérol, age, diabète...)
- **Visualiser les résultats** dans une interface interactive avec des graphiques pour favoriser une meilleure compréhension du risque par le patient, et aider à la décision médicale partagée
- **Obtenir des conseils sur la prise en charge adaptée** selon le profil du patient (arrêter le tabac, mettre en place un traitement...)
- **Générer un rapport PDF** contenant la synthèse de l'évaluation et des recommandations

### Avec l'intégration dans un logiciel métier

- **Ouvrir RisqueCV.fr facilement** via un bouton dans le logiciel métier dans une WebView
- **Préremplir automatiquement les données cliniques** disponibles dans le dossier patient, pour limiter la ressaisie (ex : valeur de choléstérol, âge, sexe, ...)
- Utiliser les graphiques pour discuter avec le patient de sa santé cardiovasculaire
- **Enregistrer en un clic le PDF final dans le dossier médical** du logiciel métier

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
const boutonOuvrirRisqueCV = document.getElementById('bouton-ouvrir-risquecv');
let handshakeTimeout = null;
const sauvegardesPdf = new Map(); // pdfId -> Promise d'enregistrement, pour garantir l'idempotence
let sessionId = null;
let correlationId = null;
let ouvertureEnCours = false;

// --- 3. FONCTIONS UTILITAIRES ---
function fermerWebView() {
	clearTimeout(handshakeTimeout);
	handshakeTimeout = null;
	webview.style.display = 'none';
	webview.src = 'about:blank';
	sauvegardesPdf.clear();
	sessionId = null;
	correlationId = null;
}

/** Crée le contexte qui rattache l'évaluation en cours sur RisqueCV au patient et à la consultation de votre logiciel. */
async function creerContexteRisqueCV() {
	const nouvelleCorrelationId = crypto.randomUUID();

    // Sauvegarder le contexte en backend (pas uniquement dans le navigateur).
	const response = await fetch('/api/votre-logiciel/risquecv/contextes', {
		method: 'POST',
		headers: {
'Content-Type': 'application/json',
			'X-CSRF-Token': getCsrfToken() // Utilisez le helper de sécurité déjà fourni par votre logiciel.
},
		body: JSON.stringify({ correlationId: nouvelleCorrelationId })
	});

	if (!response.ok) {
		throw new Error(`Échec de la création du contexte côté serveur (HTTP ${response.status}).`);
	}

	return nouvelleCorrelationId;
}

/** Transmet le PDF Base64 à votre API pour l'enregistrer dans le dossier du patient. */
async function sauvegarderPdf(base64Data, filename, pdfId, correlationId) {
	// Ce point d'entrée vérifie l'idempotence et la destination, puis appelle votre API documentaire habituelle.
	// Voir l'exemple d'implémentation REST dans le bloc « Exemple backend REST » ci-dessous.
	const response = await fetch('/api/votre-logiciel/risquecv/pdf', {
		method: 'POST',
		headers: {
'Content-Type': 'application/json',
			'X-CSRF-Token': getCsrfToken()
},
		body: JSON.stringify({
			correlationId, // Le serveur résout le patient et la consultation liés à cette évaluation.
			pdfId, // Clé d'idempotence : un même PDF ne doit être enregistré qu'une fois.
			nom_fichier: filename, // Ex. `RisqueCV_19-05-2026_17h45.pdf`.
			contenu_base64: base64Data,
			type_document: 'EVALUATION_RISQUE_CV'
		})
	});

	if (!response.ok) {
		throw new Error(`Échec de la sauvegarde côté serveur (HTTP ${response.status}).`);
	}

	console.log('✅ PDF sauvegardé avec succès dans le dossier du patient.');
}

// --- 4. DÉCLENCHEMENT DE L'OUVERTURE ---

boutonOuvrirRisqueCV.addEventListener('click', async () => {
// Une seule préparation à la fois : évite qu'une réponse ancienne remplace le contexte patient courant.
	if (ouvertureEnCours) return;
	ouvertureEnCours = true;
	boutonOuvrirRisqueCV.disabled = true;
	// Nettoyage complet avant ouverture.
	fermerWebView();

	try {
		const nouveauCorrelationId = await creerContexteRisqueCV();
	correlationId = nouveauCorrelationId;

	// Charger l'URL d'intégration seulement après la persistance du contexte métier.
	webview.src = `${CONFIG.targetOrigin}/${CONFIG.partnerSlug}/`;
	webview.style.display = 'block';

		// Si RisqueCV ne répond pas, envoyer un ping après 3 secondes.
	// Chaque ping valide relance le délai de handshake côté RisqueCV, mais il faut ensuite envoyer un prefill.
	handshakeTimeout = setTimeout(() => {
		console.warn("⏳ Délai d'attente dépassé : RisqueCV ne répond pas. Tentative de Ping...");
			// L'envoi dépend de votre framework (ici, une WebView HTML5 standard).
		if (webview.contentWindow) {
			webview.contentWindow.postMessage({ type: 'risquecv:ping' }, CONFIG.targetOrigin);
		}
	}, 3000);
} catch (error) {
		console.error('❌ Impossible de préparer le contexte RisqueCV :', error);
	} finally {
		ouvertureEnCours = false;
		boutonOuvrirRisqueCV.disabled = false;
	}
});

// --- 5. GESTION DES MESSAGES ---

// L'écouteur dépend de votre pont natif. window.addEventListener (Electron), window.chrome.webview.addEventListener (WebView2), etc.
window.addEventListener('message', async (event) => {
	// Ignorer tout message ne provenant pas de la fenêtre RisqueCV attendue.
	if (event.origin !== CONFIG.targetOrigin || event.source !== webview.contentWindow) return;

	const msg = event.data;
	// Tous les messages entrants de RisqueCV appartiennent à la version et au partenaire configurés.
	if (msg?.version !== CONFIG.version || msg?.partner !== CONFIG.partnerSlug) return;

	switch (msg?.type) {
		// Si on reçoit "ready", alors on peut envoyer les données du patient.
		case 'risquecv:ready': {
			if (!correlationId || typeof msg.sessionId !== 'string' || msg.sessionId === '') return;

			clearTimeout(handshakeTimeout);
			handshakeTimeout = null;
			sessionId = msg.sessionId;

			const cible = webview.contentWindow;
			if (!cible) return;

			cible.postMessage({
				type: 'risquecv:prefill',
				version: CONFIG.version,
				partner: CONFIG.partnerSlug,
				sessionId,
				correlationId,
				options: { pdfAck: true }, // Facultatif, si absent la valeur par défaut des options est appliquée
				payload: {
					// Les données doivent être formatées avant l'envoi (ex: "femme" et pas "F")
					age: 55,
					sexe: 'femme',
					tabac: false,
					PAS: 142,
					CT: 5.2,
					HDL: 1.3
					// Ajoutez vos autres variables cliniques ici. Le payload n'a pas besoin d'être exhaustif.
				}
			}, CONFIG.targetOrigin);
			break;
		}

		// Si on reçoit "ack", alors RisqueCV a bien reçu les données.
		case 'risquecv:prefill:ack':
			if (msg.sessionId !== sessionId || msg.correlationId !== correlationId) return;
			if (msg.status === 'empty') {
				console.info('Connexion RisqueCV établie sans donnée clinique préremplie.');
			} else if (msg.status === 'partial') {
				console.warn('⚠️ Données ignorées par RisqueCV (hors-bornes ou inconnues) :', msg.ignoredKeys);
			}
			break;

		// Le pdf:ack ne doit être envoyé qu'après l'enregistrement durable dans le dossier du patient.
		case 'risquecv:pdf': {
			// Écarte un éventuel PDF tardif d'une session précédente.
			if (msg.sessionId !== sessionId || msg.correlationId !== correlationId) return;

			const cible = webview.contentWindow;
			let sauvegardePdf = sauvegardesPdf.get(msg.pdfId);
			if (!sauvegardePdf) {
				sauvegardePdf = sauvegarderPdf(msg.data, msg.filename, msg.pdfId, correlationId);
				sauvegardesPdf.set(msg.pdfId, sauvegardePdf);
			}
			try {
				await sauvegardePdf;
				if (!cible || webview.contentWindow !== cible || sessionId !== msg.sessionId || correlationId !== msg.correlationId) return;
				cible.postMessage({
					type: 'risquecv:pdf:ack',
					version: CONFIG.version,
					partner: CONFIG.partnerSlug,
					sessionId,
					correlationId,
					pdfId: msg.pdfId,
					status: 'ok'
				}, CONFIG.targetOrigin);
			} catch (error) {
				sauvegardesPdf.delete(msg.pdfId);
				if (!cible || webview.contentWindow !== cible || sessionId !== msg.sessionId || correlationId !== msg.correlationId) return;
				cible.postMessage({
					type: 'risquecv:pdf:ack',
					version: CONFIG.version,
					partner: CONFIG.partnerSlug,
					sessionId,
					correlationId,
					pdfId: msg.pdfId,
					status: 'error',
					message: error instanceof Error ? error.message : "Le PDF n'a pas pu être enregistré."
				}, CONFIG.targetOrigin);
			}
			break;
		}

		// Si le médecin clique sur le bouton "Retour au logiciel", on masque l'interface.
		case 'risquecv:close':
			if (sessionId && msg.sessionId !== sessionId) return;
			console.log('Fermeture demandée par RisqueCV.');
			fermerWebView();
			break;

		// Si on reçoit "error", il y a eu un problème métier ou protocolaire.
		case 'risquecv:error':
			if (sessionId && msg.sessionId && msg.sessionId !== sessionId) return;
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
    partnerSlug: 'votre-slug', // Identifiant de votre logiciel (ex : "weda")
    targetOrigin: 'https://risquecv.fr' // Origine stricte
};

// --- 2. ÉTAT DE LA SESSION ---
let popupWindow = null;
let messageListener = null;
let pollClosedInterval = null;
let handshakeTimeout = null;
const sauvegardesPdf = new Map(); // pdfId -> Promise d'enregistrement, pour garantir l'idempotence
let sessionId = null;
let correlationId = null;

// --- 3. FONCTIONS UTILITAIRES ---

/** Nettoie les ressources associées à la session popup. */
function cleanupSession() {
    if (messageListener) {
        window.removeEventListener('message', messageListener);
        messageListener = null;
    }
    if (pollClosedInterval) {
        clearInterval(pollClosedInterval);
        pollClosedInterval = null;
    }
        clearTimeout(handshakeTimeout);
        handshakeTimeout = null;
	sauvegardesPdf.clear();
	sessionId = null;
	correlationId = null;
	popupWindow = null;
}

/** Crée le contexte qui rattache l'évaluation en cours sur RisqueCV au patient et à la consultation de votre logiciel. */
async function creerContexteRisqueCV() {
	const nouvelleCorrelationId = crypto.randomUUID();

    // Sauvegarder le contexte en backend (pas uniquement dans le navigateur).
	const response = await fetch('/api/votre-logiciel/risquecv/contextes', {
		method: 'POST',
		headers: {
'Content-Type': 'application/json',
			'X-CSRF-Token': getCsrfToken() // Utilisez le helper de sécurité déjà fourni par votre logiciel.
},
		body: JSON.stringify({ correlationId: nouvelleCorrelationId })
	});

	if (!response.ok) {
		throw new Error(`Échec de la création du contexte côté serveur (HTTP ${response.status}).`);
	}

	return nouvelleCorrelationId;
}

/** Transmet le PDF Base64 à votre API pour l'enregistrer dans le dossier du patient. */
async function sauvegarderPdf(base64Data, filename, pdfId, correlationId) {
	// Ce point d'entrée vérifie l'idempotence et la destination, puis appelle votre API documentaire habituelle.
	// Voir l'exemple d'implémentation REST dans le bloc « Exemple backend REST » ci-dessous.
	const response = await fetch('/api/votre-logiciel/risquecv/pdf', {
		method: 'POST',
		headers: {
'Content-Type': 'application/json',
			'X-CSRF-Token': getCsrfToken()
},
		body: JSON.stringify({
			correlationId, // Le serveur résout le patient et la consultation liés à cette évaluation.
			pdfId, // Clé d'idempotence : un même PDF ne doit être enregistré qu'une fois.
			nom_fichier: filename, // Ex. `RisqueCV_19-05-2026_17h45.pdf`.
			contenu_base64: base64Data,
			type_document: 'EVALUATION_RISQUE_CV'
		})
	});

	if (!response.ok) {
		throw new Error(`Échec de la sauvegarde côté serveur (HTTP ${response.status}).`);
	}

	console.log('✅ PDF sauvegardé avec succès dans le dossier du patient.');
}

// --- 4. DÉCLENCHEMENT DE L'OUVERTURE ---
document.getElementById('bouton-ouvrir-risquecv').addEventListener('click', async () => {
	// Si la popup est déjà ouverte, la ramener au premier plan sans recharger la session.
	if (popupWindow && !popupWindow.closed) {
		popupWindow.focus();
		return;
	}

	// Nettoyage complet avant ouverture.
	cleanupSession();

	// Ouvrir une fenêtre vide pendant le geste utilisateur évite le blocage des pop-ups pendant l'appel asynchrone qui prépare le contexte côté serveur.
	const popup = window.open('about:blank', '_blank');
	if (!popup) {
		alert('Ouverture bloquée. Veuillez autoriser les pop-ups pour utiliser RisqueCV.');
		return;
	}
popupWindow = popup;

	try {
		const nouveauCorrelationId = await creerContexteRisqueCV();
// La popup a pu être fermée puis remplacée pendant l'appel backend : ignorer cette ancienne tentative.
		if (popupWindow !== popup || popup.closed) {
			if (popupWindow === popup) cleanupSession();
			return;
		}
		correlationId = nouveauCorrelationId;
	} catch (error) {
		console.error('❌ Impossible de préparer le contexte RisqueCV :', error);
// Ne jamais fermer une nouvelle popup ouverte pendant que cette ancienne requête échouait.
		if (popupWindow === popup) {
			popup.close();
		cleanupSession();
			}
		return;
	}

	// --- 5. GESTION DES MESSAGES ---
	messageListener = async (event) => {
		// Ignorer tout message ne provenant pas de la fenêtre RisqueCV attendue.
		if (event.origin !== CONFIG.targetOrigin || event.source !== popup) return;

		const msg = event.data;
		// Tous les messages entrants de RisqueCV appartiennent à la version et au partenaire configurés.
		if (msg?.version !== CONFIG.version || msg?.partner !== CONFIG.partnerSlug) return;

		switch (msg?.type) {
			// Si on reçoit "ready", alors on peut envoyer les données du patient.
			case 'risquecv:ready': {
				if (!correlationId || typeof msg.sessionId !== 'string' || msg.sessionId === '') return;

				clearTimeout(handshakeTimeout);
				handshakeTimeout = null;
				sessionId = msg.sessionId;

				popup.postMessage({
					type: 'risquecv:prefill',
					version: CONFIG.version,
					partner: CONFIG.partnerSlug,
					sessionId,
					correlationId,
					options: { pdfAck: true }, // Facultatif, si absent la valeur par défaut des options est appliquée
					payload: {
						// Les données doivent être formatées avant l'envoi (ex: "femme" et pas "F")
						age: 55,
						sexe: 'femme',
						tabac: false,
						PAS: 142,
						CT: 5.2,
						HDL: 1.3
						// Ajoutez vos autres variables cliniques ici. Le payload n'a pas besoin d'être exhaustif.
					}
				}, CONFIG.targetOrigin);
				break;
			}

			// Si on reçoit "ack", alors RisqueCV a bien reçu les données.
			case 'risquecv:prefill:ack':
				if (msg.sessionId !== sessionId || msg.correlationId !== correlationId) return;
				if (msg.status === 'empty') {
					console.info('Connexion RisqueCV établie sans donnée clinique préremplie.');
				} else if (msg.status === 'partial') {
					console.warn('⚠️ Données ignorées par RisqueCV (hors-bornes ou inconnues) :', msg.ignoredKeys);
				}
				break;

			// Le pdf:ack ne doit être envoyé qu'après l'enregistrement durable dans le dossier du patient.
			case 'risquecv:pdf': {
				// Écarte un éventuel PDF tardif d'une session précédente.
				if (msg.sessionId !== sessionId || msg.correlationId !== correlationId) return;

				let sauvegardePdf = sauvegardesPdf.get(msg.pdfId);
				if (!sauvegardePdf) {
					sauvegardePdf = sauvegarderPdf(msg.data, msg.filename, msg.pdfId, correlationId);
					sauvegardesPdf.set(msg.pdfId, sauvegardePdf);
				}
				try {
					await sauvegardePdf;
					if (popup.closed || sessionId !== msg.sessionId || correlationId !== msg.correlationId) return;
					popup.postMessage({
						type: 'risquecv:pdf:ack',
						version: CONFIG.version,
						partner: CONFIG.partnerSlug,
						sessionId,
						correlationId,
						pdfId: msg.pdfId,
						status: 'ok'
					}, CONFIG.targetOrigin);
				} catch (error) {
					sauvegardesPdf.delete(msg.pdfId);
					if (popup.closed || sessionId !== msg.sessionId || correlationId !== msg.correlationId) return;
					popup.postMessage({
						type: 'risquecv:pdf:ack',
						version: CONFIG.version,
						partner: CONFIG.partnerSlug,
						sessionId,
						correlationId,
						pdfId: msg.pdfId,
						status: 'error',
						message: error instanceof Error ? error.message : "Le PDF n'a pas pu être enregistré."
					}, CONFIG.targetOrigin);
				}
				break;
			}

			// Si le médecin clique sur le bouton "Retour au logiciel", on ferme la popup.
			case 'risquecv:close':
				if (sessionId && msg.sessionId !== sessionId) return;
				console.log('Fermeture demandée par RisqueCV.');
				popup.close();
				cleanupSession();
				break;

			// Si on reçoit "error", il y a eu un problème métier ou protocolaire.
			case 'risquecv:error':
				if (sessionId && msg.sessionId && msg.sessionId !== sessionId) return;
				console.error(`❌ Erreur RisqueCV [${msg.code}]:`, msg.message);
				break;
		}
	};

	window.addEventListener('message', messageListener);

	// Détecter la fermeture manuelle de la popup.
	pollClosedInterval = setInterval(() => {
		if (popup.closed) {
			console.info("ℹ️ Session RisqueCV terminée (fenêtre fermée par l'utilisateur).");
			cleanupSession();
		}
	}, 1000);

	// Si RisqueCV ne répond pas, envoyer un ping après 3 secondes.
	// Chaque ping valide relance le délai de handshake côté RisqueCV, mais il faut ensuite envoyer un prefill.
	handshakeTimeout = setTimeout(() => {
		console.warn("⏳ Délai d'attente dépassé : RisqueCV ne répond pas. Tentative de Ping...");
		if (popupWindow === popup && !popup.closed) {
			popup.postMessage({ type: 'risquecv:ping' }, CONFIG.targetOrigin);
		}
	}, 3000);

	// Charger l'URL d'intégration seulement après la persistance du contexte métier.
	popup.location.href = `${CONFIG.targetOrigin}/${CONFIG.partnerSlug}/`;
});
```

</details>

<details class="code-spoiler" markdown="1">
<summary>🖥️ Exemple backend REST</summary>

Les noms de routes, de middlewares et de services ci-dessous sont illustratifs. Le point important est de laisser les identifiants propres à RisqueCV (`correlationId`, `pdfId`) dans cette couche d'intégration, puis d'appeler votre API existante pour enregistrer le document dans le bon dossier patient.

```typescript
const MAX_PDF_BYTES = 5 * 1024 * 1024; // 5 Mo (pour info, un PDF de RisqueCV fait habituellement environ 40 Ko)
const MAX_BASE64_CHARACTERS = Math.ceil(MAX_PDF_BYTES / 3) * 4;

// À adapter à votre framework. Ces contrôles s'appliquent aux deux routes d'intégration.
const securiteRoutesRisqueCV = [
	authentifierUtilisateur,
	autoriserFonctionnaliteRisqueCV,
	verifierJetonCsrf,
	limiterRequetes({ fenetreMs: 60_000, maximum: 20 }),
	express.json({ limit: '8mb' }) // Limite HTTP, suffisante pour un PDF Base64 de 5 Mo et son enveloppe JSON.
];

/** Décode un PDF Base64 strictement borné et vérifie sa signature minimale. */
function decoderPdfBase64(valeur: unknown): Buffer | null {
	if (typeof valeur !== 'string' || valeur.length === 0 || valeur.length > MAX_BASE64_CHARACTERS) return null;
	if (valeur.length % 4 !== 0 || !/^[A-Za-z0-9+/]+={0,2}$/.test(valeur)) return null;

	const contenu = Buffer.from(valeur, 'base64');
	if (contenu.length === 0 || contenu.length > MAX_PDF_BYTES) return null;
	if (contenu.subarray(0, 5).toString('ascii') !== '%PDF-') return null;
	return contenu;
}

/** Ignore tout chemin fourni par le navigateur et produit un nom PDF court et sûr. */
function normaliserNomPdf(valeur: unknown): string {
	const nomBrut = typeof valeur === 'string' ? (valeur.split(/[\\/]/).at(-1) ?? '') : '';
	const base = nomBrut
		.normalize('NFKC')
		.replace(/\.pdf$/i, '')
		.replace(/[^\p{L}\p{N}._ -]/gu, '_')
		.replace(/\s+/g, ' ')
		.trim()
		.slice(0, 100);
	return `${base || 'RisqueCV'}.pdf`;
}

// Endpoint pour enregistrer un contexte RisqueCV (lien entre une évaluation RisqueCV, et un patient/consultation/utilisateur de votre logiciel)
app.post('/api/votre-logiciel/risquecv/contextes', ...securiteRoutesRisqueCV, async (request, response) => {
	const { correlationId } = request.body as { correlationId?: unknown };

	// L'UUID que vous aviez généré ne contient aucune donnée patient.
	if (!isUuidV4(correlationId)) {
		return response.status(400).json({ message: 'correlationId invalide.' });
	}

	// Ces informations proviennent du contexte métier authentifié de votre application (session serveur, jeton, dossier actuellement ouvert côté backend, etc.)
	const contexteMetier = request.contexteMetier;
	if (!contexteMetier?.patientId || !contexteMetier.consultationId || !request.user) {
		return response.status(409).json({ message: 'Aucun contexte patient actif.' });
	}
	if (!await autorisations.peutAjouterDocument(request.user, contexteMetier.patientId, contexteMetier.consultationId)) {
		return response.status(403).json({ message: 'Accès au dossier patient refusé.' });
	}

	// Stockage temporaire : expirez le contexte après un délai adapté à votre usage.
	await risqueCvContexts.insert({
		correlationId, // L'UUID anonyme que vous avez généré et transmis à la fenêtre RisqueCV.
		patientId: contexteMetier.patientId, // Identifiant du patient dans votre logiciel
		consultationId: contexteMetier.consultationId, // Identifiant de la consultation dans votre logiciel
		userId: request.user.id, // Identifiant de l'utilisateur dans votre logiciel
		expiresAt: addMinutes(new Date(), 30) // Le contexte expire après 30 minutes
	});

	return response.sendStatus(204);
});

// ------------------------------------
// Endpoint pour enregistrer un PDF reçu de RisqueCV dans le dossier patient de manière fiable
type RisqueCvPdfInput = {
	correlationId: string;
	pdfId: string;
	nom_fichier: string;
	contenu_base64: string;
	type_document: 'EVALUATION_RISQUE_CV';
};

app.post('/api/votre-logiciel/risquecv/pdf', ...securiteRoutesRisqueCV, async (request, response) => {
	const pdf = request.body as Partial<RisqueCvPdfInput>;

	if (
		!isUuidV4(pdf.correlationId)
		|| typeof pdf.pdfId !== 'string'
		|| pdf.pdfId.trim() === ''
		|| pdf.pdfId.length > 128
		|| typeof pdf.nom_fichier !== 'string'
		|| pdf.type_document !== 'EVALUATION_RISQUE_CV'
	) {
		return response.status(400).json({ message: 'PDF RisqueCV incomplet.' });
	}

	// Le contexte fait autorité : le navigateur ne fournit jamais de patientId à cette route (risque d'enregistrement du PDF dans le mauvais dossier patient !!!)
	const contexte = await risqueCvContexts.find(pdf.correlationId);
	if (!contexte || contexte.expiresAt < new Date() || contexte.userId !== request.user?.id) {
		return response.status(404).json({ message: 'Contexte RisqueCV introuvable ou expiré.' });
	}
	if (!request.user || !await autorisations.peutAjouterDocument(request.user, contexte.patientId, contexte.consultationId)) {
		return response.status(403).json({ message: 'Accès au dossier patient refusé.' });
	}

	const contenuPdf = decoderPdfBase64(pdf.contenu_base64);
	if (!contenuPdf) {
		return response.status(400).json({ message: 'PDF invalide ou trop volumineux.' });
	}

	try {
		// Cette clé doit être UNIQUE au niveau du document, ou transmise comme clé d'idempotence
		// à votre service documentaire. L'opération crée le document ou retourne l'existant atomiquement.
		const resultat = await documents.createIdempotent({
			idempotencyKey: `risquecv:${pdf.correlationId}:${pdf.pdfId}`,
			patientId: contexte.patientId,
			consultationId: contexte.consultationId,
			filename: normaliserNomPdf(pdf.nom_fichier),
			data: contenuPdf,
			type: pdf.type_document
		});

		// Un retry après perte de la réponse HTTP renvoie 204 et ne crée jamais un second document.
		return response.sendStatus(resultat.created ? 201 : 204);
	} catch (error) {
		request.log?.error({ error }, 'Échec de l’enregistrement du PDF RisqueCV');
		return response.status(500).json({ message: "Le PDF n'a pas pu être enregistré." });
	}
});
```

</details>

---

## 🏗 Description de l'architecture du protocole

L'intégration repose sur un protocole d'échange de messages asynchrones via `window.postMessage` :

### 1. Ouverture
RisqueCV est conçu pour être ouvert depuis votre application via :

- **WebView (recommandé)** : RisqueCV détecte automatiquement son parent (`window.parent`) pour initier le dialogue.
- **Fenêtre popup nouvel onglet (recommandé)** : `window.open('https://risquecv.fr/slug-partenaire/', '_blank')`. Cela permet une communication bilatérale fluide via la référence `window.opener`.
- **Iframe** : compatible mais non recommandé pour des raisons d'UI/UX

<details markdown="1">
<summary>Détails pour l'implémentation via iframe</summary>

1. Pour que votre logiciel puisse intégrer RisqueCV dans une iframe, le serveur de RisqueCV doit vous y autoriser (`Content-Security-Policy: frame-ancestors`). Si vous constatez une erreur "Clickjacking" ou "Refused to frame", demandez à ce que votre domaine soit bien whitelisté dans nos entêtes.
2. Si vous décidez d'utiliser une iframe avec l'attribut `sandbox="..."`, vous devez impérativement configurer les valeurs suivantes :
   - `allow-scripts` : indispensable pour autoriser le fonctionnement de RisqueCV (tous les calculs cliniques et graphiques s'exécutent côté client en Javascript).
   - `allow-same-origin` : indispensable pour que la communication `postMessage` et la validation d'origine fonctionnent. Sans ce paramètre, l'origine de l'iframe sera traitée comme `null` (unique origin) par le navigateur, ce qui empêchera RisqueCV de valider l'origine de vos messages et vice-versa.
   - `allow-popups` : indispensable pour permettre l'ouverture des PDF générés et des liens externes.

**Exemple :**
```html
<iframe src="https://risquecv.fr/doctolib/" sandbox="allow-scripts allow-same-origin allow-popups"></iframe>
```

</details>

### 2. Établissement de la connexion ("handshake")

Le protocole suit une machine à états stricte pour garantir la sécurité des données :

1.  **Phase d'ouverture de RisqueCV** : Dès l'ouverture, votre application doit se mettre à l'écoute de l'événement `message` global.
2.  **Signal "ready" (RisqueCV vers Partenaire)** : Une fois chargé, le site RisqueCV émet un message `risquecv:ready` pour vous informer que le tunnel de communication est ouvert et vous transmettre un `sessionId` unique qu'il faudra utiliser pour tous les messages suivants. RisqueCV ne connaît pas encore le patient à cette étape : ce message ne contient pas de `correlationId`.
    - *Signal ping (Partenaire vers RisqueCV)* : Si votre application a manqué le signal initial, vous pouvez envoyer un message `risquecv:ping`. RisqueCV vous renverra le message `risquecv:ready`.
3.  **Injection "prefill" (Partenaire vers RisqueCV)** : En réponse au `risquecv:ready`, vous envoyez les données patient (age, sexe, cholestérol...) et un `correlationId` UUID v4 via un message `risquecv:prefill` (format détaillé plus bas). Avant l'ouverture, votre logiciel doit créer puis persister côté serveur l'association entre cet identifiant, le patient interne, la consultation interne et l'utilisateur connecté.
	- *Verrouillage de session (channel locking)* : Dès la réception de votre premier `risquecv:prefill` structurellement valide, RisqueCV **verrouille le canal** sur votre origine et votre fenêtre. Dès le premier `prefill` accepté (y compris un payload vide `{}`), il fige aussi le `correlationId`. Pour le reste de la session, RisqueCV n'acceptera plus aucun message provenant d'une autre origine ou d'une autre fenêtre que la vôtre, ni aucun message signé avec un autre `sessionId` ou un autre `correlationId`.
    - *Délai de repli (handshake timeout)* : Si RisqueCV ne reçoit **aucun trafic valide** (ni ping, ni prefill) dans les **5 secondes** suivant son ouverture, il bascule automatiquement en **mode standard** (non lié au logiciel métier). Un `risquecv:ping` valide relance ce délai et renvoie le message `risquecv:ready` (avec le même `sessionId`); il doit ensuite être suivi d'un `risquecv:prefill`. Cela évite de bloquer le médecin si votre logiciel métier subit un bug technique.
	- *Connexion sans donnée clinique* : si votre logiciel n'a aucune donnée fiable à préremplir mais souhaite tout de même récupérer le PDF final, envoyez un `risquecv:prefill` avec `payload: {}`. RisqueCV répondra par un ACK `status: "empty"` et activera le canal de retour PDF.

### 3. Traitement des données
L'algorithme de RisqueCV assure l'intégrité, la validation et la normalisation des données reçues :

- **Validation des données entrantes** : Les clés inconnues ou les valeurs mal formatées sont ignorées.
- **Validation des bornes** : Si vous envoyez une valeur numérique cliniquement aberrante (ex: age = 300), le champ est ignoré pour protéger la cohérence médicale.
- **Cohérence inter-champs** : Si l'injection crée une impossibilité logique (ex: vous envoyez un âge de diagnostic du diabète supérieur à l'âge actuel du patient), les valeurs incohérentes sont rejetées.
- **Accusé de réception (`ack`)** : RisqueCV vous renvoie un message `risquecv:prefill:ack` (acknowledgement) quand le `prefill` est accepté (au moins une donnée clinique valide, ou payload vide `{}`). Les payloads non plats, trop volumineux, ou non vides mais sans aucune donnée clinique exploitable renvoient un message `risquecv:error`.
- **Mise à jour instantanée** : L'injection des données dans l'interface de RisqueCV est immédiate. Tous les scores et graphiques se mettent à jour dès réception de votre `prefill`.

### 4. UI adaptée au partenaire
- Bouton "Retour au Logiciel" (texte personnalisable, ex "Retour à Doctolib")
- Bouton PDF "Envoyer vers Logiciel" (texte personnalisable, ex "Envoyer vers Doctolib")
- Le reste de l'application est strictement identique à la version publique.

### 5. Récupération du rapport PDF
Lorsque le médecin a terminé son évaluation sur RisqueCV, il clique sur "Envoyer vers logiciel" (ou sur "Retour vers logiciel")
1. RisqueCV génère un rapport PDF (localement dans le navigateur via la librairie `pdfmake`, aucune donnée n'est envoyée à nos serveurs).
2. Il vous transmet le PDF encodé en **Base64** via un message `risquecv:pdf`, avec un `pdfId` opaque permettant de corréler l'envoi et son accusé de réception, ainsi que le `correlationId` du contexte initial.
3. Votre serveur résout le `correlationId` dans l'association métier persistée à l'ouverture, vérifie les droits de l'utilisateur puis enregistre le document dans ce patient et cette consultation précis. Il ne doit jamais utiliser le dossier actuellement affiché par le médecin, ni faire confiance à un identifiant de patient fourni par le navigateur. Il traite également `pdfId` comme clé d'idempotence.
4. Lorsque l'enregistrement du PDF dans le dossier patient est terminé, votre logiciel envoie un message `risquecv:pdf:ack` à RisqueCV pour l'informer que le PDF a été enregistré avec succès.

> **Note sur le bouton "Retour vers logiciel"** : Si le médecin clique sur le bouton de retour alors qu'une évaluation est disponible mais que le PDF n'a pas encore été transmis, une modale de confirmation s'affiche dans RisqueCV. Elle lui propose d'envoyer le PDF et quitter, de quitter sans envoyer le PDF, ou de rester sur l'interface. S'il choisit de quitter (avec ou sans envoi), le signal de fermeture `risquecv:close` est émis.

### 6. Fermeture de session
Lors du clic sur le bouton de retour, RisqueCV émet un signal `risquecv:close`.

> #### Prévention de l'inception des iframes
> Rediriger une Iframe vers une URL externe peut provoquer le chargement de votre propre portail à l'intérieur de l'Iframe
> - **Dans une Iframe** : RisqueCV émet le message `risquecv:close` et **reste sur sa page**. C'est à votre application de capter ce message pour détruire l'Iframe (pour éviter l'inception)
> - **Dans un Nouvel onglet / Popup** : RisqueCV émet le message, tente de s'auto-fermer (`window.close()`), et n'utilise sa redirection de secours (`returnUrl`) qu'en tout dernier recours.

---

## 🔒 Sécurité et confidentialité

Ce protocole a été conçu pour répondre aux exigences les plus strictes de confidentialité (RGPD / HDS) :

- **Zéro transit Internet** : Les données patient circulent exclusivement dans la mémoire vive de l'ordinateur du médecin, entre votre fenêtre et celle de RisqueCV.
- **Zéro persistance** : RisqueCV n'enregistre absolument rien concernant les données cliniques injectées ou calculées (ni base de données, ni cookies). Une fois la fenêtre fermée, les données cliniques sont définitivement purgées.
- **Isolation des origines** : RisqueCV rejette tout message dont l'`event.origin` ne correspond pas strictement à un liste blanche de partenaires.
- **Pas de cookies** : RisqueCV n'utilise aucun cookie.
- **Pas de publicité** : RisqueCV n'affiche aucune publicité.
- **Contexte métier opaque** : Le `correlationId` est un UUID v4 aléatoire, créé par votre logiciel et lié côté serveur au patient, à la consultation et à l'utilisateur. Il ne contient aucune donnée de santé et n'est jamais dérivé d'un nom, prénom, numéro de sécurité sociale ou autre identifiant patient.

---


## 📖 Dictionnaire des caractéristiques patient

Le `payload` peut contenir n'importe quelle combinaison des clés ci-dessous. **Toutes les valeurs sont optionnelles** : omettez une clé pour ne pas la transmettre. Toute clé inconnue sera ignorée.

Utiliser de préférence le **typage JSON natif** : nombres pour les nombres, booléens pour les booléens.

<details markdown="1">
<summary>Plus d'information sur les formats attendus</summary>

Le format recommandé est d'envoyer les **clés** et les **types JSON natifs** tels que documentés ci-dessous. 
<br>
Cependant, pour faciliter l'intégration avec les logiciels métier, RisqueCV tolère certaines erreurs de format : 

- les nombres peuvent être envoyés sous forme de string (ex : `"130"`, `"130.5"` ou `"130,5"`). 
- Les champs déclarés comme entiers sont d'abord contrôlés sur leurs bornes, puis arrondis à l'entier le plus proche.
- les booléens peuvent être envoyés sous forme native (`true`, `false`), sous forme de chaînes (`"true"`, `"false"`, `"1"`, `"0"`) ou sous forme numérique (`1`, `0`)
- les valeurs `null` sont traitées comme des valeurs ignorées et signalées dans `ignoredKeys`. Si vous voulez établir la session sans préremplir de donnée clinique, envoyez plutôt un payload vide `{}`.
- les unités ne sont jamais converties automatiquement : une valeur comme `"2 g/L"`, `"130 mmHg"` ou `"48 mmol/mol"` est ignorée pour des raisons de sécurité clinique.

Utiliser de préférence les **clés canoniques** documentées ci-dessous (ex: `PAS`, `HbA1c`, `age`). Les variations de casse (ex : `pas`, `hba1c`) sont tolérées mais non recommandées.
- les clés sont comparées sans tenir compte de la casse, puis rattachées à leur clé canonique (ex : `pas`, `PAS` ou `Pas` sont traités comme `PAS`, `hba1c` comme `HbA1c`, `mrc` comme `MRC`) 
- En cas de présence de plusieurs clés pointant vers la même donnée, seule la clé canonique exacte est traitée. 
    - Par exemple, si `PAS` et `pas` sont envoyées ensemble, seule `PAS` sera traitée, tandis que `pas` sera signalée dans `ignoredKeys`. 
    - Si plusieurs variantes non canoniques pointent vers la même donnée sans clé canonique exacte (ex : `Pas` et `pas` sans `PAS`), elles sont **toutes** ignorées et signalées dans `ignoredKeys`.

</details>

### ⚠️ ATTENTION, ERREURS FREQUENTES :
<div class="warning">
- <span style="font-weight: bold;">Respecter les unités mentionnées</span>. Soyez particulièrement vigilants sur le cholestérol (<code class="language-plaintext">CT</code>, <code class="language-plaintext">HDL</code>, <code class="language-plaintext">LDL</code>) qui doit impérativement être envoyé en <code class="language-plaintext">mmol/L</code> (et non en g/L), ainsi que sur l'<code class="language-plaintext">HbA1c</code> qui doit être envoyée en <code class="language-plaintext">%</code> (et non en mmol/mol).<br>
- <span style="font-weight: bold;">Ne pas envoyer de données nominatives</span> (même si elles seront ignorées et non traitées).<br>
- <span style="font-weight: bold;">Privilégier les données les plus récentes</span>. L'évaluation du risque cardiovasculaire n'est pertinente qu'avec des données à jour. Une vérification de la date des données doit notamment être mise en place pour la <code class="language-plaintext">PAS</code>, le <code class="language-plaintext">CT</code>, <code class="language-plaintext">HDL</code>, <code class="language-plaintext">LDL</code>, le <code class="language-plaintext">DFG</code>, la <code class="language-plaintext">hs-CRP</code> et l'<code class="language-plaintext">HbA1c</code>. En cas de doute sur la fraîcheur d'une donnée, il est préférable de ne pas l'envoyer : le médecin pourra la saisir manuellement.<br>
</div>

### 1. Les 4 premières questions systématiques de RisqueCV.fr
Ces booléens pilotent les 4 premières questions du formulaire.
Les mettre à `false` permet de sauter les questions de tri initiales.

| Clé | Type | Description | True si... |
| :--- | :--- | :--- | :--- |
| `atcd` | `boolean` | Antécédents de maladie cardiovasculaire avérée. | Maladie coronaire (angor, infarctus du myocarde, syndrome coronarien aigu, stent ou pontage coronarien), AVC, AIT, AOMI, anévrisme de l'aorte abdominale (voir la liste complète sur le site, sous le titre "Antécédents cardiovasculaires") |
| `diabete` | `boolean` | Présence d'un diabète (Type 1 ou 2). | Diabète (peu importe le type et le traitement) |
| `MRC` | `boolean` | Maladie Rénale Chronique (DFG < 60 ou albuminurie). | DFG < 60 ou albuminurie ou "Maladie rénale chronique" |
| `autrepb` | `boolean` | Autres situations complexes ou particulières qui nécessitent une évaluation personnalisée. | Hypercholestérolémie familiale hétérozygote, grossesse, etc. (voir la liste complète sur le site, sous le titre "Autre situation particulière ?") |

### 2. Valeurs numériques

| Clé | Type | Unité | Format | Description |
| :--- | :--- | :--- | :--- | :--- |
| `age` | `number` | ans | Entier | Âge du patient |
| `PAS` | `number` | mmHg | Entier | Pression Artérielle Systolique (mesure du jour ; max conseillé 6-12 mois) |
| `CT` | `number` | mmol/L | Décimal | Cholestérol Total (idéalement < 3 mois ; max conseillé 12-24 mois) |
| `HDL` | `number` | mmol/L | Décimal | Cholestérol HDL (idéalement < 3 mois ; max conseillé 12-24 mois) |
| `LDL` | `number` | mmol/L | Décimal | Cholestérol LDL (idéalement < 3 mois ; max conseillé 12-24 mois) |
| `DFG` | `number` | mL/min/1.73m² | Décimal | Débit de Filtration Glomérulaire (idéalement < 3 mois ; max conseillé 12-24 mois) |
| `HbA1c` | `number` | % | Décimal | Hémoglobine glyquée (idéalement < 3 mois ; max conseillé 6-12 mois) |
| `crp` | `number` | mg/L | Décimal | Protéine C-réactive ultra-sensible (de préférence hs-CRP, pas la CRP standard). |
| `imc` | `number` | kg/m² | Décimal | Indice de Masse Corporelle |
| `agediabete` | `number` | ans | Entier | Âge lors du diagnostic du diabète |
| `age_atcd` | `number` | ans | Entier | Âge lors du premier événement cardiovasculaire (AVC, AIT, SCA, IDM, AOMI, anévrisme de l'aorte abdominale) |

### 3. Valeurs de type string

| Clé | Type | Valeurs autorisées (exemples) |
| :--- | :--- | :--- |
| `sexe` | `string` | `"homme"`, `"femme"` |
| `typediabete` | `string` | `"type1"`, `"type2"`, `"autre"` |
| `albuminurie` | `string` | `"non"`, `"micro"`, `"oui"` |
| `pays` | `string` | • **Recommandé :** code ISO 3166-1 alpha-2 (ex : `"FR"`, `"BE"`, `"US"`) <br> • **Également accepté :** nom naturel en français (ex : `"France"`, `"Belgique"`, `"États-Unis"`) |

<details markdown="1">
<summary>Liste des 200 identifiants pays acceptés dans `pays`</summary>

| ID accepté dans `pays` | Nom français canonique accepté |
| :--- | :--- |
| `AD` | Andorre |
| `AE` | Émirats arabes unis |
| `AF` | Afghanistan |
| `AG` | Antigua-et-Barbuda |
| `AL` | Albanie |
| `AM` | Arménie |
| `AO` | Angola |
| `AR` | Argentine |
| `AT` | Autriche |
| `AU` | Australie |
| `AZ` | Azerbaïdjan |
| `BA` | Bosnie-Herzégovine |
| `BB` | Barbade |
| `BD` | Bangladesh |
| `BE` | Belgique |
| `BF` | Burkina Faso |
| `BG` | Bulgarie |
| `BH` | Bahreïn |
| `BI` | Burundi |
| `BJ` | Bénin |
| `BM` | Bermudes |
| `BN` | Brunei |
| `BO` | Bolivie |
| `BR` | Brésil |
| `BS` | Bahamas |
| `BT` | Bhoutan |
| `BW` | Botswana |
| `BY` | Biélorussie |
| `BZ` | Belize |
| `CA` | Canada |
| `CD` | Congo-Kinshasa |
| `CF` | République centrafricaine |
| `CG` | Congo-Brazzaville |
| `CH` | Suisse |
| `CI` | Côte d’Ivoire |
| `CL` | Chili |
| `CM` | Cameroun |
| `CN` | Chine |
| `CO` | Colombie |
| `CR` | Costa Rica |
| `CU` | Cuba |
| `CV` | Cap-Vert |
| `CY` | Chypre |
| `CZ` | Tchéquie |
| `DE` | Allemagne |
| `DJ` | Djibouti |
| `DK` | Danemark |
| `DM` | Dominique |
| `DO` | République dominicaine |
| `DZ` | Algérie |
| `EC` | Équateur |
| `EE` | Estonie |
| `EG` | Égypte |
| `EH` | Sahara occidental |
| `ER` | Érythrée |
| `ES` | Espagne |
| `ET` | Éthiopie |
| `FI` | Finlande |
| `FJ` | Fidji |
| `FM` | Micronésie |
| `FR` | France |
| `GA` | Gabon |
| `GB` | Royaume-Uni |
| `GD` | Grenade |
| `GE` | Géorgie |
| `GH` | Ghana |
| `GI` | Gibraltar |
| `GL` | Groenland |
| `GM` | Gambie |
| `GN` | Guinée |
| `GQ` | Guinée équatoriale |
| `GR` | Grèce |
| `GT` | Guatemala |
| `GW` | Guinée-Bissau |
| `GY` | Guyana |
| `HN` | Honduras |
| `HR` | Croatie |
| `HT` | Haïti |
| `HU` | Hongrie |
| `ID` | Indonésie |
| `IE` | Irlande |
| `IL` | Israël |
| `IN` | Inde |
| `IQ` | Irak |
| `IR` | Iran |
| `IS` | Islande |
| `IT` | Italie |
| `JM` | Jamaïque |
| `JO` | Jordanie |
| `JP` | Japon |
| `KE` | Kenya |
| `KG` | Kirghizistan |
| `KH` | Cambodge |
| `KI` | Kiribati |
| `KM` | Comores |
| `KN` | Saint-Christophe-et-Niévès |
| `KP` | Corée du Nord |
| `KR` | Corée du Sud |
| `KW` | Koweït |
| `KY` | Îles Caïmans |
| `KZ` | Kazakhstan |
| `LA` | Laos |
| `LB` | Liban |
| `LC` | Sainte-Lucie |
| `LI` | Liechtenstein |
| `LK` | Sri Lanka |
| `LR` | Liberia |
| `LS` | Lesotho |
| `LT` | Lituanie |
| `LU` | Luxembourg |
| `LV` | Lettonie |
| `LY` | Libye |
| `MA` | Maroc |
| `MC` | Monaco |
| `MD` | Moldavie |
| `ME` | Monténégro |
| `MG` | Madagascar |
| `MH` | Îles Marshall |
| `MK` | Macédoine du Nord |
| `ML` | Mali |
| `MM` | Birmanie |
| `MN` | Mongolie |
| `MR` | Mauritanie |
| `MT` | Malte |
| `MU` | Maurice |
| `MV` | Maldives |
| `MW` | Malawi |
| `MX` | Mexique |
| `MY` | Malaisie |
| `MZ` | Mozambique |
| `NA` | Namibie |
| `NE` | Niger |
| `NG` | Nigeria |
| `NI` | Nicaragua |
| `NL` | Pays-Bas |
| `NO` | Norvège |
| `NP` | Népal |
| `NZ` | Nouvelle-Zélande |
| `OM` | Oman |
| `PA` | Panama |
| `PE` | Pérou |
| `PG` | Papouasie-Nouvelle-Guinée |
| `PH` | Philippines |
| `PK` | Pakistan |
| `PL` | Pologne |
| `PS` | Territoires palestiniens |
| `PT` | Portugal |
| `PY` | Paraguay |
| `QA` | Qatar |
| `RO` | Roumanie |
| `RS` | Serbie |
| `RU` | Russie |
| `RW` | Rwanda |
| `SA` | Arabie saoudite |
| `SB` | Îles Salomon |
| `SC` | Seychelles |
| `SD` | Soudan |
| `SE` | Suède |
| `SG` | Singapour |
| `SI` | Slovénie |
| `SK` | Slovaquie |
| `SL` | Sierra Leone |
| `SM` | Saint-Marin |
| `SN` | Sénégal |
| `SO` | Somalie |
| `SR` | Suriname |
| `SS` | Soudan du Sud |
| `ST` | Sao Tomé-et-Principe |
| `SV` | Salvador |
| `SY` | Syrie |
| `SZ` | Eswatini |
| `TC` | Îles Turques-et-Caïques |
| `TD` | Tchad |
| `TG` | Togo |
| `TH` | Thaïlande |
| `TJ` | Tadjikistan |
| `TL` | Timor oriental |
| `TM` | Turkménistan |
| `TN` | Tunisie |
| `TO` | Tonga |
| `TR` | Turquie |
| `TT` | Trinité-et-Tobago |
| `TW` | Taïwan |
| `TZ` | Tanzanie |
| `UA` | Ukraine |
| `UG` | Ouganda |
| `US` | États-Unis |
| `UY` | Uruguay |
| `UZ` | Ouzbékistan |
| `VC` | Saint-Vincent-et-les Grenadines |
| `VE` | Venezuela |
| `VG` | Îles Vierges britanniques |
| `VN` | Viêt Nam |
| `VU` | Vanuatu |
| `WS` | Samoa |
| `XK` | Kosovo |
| `YE` | Yémen |
| `ZA` | Afrique du Sud |
| `ZM` | Zambie |
| `ZW` | Zimbabwe |

</details>

### 4. Booléens

| Clé | Type | Description |
| :--- | :--- | :--- |
| `tabac` | `boolean` | Tabagisme actif actuel. |
| `antithrombotique` | `boolean` | Traitement actuel : aspirine ou autre antiagrégant plaquettaire ou anticoagulants. |
| `insuline` | `boolean` | Diabète traité par insuline. |
| `hyperCHOfamille`| `boolean` | Hypercholestérolémie familiale hétérozygote connue. |
| `retinopathie` | `boolean` | Présence d'une rétinopathie diabétique. |
| `neuropathie` | `boolean` | Présence d'une neuropathie diabétique. |
| `atcd_coronarien` | `boolean` | Antécédent de maladie coronaire (IDM, SCA, revascularisation). |
| `atcd_cerebrovasculaire`| `boolean` | Antécédent d'AVC ou d'AIT. |
| `atcd_aomi` | `boolean` | Antécédent d'Artériopathie Oblitérante des Membres Inférieurs. |
| `atcd_anevrismeAorte`| `boolean` | Antécédent d'anévrisme de l'aorte abdominale. |
| `atcd_evenement_recurrent` | `boolean` | Nouvel événement cardiovasculaire malgré une statine à dose maximale tolérée. |
| `atcd_evenement_recent` | `boolean` | Événement cardiovasculaire survenu il y a moins de 6 semaines. |
| `atcd_polyvasculaire` | `boolean` | Atteinte polyvasculaire (par exemple coronaire + AOMI). |
| `microangiopathie3sites`| `boolean` | Présence d'une microangiopathie sur ≥3 sites (ex: rétino + neuro + albu). |
| `autreFacteurMajeur` | `boolean` | Présence d'un autre facteur de risque majeur (pour l'HF). |
| `evaluationComplete`| `boolean` | Force l'affichage de l'évaluation complète (tunnel détaillé). |

---

## 📋 Catalogue des messages

Tous les messages de session partagent une structure de base :
- `type`,
- `version` (fixée à `1`),
- `partner`,
- `sessionId`.

Dès qu'un `prefill` est accepté, tous les messages suivants portent aussi :
- `correlationId`.

Le message `risquecv:ping` est volontairement hors session et ne contient que son `type`.

| Champ | Rôle |
| :--- | :--- |
| `type` | Identifie le type de message du protocole et donc son format. Utilisez exclusivement les valeurs documentées dans le catalogue ci-dessous. |
| `version` | Version du protocole d'intégration entre RisqueCV et les logiciels métiers partenaires. Actuellement fixée à `1`. Elle est exigée dans tous les messages de session et toute autre valeur est rejetée. |
| `partner` | Slug de votre logiciel métier. Il doit correspondre exactement au partenaire attendu par RisqueCV (whitelist). |
| `sessionId` | Identifiant opaque généré par RisqueCV lors du `risquecv:ready`. Il identifie une session unique de communication et contribue à sa sécurité avec la validation de l'origine et de la fenêtre `postMessage`. Le partenaire doit le reprendre sans modification dans chaque message suivant, sans dépendre de son format, le générer, le persister ou le réutiliser. |
| `correlationId` | UUID v4 généré par le logiciel métier partenaire au lancement de RisqueCV, puis transmis dans le premier `risquecv:prefill`. Il lie le patient et la consultation ayant lancé le calcul avec le PDF d'évaluation reçu, afin d'éviter un enregistrement dans le dossier du mauvais patient. Générez un UUID v4 neuf (par exemple `crypto.randomUUID()`), puis créez une association temporaire côté serveur `{ correlationId, patientIdInterne, consultationIdInterne, userId }`. Cette association est la source de vérité : ne la conservez pas uniquement dans le navigateur. Elle peut être créée par une action, API, RPC ou IPC existant ; le protocole n'impose aucune route HTTP dédiée. L'identifiant reste identique pendant toute la session. RisqueCV le renvoie tel quel, sans l'interpréter. Ne le générez jamais à partir d'une donnée patient, même hachée : un hash de nom, prénom ou numéro de sécurité sociale expose des données sensibles et ne distingue pas les consultations. À la réception du PDF, résolvez l'identifiant côté serveur, vérifiez les droits puis enregistrez le PDF dans l'association mémorisée, **jamais dans le dossier actuellement affiché dans l'interface**. Conservez ce contexte pendant le transfert et les réessais idempotents (`pdfId`), puis expirez-le ou marquez-le comme traité après un `risquecv:pdf:ack` positif. Si le contexte est introuvable ou devenu inaccessible, répondez `risquecv:pdf:ack` avec `status: "error"`.|
| `pdfId` | Identifiant généré par RisqueCV lors de `risquecv:pdf`. Le serveur du logiciel métier l'utilise comme clé d'idempotence : un même `pdfId` représente le même document, même en cas de réessai, et ne doit donc créer qu'un seul document. RisqueCV l'utilise pour vérifier que l'accusé d'enregistrement `risquecv:pdf:ack` reçu correspond bien au PDF envoyé. |

### Étape 1 : Le signal de départ
#### 🟢 `risquecv:ready` (RisqueCV ➡️ Votre Logiciel)
Envoyé dès que RisqueCV est prêt à recevoir des données.
Ce message contient le `sessionId` requis pour la suite.

```json
{
  "type": "risquecv:ready",
  "version": 1, // Il s'agit de la version du protocole d'intégration RisqueCV
  "partner": "votre-slug", // ex : "weda", "doctolib", "medistory", etc.
  "sessionId": "uuid-genere-par-risquecv" // Identifiant unique de la session
}
```

`correlationId` n'est pas présent dans `risquecv:ready`, car RisqueCV ne connaît pas encore le contexte métier. Il devient obligatoire avec le premier `risquecv:prefill` accepté.

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
  "sessionId": "uuid-genere-par-risquecv", // Le même que celui reçu dans risquecv:ready
  "correlationId": "c56a4180-65aa-42ec-a945-5fd21dec0538", // UUID v4 généré par le logiciel métier (jamais à partir de données patient)
  "options": {
    "pdfAck": true // Facultatif ; true est la valeur par défaut
  },
  "payload": {
    "age": 55,
    "sexe": "femme",
    "pays": "FR",
    "tabac": false,
    "PAS": 142, // pour les valeurs numériques, il faut envoyer des nombres (pas d'unités)
    "atcd": true,
    // ... voir dictionnaire des clés ci-dessus
  }
}
```

L'objet `options` et chacune de ses propriétés sont facultatifs. 
- Si vous utilisez l'option `"pdfAck": false`, le PDF sera considéré comme transmis par RisqueCV dès que `postMessage` aura réussi, sans attendre l'accusé de réception. Ce comportement peut accélérer la fermeture de la fenêtre RisqueCV, mais induit un risque de perte de données si la sauvegarde du PDF échoue de votre côté.

### Étape 3 : La confirmation de réception
#### ✅ `risquecv:prefill:ack` (RisqueCV ➡️ Votre Logiciel)
Envoyé après réception du `prefill`. Confirme quelles données ont été validées et injectées.

```json
{
  "type": "risquecv:prefill:ack", // acknowledge
  "version": 1,
  "partner": "votre-slug",
  "sessionId": "uuid-genere-par-risquecv",
  "correlationId": "c56a4180-65aa-42ec-a945-5fd21dec0538",
  "status": "ok", // "ok", "partial" ou "empty"
  "acceptedKeys": ["age", "sexe", "pays", "tabac", "atcd"],
  "ignoredKeys": ["cleInconnue"] 
}
```

Un `payload` vide `{}` est accepté comme handshake sans donnée clinique et renvoie :

```json
{
  "type": "risquecv:prefill:ack",
  "version": 1,
  "partner": "votre-slug",
  "sessionId": "uuid-genere-par-risquecv",
  "correlationId": "c56a4180-65aa-42ec-a945-5fd21dec0538",
  "status": "empty",
  "acceptedKeys": [],
  "ignoredKeys": []
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
  "sessionId": "uuid-genere-par-risquecv",
  "correlationId": "c56a4180-65aa-42ec-a945-5fd21dec0538",
  "pdfId": "identifiant-opaque-genere-par-risquecv", // Stable lors des éventuelles multiples tentatives d'envoi d'un même PDF. À utiliser comme clé d'idempotence afin de ne pas enregistrer deux fois le même PDF dans votre logiciel, par exemple si le médecin réessaie après un délai dépassé
  "filename": "RisqueCV_19-05-2026_17h45.pdf",
  "mimeType": "application/pdf",
  "encoding": "base64",
  "data": "JVBERi..." // Flux binaire converti en string Base64 (environ 50kB)
}
```
> **Note technique :** La propriété `data` contient la chaîne Base64 brute du PDF (ex: `JVBERi0...`). Elle **ne contient pas** l'en-tête Data URI. Si vous souhaitez générer un lien de téléchargement ou l'afficher, vous devez concaténer la chaîne ainsi en Javascript :
```javascript
const pdfUrl = "data:application/pdf;base64," + msg.data;
``` 

### Étape 5 : La confirmation d'enregistrement du PDF
#### ✅ `risquecv:pdf:ack` (Votre Logiciel ➡️ RisqueCV)

Lorsque `options.pdfAck` vaut `true` (ce qui est le cas par défaut), vous devez envoyer cet accusé après la confirmation de l'enregistrement du PDF dans le dossier patient. Ne pas envoyer cet accusé lors de la réception du message `risquecv:pdf`, mais bien **après l'enregistrement du PDF** dans votre logiciel.

Succès :

```json
{
  "type": "risquecv:pdf:ack",
  "version": 1,
  "partner": "votre-slug",
  "sessionId": "L_ID_RECU_DANS_READY",
  "correlationId": "c56a4180-65aa-42ec-a945-5fd21dec0538",
  "pdfId": "identifiant-opaque-recu-dans-risquecv:pdf",
  "status": "ok"
}
```

Échec :

```json
{
  "type": "risquecv:pdf:ack",
  "version": 1,
  "partner": "votre-slug",
  "sessionId": "L_ID_RECU_DANS_READY",
  "correlationId": "c56a4180-65aa-42ec-a945-5fd21dec0538",
  "pdfId": "identifiant-opaque-recu-dans-risquecv:pdf",
  "status": "error",
  "message": "Le dossier patient n'est pas accessible." // Facultatif : message court et compréhensible par le médecin.
}
```

RisqueCV attend le `pdf:ack` pendant 10 secondes au maximum. En cas d'erreur ou de délai dépassé, il ne réenvoie pas automatiquement le document : le médecin reçoit une explication et peut soit télécharger le PDF pour l'ajouter manuellement, soit déclencher lui-même une nouvelle tentative. Une nouvelle tentative conserve le même `pdfId`.

### Étape 6 : Signal de fermeture
#### 🏁 `risquecv:close` (RisqueCV ➡️ Votre Logiciel)
Envoyé lorsque l'utilisateur clique sur le bouton de retour. Indique que l'hôte doit fermer l'interface d'intégration.

```json
{
  "type": "risquecv:close",
  "version": 1,
  "partner": "votre-slug",
  "sessionId": "L_ID_RECU_DANS_READY",
  "correlationId": "c56a4180-65aa-42ec-a945-5fd21dec0538"
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
  "correlationId": "c56a4180-65aa-42ec-a945-5fd21dec0538", // Absent seulement avant un prefill avec correlationId valide
  "code": "INVALID_SESSION",
  "message": "La session d integration ne correspond pas a la page ouverte."
}
```

| Code | Signification |
| :--- | :--- |
| `INVALID_MESSAGE_FORMAT` | Le JSON ne respecte pas la structure attendue, par exemple un `prefill`/`pdf:ack` sans `correlationId` UUID v4, un `pdf:ack` sans `pdfId`/`status`, un `correlationId` différent de celui figé pour la session, ou une option connue dont la valeur n'est pas du bon type. |
| `UNSUPPORTED_VERSION`| La version du protocole est différente de celle utilisée par le backend de RisqueCV. |
| `UNSUPPORTED_MESSAGE_TYPE`| Le `type` de message n'est pas pris en charge. |
| `INVALID_SESSION` | Le `sessionId` est manquant ou incorrect. |
| `PAYLOAD_NOT_A_FLAT_OBJECT` | Le `payload` n'est pas un objet JSON plat. |
| `VALID_BUT_EMPTY_PAYLOAD` | Aucune donnée clinique valide n'a été trouvée dans un payload non vide (toutes les clés sont inconnues, nulles ou invalides). |
| `INVALID_PARTNER` | Le slug partenaire ne correspond pas à l'URL ouverte. |
| `PDF_GENERATION_FAILED` | La génération du PDF a échoué. |
| `PREFILL_ALREADY_APPLIED` | Un `prefill` a déjà été appliqué pour cette session. |
| `PAYLOAD_TOO_LARGE` | Le `payload` contient trop de clés (maximum 200). |

---

## 🛠 Mode debug

Si vous rencontrez des difficultés (pas de réponse au handshake, données non injectées, etc.), vous pouvez activer le **mode verbeux** en ajoutant le paramètre `debug_integration=1` à l'URL :  
- `https://risquecv.fr/votre-slug/?debug_integration=1`


### Ce que le mode debug affiche dans votre console :

1.  **Confirmation d'initialisation** :
    - `[RisqueCV] Initialisation intégration pour partenaire : votre-slug`
    - Valide que votre URL d'intégration est correctement reconnue par RisqueCV.

2.  **Erreurs de sécurité (rejets silencieux)** :
    - `[RisqueCV] Origine non autorisée : https://votre-url.com` (Si votre domaine n'est pas dans notre liste blanche).
    - `[RisqueCV] Source de message non attendue.` (Si le message ne provient pas de l'objet `window` ayant ouvert RisqueCV).

3.  **Erreurs protocolaires** :
    - Chaque code d'erreur (`INVALID_SESSION`, `UNSUPPORTED_VERSION`, etc.) est journalisé avec une explication textuelle détaillée.
    - Facilite le débogage de vos payloads JSON sans avoir à inspecter manuellement chaque `event.data`.

<script src="https://cdnjs.cloudflare.com/ajax/libs/prism/1.29.0/prism.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/prism/1.29.0/components/prism-json.min.js"></script>
