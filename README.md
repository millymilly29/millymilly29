<div align="center">

```
╔══════════════════════════════════════════════════════╗
║  KIRILL TSYGANOV                                     ║
║  Building AI systems that actually perform.          ║
╚══════════════════════════════════════════════════════╝
```

</div>

<br>

I build **low-latency AI infrastructure** — vector engines, voice pipelines, agentic runtimes — from first principles, without ORMs or framework magic. Zero-dependency where it matters. Benchmarks over claims.

**Currently focused on:** autonomous agent tooling, sub-millisecond retrieval, and realtime voice AI.

---

### Systems

<table>
<tr>
<td width="50%" valign="top">

**[`hypercontext`](https://github.com/millymilly29/hypercontext)**  
2M-token Gemini monorepo archaeologist with persistent context caching and AST blast-radius analysis.  
`−75% cost` · `1.15s TTFT` · `16/16 tests`

</td>
<td width="50%" valign="top">

**[`synapse`](https://github.com/millymilly29/synapse)**  
In-process vector database with HNSW skip-graph, SQ8 quantization, and hybrid BM25/RRF retrieval.  
`<0.6ms P50` · `97.2% Recall@10` · `17/17 tests`

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[`subsecond`](https://github.com/millymilly29/subsecond)**  
Voice streaming engine with speculative intent prefetching and zero-buffer barge-in cancellation.  
`235ms E2E` · `<0.1ms cutoff` · `15/15 tests`

</td>
<td width="50%" valign="top">

**[`agent-firewall`](https://github.com/millymilly29/agent-firewall)**  
Command pattern firewall & dry-run safety gateway for autonomous AI agent tool execution.  
`10 threat rules` · `SHA-256 audit` · `9/9 tests`

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[`columnarjs`](https://github.com/millymilly29/columnarjs)**  
In-process columnar analytics engine with TypedArray storage and vectorized GROUP BY aggregation.  
`1M rows in 4ms` · `zero-dependency` · `28/28 tests`

</td>
<td width="50%" valign="top">

**[`swarm-operator`](https://github.com/millymilly29/swarm-operator)**  
Event-driven multi-agent mission control with DAG orchestration and live token telemetry.  
`4-agent swarm` · `<1ms bus` · `18/18 tests`

</td>
</tr>
</table>

---

### Stack

```
Languages    TypeScript  JavaScript  Python  Bash
Runtimes     Node.js v24  Web Audio API  V8
AI / LLM     Gemini 2.0 / 1.5 Pro  Claude 3.7 Sonnet
Algorithms   HNSW  BM25  RRF  SQ8  Speculative Decoding  Columnar
Security     Command Pattern Gateway  SHA-256 Audit Chain  Dry-Run Sandbox
```

---

### Contact

[`millymilly29.github.io`](https://millymilly29.github.io) &nbsp;·&nbsp; [`@therealfullmetal`](https://t.me/therealfullmetal) &nbsp;·&nbsp; [`millyrock2900@gmail.com`](mailto:millyrock2900@gmail.com)
