🌐 **[Português](#português) | [English](#english)**

---

<div id="português"></div>

# Inglês do Pré-A1 ao C2

Material de estudo pessoal para aprender inglês do zero ao nível mais alto do Quadro Europeu Comum de Referência (CEFR), pensado especificamente para falantes de português brasileiro.

O projeto inteiro vive em um único arquivo HTML (`ingles-pre-a1-ao-c2.html`), que funciona como um livro interativo no navegador — 100% offline, sem dependências externas — e já está formatado para ser exportado como PDF em tamanho A4.

## Sobre o material

A ideia aqui foi fugir de listas soltas de regras e montar um caminho único, apoiado em referências acadêmicas e gramáticas de uso (Swan, Murphy, Roach, Cruttenden, *English Profile*), focado em quatro objetivos reais: conversar com nativos, fazer entrevistas de emprego (incluindo entrevistas técnicas de TI), acompanhar aulas universitárias e prestar exames de proficiência.

* **Base em inglês britânico (RP/SSBE):** ortografia, vocabulário, gramática e transcrições em IPA seguem o padrão britânico. Sempre que o inglês americano diverge de um jeito que importa na prática, há um quadro indicando a diferença.
* **Feito para brasileiros:** em vez de ensinar inglês de forma genérica, cada seção ataca diretamente os erros de interferência do português (como omitir o sujeito, usar o presente no lugar do *present perfect* com *for/since*, colocar vogal de apoio em consoantes finais ou cair em falsos cognatos).
* **Prática fora do texto:** como nenhum texto substitui áudio e fala, o material traz instruções prontas para configurar dois agentes de IA no Gemini ou ChatGPT — o **Teacher** (para exercícios guiados e simulados orais) e o **Mate** (um amigo fictício de Manchester que conversa e corrige por *recasts* + lista periódica) —, além de roteiros de prática com amigos nativos.
* **Referências verificadas:** as regras, estimativas de horas e técnicas de estudo (repetição espaçada, recuperação ativa, *shadowing*) trazem a citação da fonte no próprio texto, com a lista completa de referências ao final.

## Estrutura e andamento

Esta é uma versão parcial. Os blocos entram no arquivo conforme passam pela pesquisa e pela revisão final.

| Parte | Nível CEFR | Foco principal | Status |
| :--- | :--- | :--- | :--- |
| **1** | **Introdução + Pré-A1** | Como funciona o CEFR, plano de estudo, configuração dos agentes de IA, sons do inglês (IPA), alfabeto, números, *to be* e blocos de sobrevivência. | Concluído |
| **2** | **A1** (*Breakthrough*) | *Present simple*, *present continuous*, *have got*, *there is/are*, *can*, preposições *in/on/at* e situações básicas do dia a dia. | Concluído |
| **3** | **A2** (*Waystage*) | *Past simple* e pronúncia do *-ed*, *past continuous*, formas de futuro, comparativos, modais de obrigação, introdução ao *present perfect* e guia do exame **A2 Key**. | Concluído |
| **4** | **B1** (*Threshold*) | *Present perfect* × *past simple* (*for/since*), *past perfect*, *used to*, condicionais 0–2, voz passiva, *reported speech*, relativas, entrevista STAR, notas de aula e **B1 Preliminary**. | Concluído |
| **5** | **B2** (*Vantage*) | Tempos narrativos completos, futuro avançado, 3ª condicional e mistas, *wish*, modais no passado, passiva impessoal, *phrasal verbs* mais frequentes no BNC, escrita acadêmica/ensaios e **B2 First / IELTS / TOEFL**. | Concluído |
| **6** | **C1** (*Effective Operational Proficiency*) | Registro acadêmico e profissional avançado, nuances, inversão, coesão em textos longos e **C1 Advanced**. | Planejado |
| **7** | **C2** (*Mastery*) | Precisão lexical, idiomaticidade, reconstrução de argumentos e **C2 Proficiency**. | Planejado |
| **8** | **Inglês para TI** | Vocabulário técnico, documentação, *dailies/stand-ups*, *code review*, *system design* e entrevistas técnicas (dividido em básico, intermediário e avançado). | Planejado |

## Como usar

Você não precisa instalar nada nem rodar servidor.

1. Baixe o arquivo `ingles-pre-a1-ao-c2.html`.
2. Abra diretamente em qualquer navegador moderno (no computador ou no celular).

### Recursos da interface e destaques técnicos

Além do conteúdo didático, construí o arquivo como uma aplicação web *single-file* de leitura e estudo, usando apenas HTML, CSS e JavaScript puro (Vanilla JS):

* **Arquitetura Single-File / 100% Offline:** todas as fontes variáveis (*Nunito*, *Inter* e *JetBrains Mono* em formato `woff2`) foram convertidas para Base64 e embutidas no CSS. Todos os diagramas (trapézio vocálico, cortes articulatórios, linhas do tempo e fluxogramas) foram desenhados em SVG inline. O arquivo não faz nenhuma requisição externa.
* **Marca-texto persistente (`M`):** implementado com as APIs nativas `Selection`, `Range` e `TreeWalker` do DOM, permitindo grifar trechos mesmo quando atravessam múltiplas tags HTML. As marcações salvam contexto e posição no `localStorage`, e um painel modal permite consultar, excluir ou pular direto para o trecho marcado com animação de foco.
* **Motor de impressão para PDF (`@media print`):** o botão **Gerar PDF** aciona uma folha de estilos pensada para papel A4 no tema claro, preservando a paleta botânica (verde-musgo e creme), escondendo elementos de interface e controlando quebras de página (`break-inside: avoid`) em tabelas, quadros e figuras.
* **Navegação e leitura:** barra de progresso de leitura, *scroll-spy* que acompanha a seção atual no sumário lateral, modo tela cheia (tecla `[`), alternância entre tema claro e escuro com persistência local e botão de cópia rápida nos blocos de prompt.

---

<div id="english"></div>

# English from Pre-A1 to C2 (Self-Study Guide & Single-File Web App)

A comprehensive, self-contained British English study guide written in Portuguese specifically for Brazilian learners, covering the entire Common European Framework of Reference for Languages (CEFR) from **Pre-A1 to C2**.

The entire project is built as a **single, dependency-free HTML file** (`ingles-pre-a1-ao-c2.html`) that works 100% offline as an interactive book in the browser and compiles cleanly into an A4 PDF via native print styles.

## About the Project

Rather than compiling disconnected grammar rules, I built this guide as a structured, evidence-based roadmap grounded in linguistics and ELT reference works (Swan, Murphy, Roach, Cruttenden, and the *English Profile* corpus). It is designed around four practical goals: holding natural conversations with native speakers, passing job interviews (including software engineering/IT interviews), attending university lectures, and taking proficiency exams.

* **British English Standard (RP/SSBE):** Spelling, vocabulary, grammar, and IPA transcriptions follow British norms, with dedicated callout boxes highlighting American English differences whenever they matter in practice.
* **Tailored for Brazilian Portuguese Speakers:** Every section directly targets L1 interference errors common among Brazilians (e.g., omitted subjects, using the present tense instead of the *present perfect* with *for/since*, vowel epenthesis in final consonant clusters, and false friends).
* **AI-Assisted & Real-World Practice:** Because text alone cannot replace listening and speaking, the guide includes structured system prompts to configure two custom AI agents — **Teacher** (for adaptive drills and official-format mock speaking exams) and **Mate** (a fictional developer from Manchester who chats naturally and provides *recasts* + periodic correction tables) — alongside tandem scripts for practicing with native friends.
* **Academic Rigor:** Study methods (spaced repetition, active retrieval, shadowing), hour estimates, and phonological rules are cited inline with a full bibliography at the end of the document.

## Content Roadmap

This is an ongoing project. New parts are added as they complete research and final review.

| Part | CEFR Level | Main Focus | Status |
| :--- | :--- | :--- | :--- |
| **1** | **Intro + Pre-A1** | How the CEFR works, study plan, AI agent setup, English phonology (IPA), alphabet, numbers, *to be*, and survival chunks. | Completed |
| **2** | **A1** (*Breakthrough*) | *Present simple*, *present continuous*, *have got*, *there is/are*, *can*, prepositions *in/on/at*, and everyday survival scenarios. | Completed |
| **3** | **A2** (*Waystage*) | *Past simple* & *-ed* pronunciation, *past continuous*, future forms, comparatives, modals, intro to *present perfect*, and the **A2 Key** exam. | Completed |
| **4** | **B1** (*Threshold*) | *Present perfect* vs. *past simple* (*for/since*), *past perfect*, *used to*, conditionals 0–2, passive voice, *reported speech*, relative clauses, STAR interviews, lecture note-taking, and **B1 Preliminary**. | Completed |
| **5** | **B2** (*Vantage*) | Full narrative tenses, advanced future, 3rd & mixed conditionals, *wish*, past modals of deduction, impersonal passive, top BNC *phrasal verbs*, academic writing/essays, and **B2 First / IELTS / TOEFL**. | Completed |
| **6** | **C1** (*Effective Operational Proficiency*) | Advanced academic and professional register, hedging, inversion, cohesion in long texts, and **C1 Advanced**. | Planned |
| **7** | **C2** (*Mastery*) | Lexical precision, idiomaticity, argument reconstruction, and **C2 Proficiency**. | Planned |
| **8** | **English for IT** | Technical vocabulary, documentation, stand-ups, code reviews, system design, and technical interviews (split into Basic, Intermediate, and Advanced). | Planned |

## Technical Highlights (Front-End & Architecture)

Beyond the educational content, I engineered the HTML file as a custom, zero-dependency reading environment using **semantic HTML5, CSS3, and Vanilla JavaScript**:

* **True Single-File Architecture (100% Offline):** Variable `woff2` fonts (*Nunito*, *Inter*, and *JetBrains Mono*) are Base64-encoded directly into the stylesheet. All linguistic diagrams (vowel trapezoids, articulatory mouth cross-sections, timelines, and decision flowcharts) are custom inline SVGs. The file makes zero external network requests.
* **Persistent DOM Text Highlighter (`M`):** Built from scratch using the native `Selection`, `Range`, and `TreeWalker` APIs, allowing users to highlight text seamlessly even across nested HTML tags. Highlights store text offsets and surrounding context in `localStorage`, and a built-in drawer modal lets users review, delete, or smooth-scroll directly to any saved highlight.
* **Print-to-PDF Styling (`@media print`):** Clicking **Gerar PDF** triggers a dedicated print stylesheet tailored for A4 pages. It forces the light-mode botanical palette, strips out UI chrome, and manages pagination (`break-inside: avoid`, `orphans`, `widows`) so tables, callout boxes, and SVG figures never split awkwardly across pages.
* **UX & Accessibility:** Features a reading progress bar, automatic scroll-spy syncing with the collapsible sidebar, distraction-free fullscreen mode (shortcut `[`), light/dark theme persistence, and one-click copy buttons for all AI prompts.

## How to Run

No build step, package manager, or local server required:

1. Download `ingles-pre-a1-ao-c2.html`.
2. Open it in any modern desktop or mobile browser.