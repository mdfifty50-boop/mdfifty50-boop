# MCP Infrastructure Portfolio

**18 MCP servers for agent reliability, observability, compliance, and cost control.**

Built to fill gaps in an ecosystem where 52% of remote endpoints are dead and 38% of servers have no authentication. Every server here solves a specific, verifiable problem that existing tools don't address.

[![npm](https://img.shields.io/badge/npm-mdfifty50--boop-red)](https://www.npmjs.com/search?q=mdfifty50-boop)
[![GitHub](https://img.shields.io/badge/GitHub-mdfifty50--boop-black)](https://github.com/mdfifty50-boop)
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

---

## Quick Install

All servers run locally. Node.js 18+ required. No API keys, no accounts, no external services needed to start.

Add to your `claude_desktop_config.json`, Cursor, Windsurf, or VS Code MCP config:

```json
{
  "mcpServers": {
    "agent-observability": {
      "command": "npx",
      "args": ["agentic-observability-mcp"]
    },
    "agent-guard": {
      "command": "npx",
      "args": ["agent-guard-mcp"]
    },
    "agent-security": {
      "command": "npx",
      "args": ["agent-security-mcp"]
    },
    "agent-workflow": {
      "command": "npx",
      "args": ["agent-workflow-mcp"]
    },
    "agent-reflexion": {
      "command": "npx",
      "args": ["agent-reflexion-mcp"]
    },
    "docx-forge": {
      "command": "npx",
      "args": ["docx-forge-mcp"]
    }
  }
}
```

---

## Server Registry

| Server | Category | What It Does | Install |
|--------|----------|-------------|---------|
| [agentic-observability-mcp](https://github.com/mdfifty50-boop/agent-observability-mcp) | Observability | **Only MCP where agents write their own traces** — tool call IS the instrumentation | `npx agentic-observability-mcp` |
| [trace-forge-mcp](https://github.com/mdfifty50-boop/trace-forge-mcp) | Observability | Structured trace writing with OpenTelemetry-compatible output | `npx trace-forge-mcp` |
| [agent-guard-mcp](https://github.com/mdfifty50-boop/agent-guard-mcp) | Safety | Loop detection via SHA-256 action fingerprinting + circuit breakers | `npx agent-guard-mcp` |
| [scope-guard-mcp](https://github.com/mdfifty50-boop/scope-guard-mcp) | Safety | Multi-agent scope enforcement at the tool call level | `npx scope-guard-mcp` |
| [agent-security-mcp](https://github.com/mdfifty50-boop/agent-security-mcp) | Security | Config scanning, prompt injection detection, credential leak detection | `npx agent-security-mcp` |
| [agentic-auth-proxy-mcp](https://github.com/mdfifty50-boop/mcp-auth-proxy) | Security | Add auth, rate limiting, and audit logging to any MCP server | `npx agentic-auth-proxy-mcp` |
| [compliance-shield-mcp](https://github.com/mdfifty50-boop/compliance-shield-mcp) | Compliance | EU AI Act audit trails, bias detection, transparency logging | `npx compliance-shield-mcp` |
| [gcc-intelligence-mcp](https://github.com/mdfifty50-boop/gcc-intelligence-mcp) | Compliance | ZATCA Phase 2, UAE Corporate Tax, GCC regulatory knowledge | `npx gcc-intelligence-mcp` |
| [agent-costcenter-mcp](https://github.com/mdfifty50-boop/agent-costcenter-mcp) | Cost | Cross-provider cost attribution for multi-model systems | `npx agent-costcenter-mcp` |
| [token-lens-mcp](https://github.com/mdfifty50-boop/token-lens-mcp) | Cost | Context window manifest analysis and budget planning | `npx token-lens-mcp` |
| [agent-memory-mcp](https://github.com/mdfifty50-boop/agent-memory-mcp) | Memory | Cross-session memory: facts, decisions, relationships | `npx agent-memory-mcp` |
| [agent-reflexion-mcp](https://github.com/mdfifty50-boop/agent-reflexion-mcp) | Learning | Agent self-improvement — decision logging, pattern analysis, goals | `npx agent-reflexion-mcp` |
| [agent-workflow-mcp](https://github.com/mdfifty50-boop/agent-workflow-mcp) | Orchestration | Multi-step workflow orchestration with dependencies and pause/resume | `npx agent-workflow-mcp` |
| [qc-validator-mcp](https://github.com/mdfifty50-boop/qc-validator-mcp) | Quality | Schema validation, content quality scoring, hallucination detection | `npx qc-validator-mcp` |
| [domain-expertise-mcp](https://github.com/mdfifty50-boop/domain-expertise-mcp) | Knowledge | Domain knowledge injection with source-cited confidence tagging | `npx domain-expertise-mcp` |
| [docx-forge-mcp](https://github.com/mdfifty50-boop/docx-forge-mcp) | Documents | Create, read, and manipulate Word documents programmatically | `npx docx-forge-mcp` |
| [secure-vault-mcp](https://github.com/mdfifty50-boop/secure-vault-mcp) | Security | Encrypted credential storage for agent workflows | `npx secure-vault-mcp` |
| [mcp-registry-mcp](https://github.com/mdfifty50-boop/mcp-registry-mcp) | Infrastructure | MCP server discovery and registry querying | `npx mcp-registry-mcp` |

**Bonus servers:** [a2a-bridge-mcp](https://github.com/mdfifty50-boop/a2a-bridge-mcp) (Google A2A ↔ MCP bridge) | [agent-replay-mcp](https://github.com/mdfifty50-boop/agent-replay-mcp) (session replay and debugging)

---

## Why These Exist

This portfolio was built in response to a systematic analysis of 21,949+ MCP servers across Glama, Smithery, npm, and GitHub:

- **52%** of remote MCP endpoints are dead on arrival (Glama, April 2026)
- **38%** of servers requiring auth have none (Mindgard.ai scan)
- **36.7%** of 7,000+ servers are vulnerable to SSRF (vulnerablemcp.info)
- **492** servers run with zero auth AND zero encryption (Trend Micro, Feb 2026)
- **91%** of servers are wrappers around existing APIs with no unique value

The gap is not more servers — it's reliable infrastructure for the agents already running.

---

## Distribution

| Registry | Status |
|----------|--------|
| [npm](https://www.npmjs.com/search?q=mdfifty50-boop) | All servers published |
| [Smithery](https://smithery.ai) | All servers listed |
| [Glama](https://glama.ai/mcp/servers) | Auto-indexed |
| [GitHub](https://github.com/mdfifty50-boop) | Source + releases |

---

## License

MIT — all servers. See individual repos for details.

---

*Statistics sourced from: Glama (April 2026), vulnerablemcp.info, Mindgard.ai MCP Security Trends, Trend Micro Feb 2026 MCP scan, Grand View Research AI agent observability market sizing.*
