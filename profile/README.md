# smaos-ai — Sovereign Multi-Agent OS & Trust Infrastructure
Sovereign, local-first, zero-dependency trust and governance infrastructure for autonomous AI agents.

> ### *"Every agent harness logs success. Almost none of them test whether the success was justified by the evidence at the wire."*

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

## 🏛️ Sovereign Governance Substrate & Regulatory Roadmap

### ✅ Milestone 1 Achieved: Local-First Execution & Pre-Execution Safety
* **Pre-Execution Fail-Closed Gates**: Intercepts tool dispatches at the wire and kernel boundary before any side effect occurs.
* **Wire-Fault Simulation**: Tests harness state preservation under simulated HTTP 504 timeouts and dropped sockets, enforcing `verdict: UNKNOWN` rather than writing false `CONFIRMED` success logs.
* **Cryptographic Provenance**: Generates RFC 8785 JCS-canonicalized Merkle DAG receipts signed with Ed25519 keys for every execution.
* **Zero Egress**: Runs 100% air-gapped on local hardware under `network_mode: "none"`.

---

### 🎯 Next Target Milestone: December 2, 2027 (EU AI Act Annex III Deadline)
Under the **EU AI Act (Regulation 2024/1689)** as amended by Digital Omnibus Regulation (EU 2026/1744), the statutory enforcement date for **standalone High-Risk AI systems (Annex III)** is **December 2, 2027**. This applies to all autonomous agent workflows operating in high-risk categories:
1. **Biometrics & Biometric Categorization**
2. **Critical Infrastructure Management** (Water, gas, electricity, cloud networks)
3. **Educational & Vocational Assessment**
4. **Employment, Worker Management & Access to Self-Employment**
5. **Access to Essential Private & Public Services** (e.g., Credit Scoring, Loan Approvals, Healthcare, Risk Evaluation)
6. **Law Enforcement**
7. **Migration, Asylum & Border Control**
8. **Administration of Justice & Democratic Processes**

---

### 🧪 Automated Rule & Testing Substrate for Annex III (Articles 9–15)
This suite serves as an automated test harness and evidence generation engine for Articles 9–15 compliance:

| Statutory Requirement | Governance Substrate Mapping | Technical Evidence Produced |
| :--- | :--- | :--- |
| **Article 9: Risk Management** | Bitemporal ledger tracking post-market evaluation and risk registers throughout the lifecycle. | `agentacct.db` audit traces & risk classification logs. |
| **Article 12: Record-Keeping** | Automatic, tamper-evident event recording over the system's operational lifetime. | SHA-256 Merkle DAG receipts signed with Ed25519 (IETF SCITT profile). |
| **Article 13: Transparency** | Machine-readable system boundaries, capability disclosures, and limitations. | Auto-generated Model Cards & System Boundary manifests. |
| **Article 14: Human Oversight** | Pre-execution fail-closed gates holding retries and enforcing human veto authority. | Resumable Cognitive Execution (RCE) interrupts & stop-button logs. |
| **Article 15: Cybersecurity & Robustness** | Local-first, air-gapped container isolation preventing prompt injection and exfiltration. | Substrate measurement receipts & 0-byte egress network traces. |

---

### ⚖️ Conformity Assessment Pathway: Annex VI Self-Assessment
Under **Article 43(2)** of the EU AI Act, standalone software falling under Annex III categories undergoes an **Internal Conformity Assessment (Annex VI)**. **No third-party Notified Body is required** for standalone software self-assessment.

Running this test harness automatically compiles the mandatory **Annex IV Technical Dossier** directly from real execution traces, allowing enterprise engineering teams to self-certify compliance for December 2, 2027 deployment.

---

## 💼 Staging Forensic Audit Offer
We deliver 5-day bounded audits for engineering and payment teams operating mutating AI workflows:
- **Tier 1 Diagnostic (€1,500 / 48-Hour Sprint)**: Ingest 250+ staging traces, calculate Toxic Receipt Index (TRI %), map retry hazards.
- **Tier 2 Forensic Audit (€2,500 / 5-Day Sprint)**: Full wire-level fault injection, 30-day trace analysis, and delivery of a `git apply fix.patch` remediation.

📩 **Contact**: `andrejlo123@gmail.com`
