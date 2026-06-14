# Pendle

APIs.json 0.19 provider profile for [Pendle](https://www.pendle.finance) — a permissionless yield tokenization protocol that splits yield-bearing assets into Principal Tokens (PT) and Yield Tokens (YT), enabling fixed-yield strategies and yield trading on-chain.

## APIs

| API | Base URL | Description |
|-----|----------|-------------|
| Pendle V2 Core API | `https://api-v2.pendle.finance/core` | 33-endpoint REST API for markets, assets, pricing, limit orders, governance, and user data across all supported chains |
| Pendle Hosted SDK | `https://api-v2.pendle.finance/core` | Transaction-payload builder exposing 13 operations (swaps, liquidity, mint/redeem PT/YT) via a single convert endpoint |

## Supported Chains

Ethereum, Arbitrum, BNB Chain, Base, Mantle, Optimism, Sonic, Berachain, and additional chains enumerated at `GET /v1/chains`.

## Authentication

Bearer token — obtain an API key at `https://api-v2.pendle.finance/dashboard`.

## Rate Limiting

Computing Unit (CU) model. Free tier: 100 CU/min, 200,000 CU/week. Paid plans at $10/$20/$40 per week scale to 500/1,000/2,000 CU/min and 1M/2M/4M CU/week respectively.

## Resources

- [Documentation](https://docs.pendle.finance)
- [API Overview](https://docs.pendle.finance/pendle-v2-dev/Backend/ApiOverview)
- [Hosted SDK Docs](https://docs.pendle.finance/pendle-v2-dev/Backend/HostedSdk)
- [Interactive API Reference](https://api-v2.pendle.finance/core/docs)
- [OpenAPI Spec](https://raw.githubusercontent.com/pendle-finance/documentation/master/static/pendle-dev-docs/openapi/open-api.json)
- [GitHub](https://github.com/pendle-finance)

## Files

- `apis.yml` — APIs.json 0.19 provider profile
- `plans/pendle-plans-pricing.yml` — plan tiers and pricing
- `rate-limits/pendle-rate-limits.yml` — CU-based rate limit details
- `finops/pendle-finops.yml` — FinOps FOCUS-aligned cost model
