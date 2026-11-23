<div align="center">
<img src="assets/yo-avatar.png" alt="Yunuscan Oruk — YO monogram" width="72">

# Yunuscan Oruk

**Verification, advisory provenance, and contract tooling for developers and MCP workflows.**

I build small, deterministic Python CLIs and read-only Model Context Protocol (MCP) servers focused on explicit contracts, tested failure paths, and honest boundaries.

[MCP Vulnerability Research](https://github.com/No3214/mcp-vulnerability-research) · [Repo Contract Check](https://github.com/No3214/repo-contract-check#quickstart) · [Resource Ledger](https://github.com/No3214/resource-ledger#quick-start)
</div>

---

## Active Open-Source Tools

| Project | What it verifies or queries | Runtime |
| --- | --- | --- |
| **[mcp-vulnerability-research](https://github.com/No3214/mcp-vulnerability-research)** | Read-only stdio MCP server querying OSV, NVD, CISA KEV, FIRST EPSS, and deps.dev across 7 tools with source provenance, per-provider trust boundaries, and explicit pagination. | Python 3.11+ · stdio MCP |
| **[repo-contract-check](https://github.com/No3214/repo-contract-check)** | Check explicit JSON and TOML expectations across local repositories offline without executing project code or leaking local paths into reports. | Python 3.11+ stdlib · CLI |
| **[resource-ledger](https://github.com/No3214/resource-ledger)** | Validate monthly electricity, water, and waste CSV records offline, keep missing months explicit as null rather than zero, and emit deterministic JSON or Markdown reports. | Python 3.11+ stdlib · CLI |

Each repository documents its verified behavior, exact exit codes, and current scope limits.

---

## How I Work

**Define a narrow contract → test failure and adversarial paths first → document what is and is not verified.**

- A passing repository contract check proves a declared manifest value or file exists, not that tests ran or a runtime is compatible.
- An advisory lookup surfaces upstream OSV, NVD, KEV, EPSS, and deps.dev evidence, not an automated exploitability verdict.
- A ledger report summarizes recorded measurements per unit without fabricating missing months or cross-unit totals.

---

## Civic Prototype

- **[nobetci-eczane](https://github.com/No3214/nobetci-eczane)** — Turkish on-duty pharmacy finder PWA prototype with map routing and offline caching (Next.js / TypeScript). Prototype only; always confirm official pharmacy duty listings before travelling.

---

## Feedback & Collaboration

Bug reports and edge-case reproductions belong on each project's issue tracker with your goal, exact command or MCP tool call, expected output, and actual output:

- [mcp-vulnerability-research issues](https://github.com/No3214/mcp-vulnerability-research/issues)
- [repo-contract-check issues](https://github.com/No3214/repo-contract-check/issues)
- [resource-ledger issues](https://github.com/No3214/resource-ledger/issues)
- For security disclosures, follow each repository's `SECURITY.md` policy.

---

## Türkçe

Geliştiriciler, MCP iş akışları ve küçük ekipler için açık kuralları denetleyen, danışma kaynaklarını şeffaf tutan ve çevrimdışı çalışabilen araçlar geliştiriyorum. Her projenin belgelerinde doğrulanan davranışlar, hata çıkış kodları ve kapsam sınırları açıkça ayrılır.
