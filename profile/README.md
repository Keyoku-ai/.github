<div align="center">

  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/keyoku-ai/.github/main/assets/banner-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/keyoku-ai/.github/main/assets/banner-light.svg">
    <img alt="keyoku" src="https://raw.githubusercontent.com/keyoku-ai/.github/main/assets/banner-light.svg" width="800">
  </picture>

  <br><br>

  <p>
    <strong>Your AI agent forgets everything between sessions. Keyoku fixes that.</strong>
  </p>

</div>

<br>

Keyoku is a persistent memory system for AI agents. It stores memories, builds a knowledge graph, and runs a proactive heartbeat that tells your agent what needs attention — without being asked.

One command to install. Zero config to start.

```bash
npx @keyoku/openclaw init
```

---

### Repositories

<table>
<tr>
<td width="50%">

#### [`keyoku`](https://github.com/keyoku-ai/keyoku)

TypeScript SDK and OpenClaw plugin. Auto-recall, auto-capture, heartbeat integration, 7 memory tools, CLI commands.

[![npm](https://img.shields.io/npm/v/@keyoku/openclaw?label=%40keyoku%2Fopenclaw&style=flat-square&color=6366f1)](https://www.npmjs.com/package/@keyoku/openclaw)
[![License: MIT](https://img.shields.io/badge/License-MIT-22c55e?style=flat-square)](https://github.com/keyoku-ai/keyoku/blob/main/LICENSE)

```bash
npx @keyoku/openclaw init
```

</td>
<td width="50%">

#### [`keyoku-engine`](https://github.com/keyoku-ai/keyoku-engine)

The memory engine. Written in Go. Semantic search (HNSW + BM25), knowledge graph, 12-signal heartbeat, memory decay, deduplication. Single binary, zero external dependencies.

[![Go](https://img.shields.io/badge/Go-1.24-00ADD8?style=flat-square&logo=go&logoColor=white)](https://github.com/keyoku-ai/keyoku-engine)
[![License: BSL 1.1](https://img.shields.io/badge/License-BSL_1.1-6366f1?style=flat-square)](https://github.com/keyoku-ai/keyoku-engine/blob/main/LICENSE)

```bash
go install github.com/keyoku-ai/keyoku-engine/cmd/keyoku-server@latest
```

</td>
</tr>
</table>

---

### How It Works

```
Your AI Agent
    │
    ▼
@keyoku/openclaw (plugin)
    │  Every message:
    │    1. Recall — search memory, inject context
    │    2. Respond — agent replies with full memory
    │    3. Capture — extract and store facts
    │  Every heartbeat:
    │    4. Scan — 12 SQL-driven signal checks
    │    5. Analyze — LLM evaluates with knowledge graph
    │    6. Act — agent responds per autonomy level
    ▼
keyoku-engine (local)
    │  semantic search, dedup, decay, knowledge graph
    ▼
SQLite + HNSW (your machine, your data)
```

---

### What makes Keyoku different

| | Store & retrieve | Keyoku |
|---|---|---|
| **Memory** | Save text, search later | Dedup, conflict detection, decay, knowledge graph |
| **Heartbeat** | Read a static file | 12 signals from actual memory — deadlines, sentiment, patterns |
| **Autonomy** | On or off | Three levels: observe, suggest, act |
| **Capture** | Manual or post-session | Real-time per-message extraction |
| **Graph** | None | Entities, relationships, BFS traversal, alias tracking |

---

<div align="center">
  <sub>All data stays on your machine. Open source. Built for agents that need to remember.</sub>
</div>
