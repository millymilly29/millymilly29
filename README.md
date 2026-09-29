<div align="center">
  <img src="assets/header.svg?v=55555" alt="Maison Margiela × Yeezy Software Archive — Kirill Tsyganov" width="100%">
</div>

```
KIRILL TSYGANOV // SOFTWARE ARCHIVE
AI AUTOMATION · PRODUCTION AGENTS · LOW-LATENCY SYSTEMS
```

Systems & AI Automation engineer building autonomous tool-calling agents, multimodal vision pipelines, enterprise RAG systems, and in-memory databases. Zero framework bloat. Strict token economics. Empirical benchmarks.

```
[ SPECIFICATION TAGS ]
[ STATUS — ACTIVE ARCHIVE ]   [ RUNTIME — PYTHON 3.11+ / NODE V22 / FASTAPI ]   [ ARCH — MEASURED METRICS ]
```

---

### [ CURATED SPECIFICATION MATRIX ]

| NO. | OBJECT | TECH STACK | PRIMARY METRIC / KEY ARCHITECTURE | SOURCE |
| :--- | :--- | :--- | :--- | :---: |
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
| `N° 13` | **AGENT-FIREWALL** | Node / AST Command Scanner | Deterministic dry-run safety gateway · **SHA-256 audit chain** | [**View Code →**](https://github.com/therealfullmetal55555/agent-firewall) |
| `N° 14` | **SYNAPSE** | Node / Browser JS (Zero-Dep) | `0.245ms P50` in-memory HNSW vector database · `99.1% Recall` | [**View Code →**](https://github.com/therealfullmetal55555/synapse) |
| `N° 15` | **CASE-STUDIES** | Python / APScheduler / Sheets | E-commerce automation · **~77% time reduction (~27h/mo)** | [**View Details →**](https://github.com/therealfullmetal55555/automation-case-studies) |
| `N° 16` | **CONTENT-QA-PIPELINE** | n8n / Groq / OpenAI / HITL | **Multi-agent writer** · Anti-cliché reviewer gate · State machine | [**View Code →**](https://github.com/therealfullmetal55555/content-qa-pipeline) |
| `N° 17` | **TELEGRAM-RAG-SCRAPER** | Python / Telethon / ChromaDB / RAG | **Enterprise channel scraper** · 100% vector citation engine | [**View Code →**](https://github.com/therealfullmetal55555/telegram-rag-scraper) |
| `N° 18` | **SMART-INBOX-AGENT** | n8n / FastAPI / Groq / Vision | **Zero-touch inbox triage** · Math-verified invoice parsing -> Sheets | [**View Code →**](https://github.com/therealfullmetal55555/smart-inbox-agent) |
| `N° 19` | **N8N-CRM-INTAKE** | n8n / HubSpot / Gemini / Qdrant | **5/5 triage pass** · HITL webhook approval · Promise guardrail | [**View Code →**](https://github.com/therealfullmetal55555/n8n-crm-intake-hubspot) |
| `N° 20` | **N8N-QDRANT-RAG** | n8n / Qdrant / Gemini / Docker | **Closed-book RAG** · Mandatory citation diffing · Refusal protocol | [**View Code →**](https://github.com/therealfullmetal55555/n8n-qdrant-rag-assistant) |
| `N° 21` | **N8N-RESEARCH-AGENT** | n8n / Tavily / Gemini / ReAct | **8-call hard budget** · SSRF-safe fetcher · Citation truth guard | [**View Code →**](https://github.com/therealfullmetal55555/n8n-autonomous-research-agent) |

---

### [ CORE STACK ]

```
AI & ORCHESTRATION    n8n (Docker), Qdrant, LlamaIndex, LangChain, Google Gemini, OpenAI (GPT-4o / Vision), ChromaDB
WORKFLOWS & CRM       HubSpot API v3, Airtable, Google Calendar / Sheets API v4, Twilio WhatsApp, aiogram 3.x, Playwright
SYSTEMS & STORAGE     PostgreSQL 16, In-Memory DBs, TypedArrays (Float64Array), SQLite, HNSW Graph, AST Command Scanners
```

---

```
GARMENT CARE / CONTACT
LOCATION      Europe / Remote
TELEGRAM      @therealfullmetal
EMAIL         millyrock2900@gmail.com
LINKEDIN      https://linkedin.com/in/kirill-tsyganov-a8681241a
CARE          DO NOT BLEACH · DRY FLAT · 100% RAW CODE
```
