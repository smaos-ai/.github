# smaos-ai — Sovereign Multi-Agent OS & Trust Infrastructure

Sovereign, local-first, zero-dependency trust and governance infrastructure for autonomous AI agents.

## 🏛️ Core Public Repositories

### ⚡ [aeib-receipt-fuzzer](https://github.com/smaos-ai/aeib-receipt-fuzzer) *(v0.2.0)*
**Wire-Level Fault Proxy, Toxic Receipt Detector & Offline Audit Log Scanner.**
- **The Problem**: Most agent frameworks sign `CONFIRMED` receipts on HTTP 504 timeouts or dropped sockets, creating toxic receipts and retry hazards.
- **The Solution**: Intercepts tool traffic with 6 wire-fault injection modes (504 timeout, TCP RST drop, JCS tamper) and enforces strict `verdict: UNKNOWN` state preservation.
- **Includes**: `fuzzer.py`, `toxic_receipt_detector.py`, `diff.py` offline scanner, `demo_killshot.py` (18pt terminal presentation), and 10 open conformance test vectors.

### 🧪 [aeib](https://github.com/smaos-ai/aeib) *(v0.1.0)*
**Agent-Effect Integrity Benchmark.** Reference runner and deterministic scenario fixtures for evaluating agent state machine resilience under non-deterministic tool outputs.

### 📜 [star-protocol](https://github.com/smaos-ai/star-protocol)
**Story-Trace-Assert-Receipt (STAR) Protocol.** Local zero-cost agent verification CLI and AST Merkle DAG receipt generator for auditable AI execution.

### 🛡️ [context-governor](https://github.com/smaos-ai/context-governor)
**Token Budget & Context Economic Governance Engine.** Context compaction and budget enforcement harness for agentic context windows.

---

## 💼 Staging Forensic Audit Offer
We deliver bounded audits for payment, engineering, and platform teams operating mutating AI workflows:
- **Tier 1 Diagnostic (€1,500 / 48-Hour Sprint)**: Scan 250+ staging traces, compute Toxic Receipt Index (TRI %), and map retry hazards.
- **Tier 2 Forensic Audit (€2,500 / 5-Day Sprint)**: Full wire-level fault injection, 30-day trace analysis, and delivery of a `git apply fix.patch` remediation.

📩 **Contact**: `andrejlo123@gmail.com`
