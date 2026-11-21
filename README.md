<div align="center">
<img src="assets/yo-avatar.png" alt="Yunuscan Oruk — YO monogram" width="72">

# Yunuscan Oruk

**Offline-first verification, security, and contract tooling for AI coding agents and MCP.**

I build small, zero-bloat Python CLIs and read-only MCP servers focused on explicit contracts, deterministic failure paths, and honest limits.

[Repo Contract Check](https://github.com/No3214/repo-contract-check#quickstart) · [MCP Vulnerability Research](https://github.com/No3214/mcp-vulnerability-research) · [Resource Ledger](https://github.com/No3214/resource-ledger#quick-start)
</div>

---

## Active Public Tools

| Project | What it verifies or queries | Stack |
| --- | --- | --- |
| **[mcp-vulnerability-research](https://github.com/No3214/mcp-vulnerability-research)** | Read-only MCP server querying OSV, NVD, CISA KEV, FIRST EPSS, and deps.dev across 7 tools with source context and explicit pagination. | Python 3.11+ · stdio MCP |
| **[repo-contract-check](https://github.com/No3214/repo-contract-check)** | Check explicit JSON and TOML expectations across local repositories offline without executing project commands. | Python 3.11+ stdlib · CLI |
| **[resource-ledger](https://github.com/No3214/resource-ledger)** | Validate monthly electricity, water, and waste CSV records offline, keep missing months visible, and generate JSON or Markdown reports. | Python 3.11+ stdlib · CLI |

---

## Releasing Next: Offline Agent Harness Suite

Locally verified zero-dependency Python 3.10+ tools staged for public `v0.1.0` repository and PyPI release (links will go live as each repository publishes):

| Stage | Tool | Scope & Verification Model | PyPI Package |
| --- | --- | --- | --- |
| Pre-execution | `mcp-guard` | Static scanner for MCP configs, exported tool schemas, and `SKILL.md`/`AGENTS.md` files: hidden Unicode/HTML injection, Lethal Trifecta risk, redacted secret detection, SHA-256 rug-pull lockfiles, context-budget token overhead, and SARIF 2.1.0. | `mcp-guard` *(staged)* |
| Pre-merge | `agent-eval-gate` | Offline trajectory grading, prompt-injection Attack Success Rate (ASR) vs. utility pass rate, Wilson 95% confidence intervals, Rogan-Gladen judge calibration, baseline regression diffs, SARIF/JUnit output, and a path-contained MCP server. | `agent-eval-gate` *(staged)* |
| Post-execution | `agent-receipt` | Cryptographic SHA-256 receipts binding command exit codes to exact git `HEAD`, working-tree hashes, test-file hashes (`--strict-tests`), optional HMAC-SHA256 signing, PR Markdown proof tables, and a read-only MCP server. | `agent-receipt-verify` *(staged)* |

---

## Engineering Principles

**Narrow scope -> deterministic offline check -> test real failure modes -> state limits explicitly.**

- A passing static config scan does not replace OS sandboxing or runtime isolation.
- An eval gate checks recorded trajectories and calibrated judges, not open-ended human judgment.
- A command receipt proves what exited `0` on which exact file tree, not semantic test strength.

---

## Civic Prototype

- **[nobetci-eczane](https://github.com/No3214/nobetci-eczane)** — Turkish emergency pharmacy-finder PWA prototype with map routing and offline caching (Next.js / TypeScript). Verify official pharmacy listings before travelling.

---

## Feedback & Türkçe

Bug reports and edge-case reproductions belong on each active repository's issue tracker with your goal, exact command or tool call, expected output, and actual output.

Yapay zeka kodlama ajanları, Model Context Protocol (MCP) yapılandırmaları ve küçük ekipler için sıfır bağımlılıklı, çevrimdışı doğrulama ve güvenlik araçları geliştiriyorum. Her araç dar bir soruna odaklanır, hata durumlarını açıkça raporlar ve neleri doğrulayıp neleri doğrulamadığını şeffaf biçimde belgeler.
