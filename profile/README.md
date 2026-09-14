# 🛡️ SMAOS — Sovereign Multi-Agent Governance Suite

> **Local-first, zero-egress execution and cryptographic verification for autonomous AI agents.**

SMAOS provides the execution, diagnostic, and attestation substrate required to deploy autonomous agents in regulated, mission-critical environments. Every open-source diagnostic and verification tool executes locally with **0-byte external cloud egress**.

---

### 🔄 The Open-Source Agent Lifecycle

Our open-source core governs the three critical transition boundaries of autonomous agent execution:

```text
┌─────────────────────────────────────────────────────────────────────────────┐
│ 1. INPUT: Context & Token Hygiene                                           │
│ └── context-governor ──► Optimizes prompt-cache hit rate & token economics   │
├─────────────────────────────────────────────────────────────────────────────┤
│ 2. EXECUTION: Invariant & Uncertainty Diagnostic                            │
│ └── aeib ──────────────► Enforces fail-closed precedence & UNKNOWN states   │
├─────────────────────────────────────────────────────────────────────────────┤
│ 3. ATTESTATION: Cryptographic Action Receipts                               │
│ └── star-protocol ─────► Generates Ed25519-signed AST Merkle action capsules│
└─────────────────────────────────────────────────────────────────────────────┘
```

---

### 📦 Core Repositories & Quickstart

| Stage | Repository | Function | Quickstart |
| :---: | :--- | :--- | :--- |
| **Input** | [`context-governor`](https://github.com/smaos-ai/context-governor) | Claude Code prompt-cache hit rate & token economics | `npx @smaos/context-governor --dry-run` |
| **Execution** | [`aeib`](https://github.com/smaos-ai/aeib) | Diagnostic benchmark for action uncertainty | `docker compose run --rm benchmark` |
| **Attestation** | [`star-protocol`](https://github.com/smaos-ai/star-protocol) | Local zero-cost AST Merkle DAG receipt generator | `npx @smaos/star verify` |

---

### 🏛️ The 3-Tier Governance Hierarchy

SMAOS separates lightweight developer tooling from high-assurance enterprise compliance:

| Tier | Component | Focus Area | Key Output / Deliverable | Status |
| :--- | :--- | :--- | :--- | :---: |
| **Tier 1: Diagnostics** | [`context-governor`](https://github.com/smaos-ai/context-governor) | Prompt cache efficiency & cost | Prompt Cache Hit Rate (%) | **Live** |
| | [`aeib`](https://github.com/smaos-ai/aeib) | Action uncertainty & fail-closed states | 10 Deterministic Scenarios | **Live v0.1.0** |
| | `memory-benchmark` | Safety retention & Compaction Cliff | Rule Survival Rate (%) | *v0.2.0 Sprint* |
| **Tier 2: Verification** | [`star-protocol`](https://github.com/smaos-ai/star-protocol) | Local cryptographic attestation | Ed25519 Merkle DAG Receipts | **Live v1.0.0** |
| | `smaos-verify` | Air-gapped browser/CLI receipt verification | Sub-2s WASM Verifier | *Packaging* |
| | `ghost-audit` | Local developer runtime & sandbox scanner | Governance Intensity Index | *Internal Beta* |
| **Tier 3: Enterprise** | `SMAOS Core` | DORA Art. 28/30 & EU AI Act Art. 12/14 compliance | Bitemporal `agentacct.db` Ledger | **Commercial SOW** |

---

### 🔒 Zero-Egress Security Guarantee

All Tier 1 and Tier 2 tools are strictly **local-first**:
* **No Telemetry**: No user prompts, source code, or traces leave your environment.
* **Air-Gapped Operation**: Benchmark and verification suites run with network isolation (`network_mode: "none"`).
* **Deterministic Verification**: Independent mathematical assertions without third-party API dependencies.

---

### 🤝 Getting Involved

- **AEIB Reproduction Sprint**: Run our offline reference benchmark [`aeib`](https://github.com/smaos-ai/aeib) and report edge cases or ambiguities.
- **Cache Optimization**: Measure your Claude Code token efficiency with [`context-governor`](https://github.com/smaos-ai/context-governor).
- **Enterprise Inquiries**: For DORA Article 28/30 tabletop audit kits and Feasibility Sprints, review our specifications or open a discussion.
