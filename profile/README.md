# SMAOS

## Agent Evidence Integrity for Consequential AI Workflows

SMAOS develops open benchmarks and evidence protocols for evaluating whether
AI-agent workflows distinguish attempted actions from confirmed external effects.

## Governance boundary

### Capability is not authority

Agents may draft, calculate, and simulate. Human operators remain responsible
for authorizing consequential actions within the applicable workflow controls.

## AEIB reference container

AEIB v0.1.0 is an offline benchmark over synthetic JSONL scenarios. The
reference container uses `network_mode: "none"` and requires no prompts,
source code, credentials, or cloud services.

This describes the reference configuration only. It does not establish the
security or privacy properties of every host, plugin, runtime, or invocation.

## AEIB

AEIB tests:

- disposition precedence;
- preservation of `UNKNOWN` outcomes;
- handling of refusal and conflicting evidence;
- missing and invalid evidence;
- deterministic offline execution.

The six dispositions are:

```text
INVALID_INPUT
MISSING_EVIDENCE
CONFLICT
REFUSED
CONFIRMED
UNKNOWN
```

Run the benchmark:

```bash
git clone --branch v0.1.0 https://github.com/smaos-ai/aeib.git aeib
cd aeib
docker compose run --rm benchmark
```

See `SPEC.md`, `LIMITATIONS.md`, and
`PUBLIC_REPRODUCTION_REPORT.md` for the frozen contract, limitations, and
reported reproduction procedure.

## Attestation scope

Separate SMAOS tooling may generate signed receipts for declared local
artifact sets. Such receipts authenticate the represented artifacts relative
to a signing key. They do not independently establish external-system truth,
source completeness, authority, or regulatory compliance.

## Related work

AEIB is the only component required to run this repository. Other SMAOS
components and commercial services are separate projects and are not required
for AEIB execution. Commercial evaluation services, if available, are scoped separately from this repository.

## Regulatory scope

This repository does not assess applicability of DORA or the EU AI Act,
determine compliance, classify incidents, or provide legal advice. References
to logging, human oversight, or ICT third-party risk are contextual only.

## Limitations

SMAOS and AEIB do not claim to:

- prove production security;
- guarantee privacy across every host or integration;
- establish external-system or ledger truth;
- replace a GRC or incident-management system;
- certify DORA or EU AI Act compliance;
- provide a legal opinion;
- guarantee safe behavior for all agent architectures.
