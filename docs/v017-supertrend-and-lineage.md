# v0.17: Supertrend Proxies, Volume Delta, Multi-Asset Correlation, and Data Lineage

## Strategy Enhancements per Asset Class

- **Major / RWA / DeFi**: Supertrend-style proxy (ATR bands with adaptive multiplier) for trend confirmation. Requires alignment with prior ADX/Williams/CCI stack. Low Supertrend strength reduces size or stands aside.
- **Large-cap alt / Perpetual**: Volume delta proxy (up-volume vs down-volume imbalance over window) required for breakout or carry confirmation. Filters weak participation.
- **All**: Multi-asset correlation regime (synthetic pairwise proxy) for portfolio risk gate: high correlation stress reduces aggregate paper size.
- Volatility scaling, class caps, stress stand-aside retained.

## Cyber / Data Security

- Data lineage: every fixture and series has a chain of custody digest (source, transform, hash).
- Advanced anomaly: isolation-style scoring on residuals + Supertrend/price divergence.
- Zero-trust: re-validate integrity, lineage, Supertrend consistency, residency attestation.
- Mutual TLS and external KMS notes for production research environments.
- Expanded redaction patterns; no secrets in tree.
- Continued hash-chained audits, PDPA, gitleaks, paper-only.

Still strictly research, paper-only. No live execution.
