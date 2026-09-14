# SMAOS — Sovereign Multi-Agent Governance Suite

Deterministic evidence by design: local-first execution, invariant testing,
and cryptographic verification for autonomous AI agents.

SMAOS provides diagnostic and attestation tooling for teams evaluating
autonomous agents in regulated and mission-critical environments.

## Governance Manifesto

**CRITICAL INVARIANT: Capability ≠ Authority**  
The default governance boundary: agents draft, calculate, and simulate;
humans authorize consequential actions.

**REFERENCE CONTAINER NETWORK STATEMENT:**  
The AEIB reference container is configured with `network_mode: none` and
does not require cloud services. For the reference container, privacy
controls include network isolation and locally verifiable execution evidence.

**COMPACTION AWARENESS:**  
Type-aware memory handling aims to preserve human constraints verbatim,
helping reduce the risk of the Compaction Cliff silently degrading safety rules.

**STEWARDSHIP:**  
Technology built to expand human creative agency.

## The Open-Source Agent Lifecycle

```
INPUT: Context & Token Hygiene
└── context-governor → Measures and helps reduce context bloat, optimizes prompt-cache hit rate

EXECUTION: Invariant & Uncertainty Diagnostic
└── aeib → Tests fail-closed precedence and UNKNOWN-state handling

ATTESTATION: Cryptographic Action Receipts
└── star-protocol → Generates locally-signed AST Merkle DAG action capsules (see limits below)
```

## Core Repositories & Quickstart

| Stage | Repository | Function | Quickstart |
| :--- | :--- | :--- | :--- |
| Input | [context-governor](https://github.com/smaos-ai/context-governor) | Prompt-cache hit rate & token economics — Measures and helps reduce context bloat | `npx @smaos/context-governor --dry-run` |
| Execution | [aeib](https://github.com/smaos-ai/aeib) | Reference benchmark — Tests fail-closed precedence and UNKNOWN-state handling | `docker compose run --rm benchmark` |
| Attestation | [star-protocol](https://github.com/smaos-ai/star-protocol) | Local AST Merkle DAG receipt generator | `npx @smaos/star verify` |

> The reference benchmark is configured to run without network access and does not require cloud services. Container execution uses `network_mode: none`; the reference benchmark does not require prompts, source code, or cloud services. This describes the reference configuration, not every possible host, plugin, or developer invocation.

## 3-Tier Hierarchy

**Tier 1 — Diagnostics:** [context-governor](https://github.com/smaos-ai/context-governor), [aeib](https://github.com/smaos-ai/aeib) (10 deterministic scenarios — see fixture list), memory-benchmark (v0.2.0 Sprint)

**Tier 2 — Verification:** [star-protocol](https://github.com/smaos-ai/star-protocol), smaos-verify (WASM verifier), ghost-audit (local sandbox scanner)

**Tier 3 — Enterprise:** SMAOS Core — evidence and tabletop tooling relevant to DORA Articles 28/30 and EU AI Act Articles 12/14; commercial SOW, not a compliance certification. Planned or commercial component: bitemporal agentacct.db ledger.

**What is signed:** JCS-canonical receipt data is hashed with SHA-256; the resulting digest and Merkle root are included in the signed manifest.json.  
**Key supply:** A locally generated Ed25519 keypair is stored locally and is not transmitted by the reference tool.  
**Authenticates:** Integrity and provenance of the local receipt package relative to the signing key.  
**Does not prove:** External-ledger settlement, source-data completeness, DORA compliance, human authorization, or production security.  

## Engagement & Verification

- **Run Benchmark:**
  ```bash
  git clone --branch v0.1.0 https://github.com/smaos-ai/aeib.git aeib
  cd aeib
  docker compose run --rm benchmark
  ```
- **Token Efficiency:** `npx @smaos/context-governor --dry-run`
- **Enterprise:** Feasibility sprint scope, pricing, turnaround per SOW

**Bottom line:** SMAOS provides local diagnostic evidence and cryptographic receipt tooling; it does not claim to establish external-system truth, guarantee privacy across every host, or certify regulatory compliance.
