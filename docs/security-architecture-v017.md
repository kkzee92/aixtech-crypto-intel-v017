# Enhanced Security Architecture v0.17

## Zero-Trust Data Plane
- Every scan: series integrity digest + data lineage chain + Supertrend consistency check + source attestation.
- Residency: prefer declared region; cross-border requires explicit attestation.
- Anomaly scoring: residual isolation proxy + directional inconsistency (Supertrend vs slope).

## Controls
- Paper-only: PermissionError on any live mode.
- No trader/withdrawal roles. Key separation.
- Expanded secret redaction (keys, seeds, tokens, PEM, base58, WIF, mnemonics).
- Hash-chained audit log.
- PDPA tripwire, gitleaks CI, Ruff/Bandit-style lint.
- Recommended: AES-256 at rest, TLS 1.3 in transit, external KMS/HSM, mutual TLS for research pipelines.

No live connectors. Research only.
