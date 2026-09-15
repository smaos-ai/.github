# SMAOS — Sovereign Multi-Agent Governance Suite

Deterministic evidence by design: local-first execution, invariant testing, and cryptographic verification for autonomous AI agents.

SMAOS provides diagnostic, evidence-reconciliation, and attestation tooling for engineering and risk teams evaluating autonomous agents in regulated and mission-critical environments.

## Governance Boundary

**Capability ≠ Authority**  
Agents draft, calculate, and simulate; humans authorize consequential actions.

## AEIB Reference-Container Statement

The AEIB reference container uses `network_mode: none` and requires no prompts,
source code, credentials, or cloud services. This describes the reference
configuration, not every possible host, plugin, or invocation.

## The Open-Source Agent Lifecycle

```
INPUT: Context & Token Hygiene
└── context-governor → Measures and helps reduce context bloat, optimizes prompt-cache hit rate

EXECUTION: Invariant & Uncertainty Diagnostic
└── aeib → Tests fail-closed precedence and UNKNOWN-state handling

ATTESTATION: Cryptographic Action Receipts
└── star-protocol → Generates locally signed Merkle-DAG receipts for specified local artifact sets; see repository documentation for exact verification procedures and limits.
```

## Core Repositories & Quickstart

| Stage | Repository | Function | Quickstart |
| :--- | :--- | :--- | :--- |
| Input | [context-governor](https://github.com/smaos-ai/context-governor) | Prompt-cache hit rate & token economics — Measures and helps reduce context bloat | `npx @smaos/context-governor --dry-run` |
| Execution | [aeib](https://github.com/smaos-ai/aeib) | Reference benchmark — Tests fail-closed precedence and UNKNOWN-state handling | `docker compose run --rm benchmark` |
| Attestation | [star-protocol](https://github.com/smaos-ai/star-protocol) | Generates locally signed Merkle-DAG receipts for specified local artifact sets; see repository documentation for exact verification procedures and limits. | `npx @smaos/star verify` |

## 3-Tier Product Hierarchy

* **Tier 1 — Diagnostics**: [context-governor](https://github.com/smaos-ai/context-governor), [aeib](https://github.com/smaos-ai/aeib) (10 deterministic scenarios), memory-benchmark
* **Tier 2 — Verification**: [star-protocol](https://github.com/smaos-ai/star-protocol), smaos-verify (WASM verifier), ghost-audit (local sandbox scanner)
* **Tier 3 — Enterprise**: SMAOS Core — evidence and tabletop tooling that may support work relevant to DORA Articles 28–30 and EU AI Act Articles 12 and 14; commercial SOW, not a compliance certification or legal opinion. Planned or commercial component: bitemporal agentacct.db ledger.

## Attestation & Signing Scope

* **Attestation Scope**: What is signed and the exact receipt format are documented in the `star-protocol` repository. Receipts authenticate local artifact package integrity relative to the signing key and do not independently establish external-system truth, completeness, or authority.
* **Key supply**: A locally generated Ed25519 keypair is stored locally and is not transmitted by the reference tool.

## Engagement & Verification

* **Run Benchmark**:
  ```bash
  git clone --branch v0.1.0 https://github.com/smaos-ai/aeib.git aeib
  cd aeib
  docker compose run --rm benchmark
  ```
* **Token Efficiency**: `npx @smaos/context-governor --dry-run`
* **Enterprise**: Feasibility sprint scope, pricing, turnaround per SOW (€750 Workflow Evidence Gap Report).

---

**Bottom line:** SMAOS provides local diagnostic evidence and cryptographic receipt tooling; it does not claim to establish external-system truth, guarantee privacy across every host, or certify regulatory compliance.
