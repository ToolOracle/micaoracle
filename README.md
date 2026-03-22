# 🪙 MiCAOracle

**MiCA Compliance MCP Server** — 20 tools | Part of [ToolOracle](https://tooloracle.io)

![Tools](https://img.shields.io/badge/MCP_Tools-20-10B898?style=flat-square)
![Status](https://img.shields.io/badge/Status-Live-00C853?style=flat-square)
![Tier](https://img.shields.io/badge/Tier-Enterprise-FF6D00?style=flat-square)
![Bus](https://img.shields.io/badge/Oracle_Bus-Connected-00C853?style=flat-square)

## Quick Connect

```bash
# Claude Desktop / Cursor / Windsurf
npx -y mcp-remote https://tooloracle.io/mica-ampel/mcp/
```

```json
// claude_desktop_config.json
{
  "mcpServers": {
    "micaoracle": {
      "command": "npx",
      "args": ["-y", "mcp-remote", "https://tooloracle.io/mica-ampel/mcp/"]
    }
  }
}
```

## Tools (20)

| Tool | Description |
|------|-------------|
| `readiness_check` | Full MiCA readiness score + Ampel per article for a token. GREEN/YELLOW/RED/GREY |
| `article_status` | Detailed Ampel for a specific MiCA article with check conditions. |
| `gap_report` | MiCA compliance gaps: RED/YELLOW/GREY with priority and actions. |
| `assess_token` | Run LIVE MiCA assessment via FeedOracle mica_full_pack. Evaluates 18 checks, upd |
| `entity_list` | List all registered entities. |
| `create_entity` | Register a new regulated entity. |
| `audit_trail` | Chain-linked audit log with integrity check. |
| `health_check` | Server + DB status. |
| `issuer_profile` | Issuer profile with all tokens and aggregate MiCA Ampel. Shows authorization sta |
| `entity_ampel` | Aggregate MiCA Ampel for an entity across ALL tokens it custodies. Shows per-tok |
| `issuer_list` | List all known token issuers with MiCA authorization status and tokens. |
| `link_token` | Link a token to an entity for monitoring. |
| `assess_entity` | Assess ALL tokens for an entity in one call. Runs live FeedOracle assessment for |
| `bridge_resolve` | Start bridge resolution for a MiCA gap. Generates template (issuer engagement, r |
| `bridge_approve` | Approve or reject a bridge resolution. Approval upgrades Ampel to GREEN. |
| `bridge_status` | Show all bridge resolutions for an entity/token. |
| `bus_status` | Oracle Event Bus status: events, cross-refs, connected oracles. |
| `freshness_check` | Expire stale evidence. Downgrades GREEN→YELLOW if evidence older than max_age_da |
| `mica_watchdog` | Monitor ESMA/EBA/BaFin for MiCA regulatory changes. Returns monitored sources an |
| `generate_report` | Generate MiCA compliance report for a token. Full article breakdown, evidence, b |

## Pricing

| Tier | Rate Limit | Price |
|------|-----------|-------|
| Free | 10 calls/day | €0 |
| Pro | 1,000 calls/day | €99/month |
| Enterprise | Unlimited | Custom |

> **Note:** This is a compliance oracle. Full tool access requires a Pro or Enterprise subscription. Free tier includes read-only assessment tools.

## Part of ToolOracle

MiCAOracle is one of **42 specialized MCP servers** in the [ToolOracle](https://tooloracle.io) ecosystem — the largest collection of production-ready MCP tools for AI agents.

### MiCA Coverage

**Related Oracles:**
- [FeedOracle](https://feedoracle.io) — Evidence-grade compliance data infrastructure
- [ToolOracle](https://tooloracle.io) — 42 Oracles, 390+ MCP Tools

## Links

- 🌐 Live: `https://tooloracle.io/mica-ampel/mcp/`
- 📚 Docs: [tooloracle.io/docs](https://tooloracle.io/docs)
- 🏠 Platform: [tooloracle.io](https://tooloracle.io)

---

*Built by [FeedOracle](https://feedoracle.io) — Evidence by Design*
