# Enable Banking (enable-banking)

Enable Banking is a Finland-based Open Banking connectivity engine and licensed PSD2 Account Information Service Provider (AISP) regulated by the Finnish Financial Supervisory Authority (FIN-FSA). Headquartered in Espoo, Enable Banking provides a single harmonized API across 2,700+ banks (ASPSPs) in 30 European countries, exposing Account Information Services (AIS) and Payment Initiation Services (PIS), TPP Infrastructure-as-a-Service for licensed Third Party Providers, and an eIDAS-backed JWT authentication model. The platform processes 25M+ API requests monthly across the EEA and maintains 1,000+ ASPSP integrations.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/enable-banking/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Open Banking, PSD2, AISP, PISP, Banking, Financial Services, Account Aggregation, Payment Initiation, Europe, Nordic, Finland, Compliance, eIDAS, SCA, DORA, GDPR

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## At a Glance

| Attribute | Value |
|---|---|
| HQ | Espoo, Finland |
| Regulator | Finnish Financial Supervisory Authority (FIN-FSA) |
| Licence | PSD2 AISP (passported across the EEA) |
| ASPSP coverage | 2,700+ banks across 30 EEA countries |
| Volume | 25M+ API requests / month |
| Production base URL | `https://api.enablebanking.com` |
| Sandbox / legacy URL | `https://api.tilisy.com` (deprecated) |
| Auth | Application JWT (RS256, eIDAS certificate, 24h max TTL) + PSU SCA at ASPSP |
| OpenAPI | 3.1.0, published at `enablebanking.com/docs/api/reference/enablebanking-api.yaml` |
| Tier | Tier-1 (real OpenAPI, full SDK samples, public docs, real CLI) |

## APIs

### Enable Banking API

The single harmonized PSD2 API for AIS and PIS across 2,700+ European ASPSPs. Four endpoint groups: User sessions, Accounts data, Payments, and Misc.

**Human URL:** [https://enablebanking.com/docs/api/reference/](https://enablebanking.com/docs/api/reference/)

**Base URL:** `https://api.enablebanking.com`

- [Documentation — Reference](https://enablebanking.com/docs/api/reference/)
- [Documentation — Getting Started](https://enablebanking.com/docs/api/getting-started/)
- [OpenAPI (local)](openapi/enable-banking-api-openapi.yml)
- [OpenAPI (upstream)](https://enablebanking.com/docs/api/reference/enablebanking-api.yaml)
- [JSON Schema — Account](json-schema/enable-banking-account-schema.json)
- [JSON Schema — Transaction](json-schema/enable-banking-transaction-schema.json)
- [JSON Schema — Payment](json-schema/enable-banking-payment-schema.json)
- [JSON Structure — Account](json-structure/enable-banking-account-structure.json)
- [JSON-LD Context](json-ld/enable-banking-context.jsonld)
- [Spectral Rules](rules/enable-banking-rules.yml)
- [Vocabulary](vocabulary/enable-banking-vocabulary.yml)
- [Naftiko Capability — User Sessions](capabilities/sessions-user-sessions.yaml)
- [Naftiko Capability — Accounts Data](capabilities/accounts-accounts-data.yaml)
- [Naftiko Capability — Payments](capabilities/payments-payments.yaml)
- [Naftiko Capability — ASPSPs and Application](capabilities/aspsps-misc.yaml)
- [Naftiko Capability — Open Banking Workflow](capabilities/open-banking.yaml)
- [Example — Start Authorization](examples/enable-banking-start-authorization-example.json)
- [Example — Get Account Transactions](examples/enable-banking-get-account-transactions-example.json)
- [Example — Create Payment](examples/enable-banking-create-payment-example.json)

#### Endpoint groups

| Tag | Path(s) | Purpose |
|---|---|---|
| User sessions | `POST /auth`, `POST /sessions`, `GET/DELETE /sessions/{session_id}` | Begin PSU authorization, exchange code for session, manage consent. |
| Accounts data | `GET /accounts/{account_id}/details`, `/balances`, `/transactions`, `/transactions/{transaction_id}` | AIS — account details, balances, transactions (up to 12 months). |
| Payments | `POST /payments`, `GET/DELETE /payments/{payment_id}`, `GET /payments/{payment_id}/transactions/{transaction_id}` | PIS — initiate, status, cancel, settled-transaction lookup. |
| Misc | `GET /aspsps`, `GET /application` | ASPSP directory and application metadata. |

## SDKs and Tooling

| Resource | Type | Repo |
|---|---|---|
| `enablebanking-api-samples` | Multi-language code samples (C#, Go, JS, PHP, Python, Ruby, Postman) | [GitHub](https://github.com/enablebanking/enablebanking-api-samples) |
| `enablebanking-cli` | Command-line client for the API and Control Panel | [GitHub](https://github.com/enablebanking/enablebanking-cli) |
| `open_banking_eidas_broker` | Microservice for eIDAS-signed mTLS requests to ASPSPs | [GitHub](https://github.com/enablebanking/open_banking_eidas_broker) |
| `psd2-oidc-mock` | Mock OIDC provider for ASPSP authentication testing | [GitHub](https://github.com/enablebanking/psd2-oidc-mock) |
| `mock-auth-ui` | Mock ASPSP consent UI for local development | [GitHub](https://github.com/enablebanking/mock-auth-ui) |

## Plans, Rate Limits, and FinOps

- [Plans / Pricing](plans/enable-banking-plans-pricing.yml) — Sandbox is free; Production and TPP-IaaS are contract-priced.
- [Rate Limits](rate-limits/enable-banking-rate-limits.yml) — Application JWT 24h max TTL; AIS EBA RTS 4×/day non-PSU-present; 180-day consent validity; PSU-present 5-minute window.
- [FinOps](finops/enable-banking-finops.yml) — FOCUS 1.0 mapping with allocation by ASPSP country, endpoint tag, and PSU type.

## Regulatory Posture

- PSD2 AISP licensed under FIN-FSA, passported across the EEA.
- GDPR compliant.
- DORA (Digital Operational Resilience Act) compliant.
- Active PSD3 / FIDA readiness roadmap.
- eIDAS certificate enrollment via Enable Banking Control Panel; supports QWAC/QSEAL where required by ASPSPs.

## Maintainers

- **Kin Lane** — Founder, API Evangelist — [apievangelist.com](https://apievangelist.com)
