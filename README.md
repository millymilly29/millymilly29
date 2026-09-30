<div align="center">
  <img src="assets/header.svg?v=55555" alt="Kirill Tsyganov — Software Archive" width="100%">
  
  <br/>
  
  # KIRILL TSYGANOV
  ### **Production AI Agents · Enterprise RAG · Low-Latency Systems**
  
  > **I build AI agents that say "I don't know" instead of making things up.**
  
  [![Telegram](https://img.shields.io/badge/Telegram-@therealfullmetal-2BA2E4?style=flat-square&logo=telegram&logoColor=white)](https://t.me/therealfullmetal)
  [![Status](https://img.shields.io/badge/Status-Open_to_Work_%2F_Freelance-000000?style=flat-square)](https://t.me/therealfullmetal)
  [![Location](https://img.shields.io/badge/Location-Tallinn_%2F_Europe_%2F_Remote-lightgrey?style=flat-square)](https://t.me/therealfullmetal)
  [![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)](LICENSE)

  <p align="center">
    <a href="https://t.me/therealfullmetal"><b>💬 Direct Chat on Telegram</b></a> •
    <a href="#-flagship-systems"><b>⚡ Flagship Systems</b></a> •
    <a href="#-curated-specification-matrix"><b>📊 All 27 Projects</b></a> •
    <a href="#-work-with-me"><b>💼 Services & Work with Me</b></a>
  </p>
</div>

---

### ⚡ [ FLAGSHIP SYSTEMS ]

```
PROOF OF ARCHITECTURE · DETERMINISTIC GUARDRAILS · MEASURED METRICS
```

#### 01 // [SYNAPSE](https://github.com/therealfullmetal55555/synapse) — In-Memory HNSW Vector Database
> **Sub-millisecond vector indexing & hybrid search without external container bloat.**
* **The Problem:** Production agent loops degrade in speed when querying heavy cloud vector databases for short-term and conversational memory.
* **The Solution:** Pure JavaScript in-memory HNSW skip-graph indexer with `Float64Array` storage, hybrid BM25 lexical search, and zero dependencies.
* **Measured Metric:** Recall@10 98.5% at N=500 → 78.8% at N=5,000 on default settings (random 64-d vectors, brute-force ground truth); P50 0.3–0.9 ms. Tunable via `efSearch` (98.0% recall at `efSearch=128`): see the recall/latency curve in the repo.
* 🔗 **[Explore Repository & Architecture →](https://github.com/therealfullmetal55555/synapse)**

#### 02 // [AGENT-FIREWALL](https://github.com/therealfullmetal55555/agent-firewall) — Autonomous Agent Execution Sandbox
> **A first-line command gate for AI agents: regex rules, risk policies, dry-run rewrite, tamper-evident audit log.**
* **The Problem:** Autonomous LLM agents with bash/tool access can generate dangerous commands (`rm -rf`, curl-pipe-sh, data exfiltration) when prompt-injected.
* **The Solution:** 10 threat rules (rm -rf, .env exfiltration, cloud IMDS, curl|bash, reverse shells…), 4 policy profiles (PARANOID / STRICT_CI / AIRGAPPED / DEVELOPMENT), automatic dry-run rewrite and a SHA-256 hash-chained audit log.
* **Measured Metric:** 10 rules · 4 policies · 13 tests, including checks for known bypasses (base64, variable indirection) and cryptographic hash chain verification. Zero dependencies. Meant to sit in front of an OS-level sandbox, not replace it.
* 🔗 **[Explore Repository & Architecture →](https://github.com/therealfullmetal55555/agent-firewall)**

#### 03 // [PASSMARK](https://github.com/therealfullmetal55555/passmark) & [BENCH-SUITE](https://github.com/therealfullmetal55555/bench-suite) — Statistical AI Evaluation Engine
> **Empirical AI evaluation harness & 172-task benchmark suite eliminating subjective vibe-checks.**
* **The Problem:** Prompts and agents are typically evaluated with arbitrary single-number averages without statistical significance testing.
* **The Solution:** Paired McNemar significance testing ($p < 0.05$), Cohen’s $\kappa = 0.718$ LLM-as-a-Judge calibration, and multi-objective Pareto Frontier analysis (Accuracy vs Latency vs Token Cost) across 6 core agent task families.
* **Measured Metric:** 172 curated tasks · 477 automated tests (100% pass) · Statistical evidence, not vibes: paired McNemar test + bootstrap CIs (reproduce via `pytest -v` or `python3 simulate_pipeline.py`).
* 🔗 **[View PASSMARK →](https://github.com/therealfullmetal55555/passmark)** · **[View BENCH-SUITE →](https://github.com/therealfullmetal55555/bench-suite)**

---

### 📦 [ CURATED PRODUCTION HIGHLIGHTS ]

| SYSTEM | TECH STACK | ARCHITECTURE & BUSINESS IMPACT | SOURCE |
| :--- | :--- | :--- | :---: |
| **N8N-LINT** | Node.js / CLI / GitHub Action / SARIF | **ESLint for n8n workflows** · 12 security rules, ungated write detection after LLMs, offline browser playground | [**View Code →**](https://github.com/therealfullmetal55555/n8n-lint) |
| **WORKBENCH** | FastAPI / Postgres RLS / Stripe / Celery | **Multi-tenant SaaS foundation** · Database-enforced tenant isolation (PostgreSQL FORCE ROW LEVEL SECURITY, verified by tests that connect as the app role) | [**View Code →**](https://github.com/therealfullmetal55555/workbench) |
| **OBSERVABILITY-STACK** | OpenTelemetry / Tempo / Prometheus / Grafana | **Agent Telemetry Stack** · RED metrics, trace-to-log correlation, 15 Prometheus alert rules & 5 dashboards | [**View Code →**](https://github.com/therealfullmetal55555/observability-stack) |
| **INVOICE-AGENT** | Vision LLM / Pydantic v2 / Sheets | **98.6% field accuracy** · Multimodal OCR parsing, multi-currency validation, null-over-guessing guardrails | [**View Code →**](https://github.com/therealfullmetal55555/invoice-document-agent) |
| **BREWCRAFT-CARE** | n8n / Qdrant / Gemini / Postgres | **20/20 acceptance pass** · Grounded RAG support desk, hybrid confidence gate, human handoff | [**View Code →**](https://github.com/therealfullmetal55555/brewcraft-rag-support) |
| **WHATSAPP-RECEPTIONIST** | FastAPI / Twilio / Google Cal | **Timezone reconciliation** · Confirm-before-write appointment state machine, zero booking conflicts | [**View Code →**](https://github.com/therealfullmetal55555/whatsapp-ai-receptionist) |
| **CONTENT-QA-PIPELINE** | n8n / Groq / OpenAI / HITL | **Multi-agent writer** · Anti-cliché reviewer gate, draft generation, Telegram human-in-the-loop | [**View Code →**](https://github.com/therealfullmetal55555/content-qa-pipeline) |

<details>
<summary><b>📂 Expand to View Complete Specification Matrix (All 28 Systems)...</b></summary>
<br/>

| NO. | OBJECT | TECH STACK | PRIMARY METRIC / KEY ARCHITECTURE | SOURCE |
| :--- | :--- | :--- | :--- | :---: |
| `N° 00` | **N8N-LINT** | Node.js / CLI / GitHub Action / SARIF | **12 security rules · 72/72 tests** · Ungated LLM write detection · Web UI | [**View Code →**](https://github.com/therealfullmetal55555/n8n-lint) |
| `N° 01` | **BREWCRAFT-CARE** | n8n / Qdrant / Gemini / Postgres | **20/20 acceptance tests** · Hybrid confidence gate · Injection shield | [**View Code →**](https://github.com/therealfullmetal55555/brewcraft-rag-support) |
| `N° 02` | **WHATSAPP-RECEPTIONIST** | FastAPI / Twilio / Google Cal | **Timezone reconciliation** · Confirm-before-write state machine | [**View Code →**](https://github.com/therealfullmetal55555/whatsapp-ai-receptionist) |
| `N° 03` | **INVOICE-AGENT** | Vision LLM / Pydantic v2 | **98.6% field accuracy** · Null-over-guessing guardrail · Sheets sync | [**View Code →**](https://github.com/therealfullmetal55555/invoice-document-agent) |
| `N° 04` | **INBOUND-LEAD-AGENT** | n8n / Ollama / Airtable / Telegram | **10/10 eval pass** · \$0 token cost · Multi-channel deduplication | [**View Code →**](https://github.com/therealfullmetal55555/inbound-lead-qualification-agent) |
| `N° 05` | **ECOM-PRICE-MONITOR** | HTTPX Async / SQLite / Telegram | **Sub-50ms WB API v4** · 5-day price history · Telegram delta alerts | [**View Code →**](https://github.com/therealfullmetal55555/ecom-price-monitor) |
| `N° 06` | **BROWSER-USE-AGENT** | Playwright Async / Vision AI | **Coordinate computer use** · Loop detection · `$0.01/run cost` | [**View Code →**](https://github.com/therealfullmetal55555/browser-use-agent) |
| `N° 07` | **LLM-EVAL-HARNESS** | YAML Specs / LLM-as-a-Judge | **19 test cases (93.0% pass)** · Isolated criteria evaluation | [**View Code →**](https://github.com/therealfullmetal55555/llm-eval-harness) |
| `N° 08` | **CRM-LEAD-AUTOMATION** | FastAPI / HubSpot API v3 | **Anti-hallucination budget** · Contact deduplication · Spam shield | [**View Code →**](https://github.com/therealfullmetal55555/crm-lead-automation) |
| `N° 09` | **RAG-SUPPORT-BOT** | Python / LlamaIndex / ChromaDB | `$0.000165 / query` · Mandatory citations · SQLite memory | [**View Code →**](https://github.com/therealfullmetal55555/rag-support-bot) |
| `N° 10` | **N8N-LEADGEN** | n8n / Docker / GPT-4o-mini | `$0.057 / 1K leads` · 13-node scraper & heuristic pitch generator | [**View Code →**](https://github.com/therealfullmetal55555/n8n-ai-leadgen-outreach) |
| `N° 11` | **N8N-ASSISTANT** | n8n / LangChain / GPT-4o | Multi-tool agent · **Confirm-Before-Write** safety gate | [**View Code →**](https://github.com/therealfullmetal55555/n8n-ai-executive-assistant) |
| `N° 12` | **MILLY-FX-PRO** | CEP 11+ / ExtendScript / AE | **26+ procedural FX modules** · 7 one-click master recipes | [**View Code →**](https://github.com/therealfullmetal55555/millyfx-pro) |
| `N° 13` | **AGENT-FIREWALL** | Node / Regex Command Scanner | Deterministic dry-run safety gateway · **SHA-256 audit chain** | [**View Code →**](https://github.com/therealfullmetal55555/agent-firewall) |
| `N° 14` | **SYNAPSE** | Node / Browser JS (Zero-Dep) | `0.245ms P50` in-memory HNSW vector database · `99.1% Recall` | [**View Code →**](https://github.com/therealfullmetal55555/synapse) |
| `N° 15` | **CASE-STUDIES** | Python / APScheduler / Sheets | E-commerce automation · **~77% time reduction (~27h/mo saved)** | [**View Details →**](https://github.com/therealfullmetal55555/automation-case-studies) |
| `N° 16` | **CONTENT-QA-PIPELINE** | n8n / Groq / OpenAI / HITL | **Multi-agent writer** · Anti-cliché reviewer gate · State machine | [**View Code →**](https://github.com/therealfullmetal55555/content-qa-pipeline) |
| `N° 17` | **TELEGRAM-RAG-SCRAPER** | Python / Telethon / ChromaDB / RAG | **Enterprise channel scraper** · 100% vector citation engine | [**View Code →**](https://github.com/therealfullmetal55555/telegram-rag-scraper) |
| `N° 18` | **SMART-INBOX-AGENT** | n8n / FastAPI / Groq / Vision | **Zero-touch inbox triage** · Math-verified invoice parsing -> Sheets | [**View Code →**](https://github.com/therealfullmetal55555/smart-inbox-agent) |
| `N° 19` | **N8N-CRM-INTAKE** | n8n / HubSpot / Gemini / Qdrant | **5/5 triage pass** · HITL webhook approval · Promise guardrail | [**View Code →**](https://github.com/therealfullmetal55555/n8n-crm-intake-hubspot) |
| `N° 20` | **N8N-QDRANT-RAG** | n8n / Qdrant / Gemini / Docker | **Closed-book RAG** · Mandatory citation diffing · Refusal protocol | [**View Code →**](https://github.com/therealfullmetal55555/n8n-qdrant-rag-assistant) |
| `N° 21` | **N8N-RESEARCH-AGENT** | n8n / Tavily / Gemini / ReAct | **8-call hard budget** · SSRF-safe fetcher · Citation truth guard | [**View Code →**](https://github.com/therealfullmetal55555/n8n-autonomous-research-agent) |
| `N° 22` | **PREMIERE-FLOW-PRO** | CEP 11.0 / ExtendScript / PPRO | **27+ timeline automation modules** · BeatGrid BPM · Ken Burns | [**View Code →**](https://github.com/therealfullmetal55555/premiere-flow-pro) |
| `N° 23` | **INDUSTRIAL-LOFI-PS** | CEP 12.0 / ScriptUI / Photoshop | **29+ ActionDescriptor FX recipes** · Thermal heatmap · Halftone · Noir | [**View Code →**](https://github.com/therealfullmetal55555/industrial-lofi-ps) |
| `N° 24` | **WORKBENCH** | FastAPI / Postgres RLS / Stripe / Celery | **Multi-tenant SaaS backend** · Stripe webhook state machine · Tenant RLS isolation | [**View Code →**](https://github.com/therealfullmetal55555/workbench) |
| `N° 25` | **OBSERVABILITY-STACK** | OpenTelemetry / Tempo / Prometheus / Grafana | **Agent telemetry stack** · RED metrics · Trace-to-log correlation · 15 alert rules | [**View Code →**](https://github.com/therealfullmetal55555/observability-stack) |
| `N° 26` | **PASSMARK** | Python 3.11+ / NumPy / SciPy / Rich | **Empirical AI eval harness** · Paired diffs · McNemar test · Cohen's κ calibration | [**View Code →**](https://github.com/therealfullmetal55555/passmark) |
| `N° 27` | **BENCH-SUITE** | Python 3.11+ / Pydantic v2 / JSONSchema | **172 tasks across 6 families** · Stratified scoring · Pareto frontier analysis | [**View Code →**](https://github.com/therealfullmetal55555/bench-suite) |

</details>

---

### 💼 [ WORK WITH ME ]

I help engineering teams, startups, and businesses build **reliable AI systems that run in production without hallucinations, runaway token costs, or data leaks**.

#### What I Build:
1. **Autonomous AI Agents & Tool-Calling Workflows** (FastAPI, n8n, LangChain, Playwright) — structured data extraction, CRM sync, customer support with human-in-the-loop.
2. **Enterprise RAG & Grounded Search** (Qdrant, ChromaDB, LlamaIndex) — strict citation verification, closed-book guardrails, sub-second latency.
3. **AI Safety, Firewalls & Sandboxing** (command-pattern scanning, input sanitization, rate-limiting, tamper-evident audit logging).
4. **Custom Backend & Automation Engines** (PostgreSQL RLS, Stripe state machines, OpenTelemetry observability).

#### Engagement Format:
* **Rapid Prototyping:** Working MVP with unit tests in 5–7 business days.
* **Production Deployment:** Full Docker Compose / CI/CD and observability.
* **Direct Communication:** Daily asynchronous updates + Telegram channel.

👉 **Ready to automate your operations? Reach out directly:**
* **Telegram:** [@therealfullmetal](https://t.me/therealfullmetal)
* **LinkedIn:** [Kirill Tsyganov](https://linkedin.com/in/kirill-tsyganov-a8681241a)
* **Email:** `millyrock2900 [at] gmail.com`

---

### 🇷🇺 [ ДЛЯ РУССКОЯЗЫЧНЫХ КЛИЕНТОВ / СНГ ]

Разрабатываю **производственные AI-агенты, RAG-системы и комплексную автоматизацию бизнес-процессов под ключ**:
* **Автономные агенты без галлюцинаций:** квалификация лидов в CRM (AmoCRM, HubSpot), умная сортировка входящих писем и счетов, боты поддержки с контролем точности.
* **Автоматизация e-commerce и маркетинга:** мониторинг цен маркетплейсов (Wildberries / Ozon), кросспостинг контента, сквозная аналитика.
* **Индивидуальные бэкенд-решения:** интеграции Telegram/WhatsApp, вебхуки, биллинг, базы данных с изоляцией тенантов.

💬 **Обсудить задачу или получить консультацию:** [**Написать в Telegram (@therealfullmetal)**](https://t.me/therealfullmetal)
