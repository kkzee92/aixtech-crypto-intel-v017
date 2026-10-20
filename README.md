# AIxTech Crypto Intel v0.17: Enhanced Paper-Only Trading Information System

Research harness for automated cryptocurrency **information** systems and paper strategy evaluation. Strictly paper-only: no live orders, no exchange secrets, not financial advice.

Builds on previous versions (including kkzee92/aixtech-crypto-intel and zeekiankok92 references).

## v0.17 Enhancements

- Supertrend-style ATR-based trend proxy for Major, RWA, and DeFi strategies.
- Volume delta / imbalance proxy for Large-cap alt and Perpetual carry filters.
- Multi-asset correlation regime detection for portfolio-level risk gates.
- Advanced zero-trust: mutual TLS notes, data lineage tracking, isolation-style anomaly scoring.
- Enhanced data security: residency enforcement, lineage digests, expanded redaction.

## Asset Class Strategies (Enhanced)

| Class | Key Enhancements | Risk Cap |
|-------|------------------|----------|
| Major | Supertrend + prior multi-factor (ADX, Williams, CCI, etc.) | 8% |
| Large-cap alt | Volume delta confirmation on breakouts | 4% |
| Stablecoin | Unchanged depeg alerts | 0% |
| DeFi | Supertrend in calm regimes + volume | 2% |
| Meme | Burst + volume accel | 0.5% |
| L2 | Relative Supertrend excess | 3% |
| RWA | Slow Supertrend + gap halt | 2% |
| Perpetual | Volume delta + funding consistency | 2% |

Full details in docs/.

## Security Architecture

- Zero-trust re-validation on every scan: integrity + lineage + Supertrend consistency.
- Data residency preferred (e.g., SG); cross-border attestation required.
- Hash-chained audit, expanded secret redaction, PDPA tripwire.
- Paper-only PermissionError guards.

## Run (synthetic only)

See previous versions for CLI patterns. All on synthetic fixtures.

**Disclaimer**: Research only. Not investment advice. No live trading.
