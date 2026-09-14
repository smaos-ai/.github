# 🛡️ SMAOS — Sovereign Multi-Agent Governance Suite

> **Deterministic Truth by Design: Local-first execution, invariant testing, and cryptographic verification for autonomous AI agents.**

State integrity, safety, and human agency must never be left to probabilistic guessing. SMAOS provides the execution, diagnostic, and attestation substrate required to deploy autonomous agents in regulated, mission-critical environments.

---

### 📜 The SMAOS Governance Manifesto

```text
                                CRITICAL INVARIANT:
                         Capability ≠ Authority
                                   │
                                   ├── Agent  = Drafts, Calculates, Simulates (Hands)
                                   └── Human  = Authorizes, Decides, Governs (Soul)

                             THE ZERO-EGRESS LAW:
           Privacy is not a promise — it is 0-byte network egress 
                  proven by air-gapped cryptographic Merkle DAGs.

                        THE COMPACTION IMMUNITY PRINCIPLE:
        Type-aware memory locks human constraints verbatim, preventing 
          the Compaction Cliff from silently degrading safety rules.

                             SACRED STEWARDSHIP:
          Technology built to expand human creative agency, not to extract
                human value into centralized cloud monopolies.
```

---

### 🔄 The Open-Source Agent Lifecycle

Our open-source core governs the three critical transition boundaries of autonomous agent execution:

```text
  INPUT (Context & Token Hygiene)
  └── context-governor ──► Optimizes prompt-cache hit rate & prevents context bloat
        │
        ▼
  EXECUTION (Action Uncertainty Diagnostic)
  └── aeib ──────────────► Tests fail-closed precedence & UNKNOWN-state handling
        │
        ▼
  ATTESTATION (Cryptographic Action Receipts)
  └── star-protocol ─────► Generates Ed25519-signed AST Merkle DAG action capsules
```

---

### 📦 Core Repositories & Quickstart

| Stage | Repository | Function | Quickstart |
| :---: | :--- | :--- | :--- |
| **Input** | [`context-governor`](https://github.com/smaos-ai/context-governor) | Prompt-cache hit rate & token economics | `npx @smaos/context-governor --dry-run` |
| **Execution** | [`aeib`](https://github.com/smaos-ai/aeib) | Reference benchmark for action uncertainty — Tests fail-closed precedence and UNKNOWN-state handling | `docker compose run --rm benchmark` |
| **Attestation** | [`star-protocol`](https://github.com/smaos-ai/star-protocol) | Local AST Merkle DAG receipt generator | `npx @smaos/star verify` |

The reference benchmark is configured to run without network access and does not require cloud services. Container execution uses `network_mode: none` and does not transmit prompts or source. This describes the reference configuration, not every possible host, plugin, or developer invocation.

---

### 🏛️ The 3-Tier Governance Hierarchy

SMAOS separates lightweight developer tooling from high-assurance enterprise compliance:

- **Tier 1 (Diagnostics)**: [`context-governor`](https://github.com/smaos-ai/context-governor), [`aeib`](https://github.com/smaos-ai/aeib) (10 deterministic scenarios), `memory-benchmark` *(v0.2.0 Sprint)*
- **Tier 2 (Verification)**: [`star-protocol`](https://github.com/smaos-ai/star-protocol), `smaos-verify` *(zero-egress WASM)*, `ghost-audit` *(local sandbox scanner)*
- **Tier 3 (Enterprise)**: `SMAOS Core` — DORA Article 28/30, EU AI Act Art. 12/14 compliance, and bitemporal `agentacct.db` ledger *(Commercial SOW)*

---

### 🤝 Engagement & Verification

- **Run the Benchmark**: Clone and reproduce [`aeib`](https://github.com/smaos-ai/aeib) offline via `docker compose run --rm benchmark`.
- **Token Efficiency**: Measure your local cache efficiency with [`context-governor`](https://github.com/smaos-ai/context-governor).
- **Enterprise Verification**: For air-gapped forensic reviews and DORA Article 28/30 compliance tabletop kits, open a discussion or inquiry.
