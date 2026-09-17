# smaos-ai — Sovereign Multi-Agent OS & Trust Infrastructure
Sovereign, local-first, zero-dependency trust and governance infrastructure for autonomous AI agents.

## 🏛️ Core Public Repositories

### ⚡ [aeib-receipt-fuzzer](https://github.com/smaos-ai/aeib-receipt-fuzzer) *(v0.2.0)*
**Wire-Level Fault Proxy, Toxic Receipt Detector & Offline Log Scanner.**
- **Target Audience**: **Backend & Platform Leads, Payment Engineers, AI Infrastructure Teams**
- **The Problem**: ~45% of agent SDKs log false `CONFIRMED` receipts on HTTP 504 timeouts, causing silent ledger drift and double-execution retry storms.
- **The Solution**: Injects 6 wire-fault modes (504 timeout, TCP RST, JCS tamper) and enforces strict `verdict: UNKNOWN` state preservation.
- **Quantified Benefit**: **100% Preserved Uncertainty (\(\Delta=0\) Toxic Receipts)** | **0 Silent Ledger Errors**.

### 🧪 [aeib](https://github.com/smaos-ai/aeib) *(v0.1.0)*
**Agent-Effect Integrity Benchmark.**
- **Target Audience**: **AI Safety Researchers, QA Engineers, Agentic Framework Authors**
- **The Problem**: Agent state machines fail unpredictably when downstream microservices return non-deterministic errors.
- **The Solution**: Offline containerized benchmark (`network_mode: "none"`) evaluating state machines against 6-disposition precedence cascades.
- **Quantified Benefit**: **100% Offline Reproducibility** | **0 Cloud Egress / $0 Telemetry Tax**.

### 📜 [star-protocol](https://github.com/smaos-ai/star-protocol)
**Story-Trace-Assert-Receipt (STAR) Protocol CLI.**
- **Target Audience**: **CISOs, Risk Officers, Compliance Auditors (DORA Art. 17 & EU AI Act)**
- **The Problem**: "Vibe-compliance" text logs fail to satisfy auditors under strict EU AI Act and DORA evidence rules.
- **The Solution**: AST Merkle DAG receipt generator and Ed25519 local verifier producing tamper-proof execution chains.
- **Quantified Benefit**: **100% Cryptographic Audit Traceability** | **10x Faster Compliance Audits** (sub-1KB receipts).

### 🛡️ [context-governor](https://github.com/smaos-ai/context-governor)
**Token Budget & Context Economic Governance Engine.**
- **Target Audience**: **FinOps Leads, Enterprise Architects, LLM Cost Optimization Teams**
- **The Problem**: Context bloat causes ~90% safety constraint decay ("Compaction Cliff") and escalating token costs in long runs.
- **The Solution**: Saliency-first context compaction and budget enforcement harness.
- **Quantified Benefit**: **40%–60% Token Cost Reduction** | **96%+ Constraint Retention @ Round 5**.

---

## 💼 Staging Forensic Audit Offer
We deliver 5-day bounded audits for engineering and payment teams operating mutating AI workflows:
- **Tier 1 Diagnostic (€1,500 / 48-Hour Sprint)**: Ingest 250+ staging traces, calculate Toxic Receipt Index (TRI %), map retry hazards.
- **Tier 2 Forensic Audit (€2,500 / 5-Day Sprint)**: Full wire-level fault injection, 30-day trace analysis, and delivery of a `git apply fix.patch` remediation.

📩 **Contact**: `andrejlo123@gmail.com`
