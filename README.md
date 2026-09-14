# SMAOS — Sovereign Multi-Agent Governance Suite

Local-first execution and verification for autonomous AI agents.

| Stage | Repository | Function | Quickstart |
| :--- | :--- | :--- | :--- |
| **Input** | [`context-governor`](https://github.com/smaos-ai/context-governor) | Prompt-cache hit rate & token economics | `npx @smaos/context-governor --dry-run` |
| **Execution** | [`aeib`](https://github.com/smaos-ai/aeib) | Reference benchmark for action uncertainty — Tests fail-closed precedence and UNKNOWN-state handling | `docker compose run --rm benchmark` |
| **Attestation** | [`star-protocol`](https://github.com/smaos-ai/star-protocol) | Local AST Merkle DAG receipt generator | `npx @smaos/star verify` |

The reference benchmark is configured to run without network access and does not require cloud services. Container uses `network_mode: none`.

- **Tier 1**: `context-governor`, `aeib` (10 scenarios — see fixture list), `memory-benchmark`
- **Tier 2**: `star-protocol`, `smaos-verify`, `ghost-audit`
- **Tier 3**: `SMAOS Core` — commercial SOW
