<div align="center">

  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/keyoku-ai/.github/main/assets/banner-dark.svg?v=2">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/keyoku-ai/.github/main/assets/banner-light.svg?v=2">
    <img alt="keyoku" src="https://raw.githubusercontent.com/keyoku-ai/.github/main/assets/banner-light.svg?v=2" width="800">
  </picture>

  <br><br>

  <p>
    <strong>Your coding agent, with muscle memory.</strong>
  </p>

</div>

<br>

Keyoku watches how you work in Claude Code, Cursor, or Codex, learns your repeated patterns, and turns them into workflows you run with one command. Approve once — never re-explain a process again.

One command to install. Works out of the box — no API key required. Add a Gemini or Anthropic key when you want model-refined suggestions. Everything stays on your machine.

```bash
npx keyoku init
```

---

### Repositories

<table><tr><td width="50%" valign="top">

**[`keyoku`](https://github.com/keyoku-ai/keyoku)** — MCP server & CLI (TypeScript)

[![npm](https://img.shields.io/npm/v/keyoku?label=keyoku&style=flat-square&color=6366f1)](https://www.npmjs.com/package/keyoku) [![License: MIT](https://img.shields.io/badge/License-MIT-22c55e?style=flat-square)](https://github.com/keyoku-ai/keyoku/blob/main/LICENSE)

Activity tracing, pattern detection, workflow execution, goal convergence, connector gateway

</td><td width="50%" valign="top">

**[`keyoku-engine`](https://github.com/keyoku-ai/keyoku-engine)** — Memory & knowledge backend (Go)

[![Go](https://img.shields.io/badge/Go-1.24-00ADD8?style=flat-square&logo=go&logoColor=white)](https://github.com/keyoku-ai/keyoku-engine) [![License: BSL 1.1](https://img.shields.io/badge/License-BSL_1.1-6366f1?style=flat-square)](https://github.com/keyoku-ai/keyoku-engine/blob/main/LICENSE)

Semantic search, knowledge graph, memory decay, 12-signal heartbeat — powers team sync and the context graph

</td></tr></table>

---

### How It Works

```
Claude Code · Cursor · Codex
    │
    ├─ PostToolUse hook ──► activity log (local JSONL)
    │                            │
    └─ MCP connection            ▼
         │              pattern detection
         │           heuristics find candidates,
         │           a small model refines them
         │                    │
         ▼                    ▼
   workflow_execute ◄── approved templates
         │
         ├─ bash steps    → run directly (timeouts, audit)
         ├─ agent steps   → hand off to your coding agent
         └─ review steps  → wait for your sign-off
```

---

### What makes Keyoku different

| | Snippets & aliases | Keyoku |
|---|---|---|
| **Discovery** | You write them by hand | Learned from how you actually work |
| **Steps** | Static shell commands | Bash + agent judgment + human review, mixed |
| **Execution** | Fire and forget | Step-by-step state, pause/resume, full audit trail |
| **Scope** | One machine, one shell | Any MCP agent; team sync via keyoku-engine |
| **Trust** | Implicit | Approval is the boundary — nothing runs unsigned |

---

<div align="center">
  <sub>All data stays on your machine. Open source. Built for agents that do real work.</sub>
</div>
