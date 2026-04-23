# MCP Infrastructure Portfolio

**20 MCP servers for agent reliability, observability, compliance, and cost control.**

Built to fill gaps in an ecosystem where 52% of remote endpoints are dead and 38% of servers have no authentication. Every server here solves a specific, verifiable problem that existing tools don't address.

[![npm](https://img.shields.io/badge/npm-mdfifty50--boop-red)](https://www.npmjs.com/search?q=mdfifty50-boop)
[![Smithery](https://img.shields.io/badge/Smithery-20_servers-green)](https://smithery.ai)
[![GitHub](https://img.shields.io/badge/GitHub-mdfifty50--boop-black)](https://github.com/mdfifty50-boop)
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

---

## Quick Install

All servers run locally. Node.js 18+ required. No API keys, no accounts, no external services needed to start.

Add to your `claude_desktop_config.json`, Cursor, Windsurf, or VS Code MCP config:

```json
{
  "mcpServers": {
    "agent-observability": { "command": "npx", "args": ["agentic-observability-mcp"] },
    "agent-guard": { "command": "npx", "args": ["agent-guard-mcp"] },
    "agent-security": { "command": "npx", "args": ["agent-security-mcp"] },
    "compliance-shield": { "command": "npx", "args": ["compliance-shield-mcp"] },
    "token-lens": { "command": "npx", "args": ["token-lens-mcp"] },
    "agent-costcenter": { "command": "npx", "args": ["agent-costcenter-mcp"] }
  }
}
```

---

## Server Registry

### Safety & Security
| Server | What It Does | Install |
|--------|-------------|---------|
| [agent-guard-mcp](https://github.com/mdfifty50-boop/agent-guard-mcp) | Loop detection via SHA-256 action fingerprinting + circuit breakers | `npx agent-guard-mcp` |
| [scope-guard-mcp](https://github.com/mdfifty50-boop/scope-guard-mcp) | Multi-agent scope enforcement at the tool call level | `npx scope-guard-mcp` |
| [agent-security-mcp](https://github.com/mdfifty50-boop/agent-security-mcp) | Prompt injection detection, secret scanning, permission auditing | `npx agent-security-mcp` |
| [secure-vault-mcp](https://github.com/mdfifty50-boop/secure-vault-mcp) | AES-256-GCM encrypted secrets with short-lived tokens and rotation | `npx secure-vault-mcp` |
| [agentic-auth-proxy-mcp](https://github.com/mdfifty50-boop/mcp-auth-proxy) | Drop-in auth, rate limiting, and audit logging for any MCP server | `npx agentic-auth-proxy-mcp` |

### Observability & Cost
| Server | What It Does | Install |
|--------|-------------|---------|
| [agentic-observability-mcp](https://github.com/mdfifty50-boop/agent-observability-mcp) | **Only MCP where agents write their own traces** — tool call IS the instrumentation | `npx agentic-observability-mcp` |
| [trace-forge-mcp](https://github.com/mdfifty50-boop/trace-forge-mcp) | Structured trace writing with OpenTelemetry-compatible output | `npx trace-forge-mcp` |
| [agent-costcenter-mcp](https://github.com/mdfifty50-boop/agent-costcenter-mcp) | Cross-provider cost attribution with budget alerts and reports | `npx agent-costcenter-mcp` |
| [token-lens-mcp](https://github.com/mdfifty50-boop/token-lens-mcp) | Context window analysis, token budgeting, and smart truncation | `npx token-lens-mcp` |

### Compliance & Knowledge
| Server | What It Does | Install |
|--------|-------------|---------|
| [compliance-shield-mcp](https://github.com/mdfifty50-boop/compliance-shield-mcp) | EU AI Act audit trails, risk classification, transparency logging | `npx compliance-shield-mcp` |
| [gcc-intelligence-mcp](https://github.com/mdfifty50-boop/gcc-intelligence-mcp) | ZATCA Phase 2, UAE Corporate Tax, GCC regulatory intelligence | `npx gcc-intelligence-mcp` |
| [domain-expertise-mcp](https://github.com/mdfifty50-boop/domain-expertise-mcp) | Domain knowledge injection with source-cited confidence tagging | `npx domain-expertise-mcp` |
| [qc-validator-mcp](https://github.com/mdfifty50-boop/qc-validator-mcp) | Schema validation, content quality scoring, hallucination detection | `npx qc-validator-mcp` |

### Agent Infrastructure
| Server | What It Does | Install |
|--------|-------------|---------|
| [agent-memory-mcp](https://github.com/mdfifty50-boop/agent-memory-mcp) | Cross-session persistent memory: facts, decisions, relationships | `npx agent-memorystore-mcp` |
| [agent-reflexion-mcp](https://github.com/mdfifty50-boop/agent-reflexion-mcp) | Agent self-improvement — decision logging, pattern analysis, goals | `npx agent-reflexion-mcp` |
| [agent-workflow-mcp](https://github.com/mdfifty50-boop/agent-workflow-mcp) | Multi-step workflow orchestration with dependencies and pause/resume | `npx agent-workflow-mcp` |
| [agent-replay-mcp](https://github.com/mdfifty50-boop/agent-replay-mcp) | Session recording, replay, and divergence detection for debugging | `npx agent-replay-mcp` |
| [a2a-bridge-mcp](https://github.com/mdfifty50-boop/a2a-bridge-mcp) | Agent-to-agent communication with capability discovery and task delegation | `npx a2a-bridge-mcp` |
| [mcp-registry-mcp](https://github.com/mdfifty50-boop/mcp-registry-mcp) | MCP server fleet health monitoring and duplicate detection | `npx mcp-registry-mcp` |

### Documents
| Server | What It Does | Install |
|--------|-------------|---------|
| [docx-forge-mcp](https://github.com/mdfifty50-boop/docx-forge-mcp) | Create, read, and manipulate Word documents programmatically | `npx docx-forge-mcp` |

---

## Why These Exist

Built from systematic analysis of 21,949+ MCP servers across Glama, Smithery, npm, and GitHub:

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
| [npm](https://www.npmjs.com/search?q=mdfifty50-boop) | 10 published, 10 pending |
| [Smithery](https://smithery.ai) | All 20 listed |
| [MCPize](https://mcpize.com) | 14 deployed |
| [Glama](https://glama.ai/mcp/servers) | All 20 auto-indexed |
| [GitHub](https://github.com/mdfifty50-boop) | All 20 — source + releases |

---

## License

MIT — all servers. See individual repos for details.

---

*Statistics sourced from: Glama (April 2026), vulnerablemcp.info, Mindgard.ai MCP Security Trends, Trend Micro Feb 2026 MCP scan.*
