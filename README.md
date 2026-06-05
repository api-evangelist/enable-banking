# Enable Banking (enable-banking)

Enable Banking is a Finland-based Open Banking connectivity engine and licensed PSD2 Account Information Service Provider (AISP) regulated by the Finnish Financial Supervisory Authority (FIN-FSA). Headquartered in Espoo, Enable Banking provides a single harmonized API across 2,700+ banks (ASPSPs) in 30 European countries, exposing Account Information Services (AIS) and Payment Initiation Services (PIS), TPP Infrastructure-as-a-Service for licensed Third Party Providers, and an eIDAS-backed JWT authentication model. The platform processes 25M+ API requests monthly across the EEA and maintains 1,000+ ASPSP integrations, serving accounting and ERP platforms, credit risk and KYC providers, wealth managers, and payment service providers including Qred Bank, Fimento, CapitalBox, and iDenfy. Enable Banking is GDPR and DORA compliant with an active PSD3 / FIDA roadmap.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/enable-banking/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/enable-banking/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming

## Tags

- Open Banking
- PSD2
- AISP
- PISP
- Banking
- Financial Services
- Account Aggregation
- Payment Initiation
- Europe
- Nordic
- Finland
- Compliance
- eIDAS
- SCA
- DORA
- GDPR

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Enable Banking API

The Enable Banking API is a single harmonized PSD2 Open Banking API providing Account Information Services (AIS) and Payment Initiation Services (PIS) across 2,700+ banks (ASPSPs) in 30 European countries. The API normalizes user sessions, consent and SCA flows, account details, balances, transactions, and payment initiation behind one REST surface. Authentication uses application-issued JWTs signed with RS256 against an eIDAS-backed certificate registered via the Enable Banking Control Panel. Endpoint groups cover User sessions (/auth, /sessions), Accounts data (/accounts/{account_id}/details, /balances, /transactions), Payments (/payments and /payments/{payment_id}), and Misc (/aspsps, /application).

- **Human URL:** [https://enablebanking.com/docs/api/reference/](https://enablebanking.com/docs/api/reference/)
- **Base URL:** `https://api.enablebanking.com`

#### Tags

- Open Banking
- PSD2
- AISP
- PISP
- Account Information
- Payment Initiation
- Banking
- Aggregation
- Europe
- Nordic

#### Properties

- [Documentation](https://enablebanking.com/docs/)
- [Documentation](https://enablebanking.com/docs/api/reference/)
- [Getting Started](https://enablebanking.com/docs/api/getting-started/)
- [OpenAPI](openapi/enable-banking-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/enable-banking-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/enable-banking-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://enablebanking.com/docs/api/reference/enablebanking-api.yaml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [JSON Schema](json-schema/enable-banking-account-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/enable-banking-transaction-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/enable-banking-payment-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/enable-banking-account-structure.json)
- [JSON-LD](json-ld/enable-banking-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Spectral Rules](rules/enable-banking-rules.yml)
- [Vocabulary](vocabulary/enable-banking-vocabulary.yml)
- [SDK](https://github.com/enablebanking/enablebanking-api-samples/tree/master/python_example)
- [SDK](https://github.com/enablebanking/enablebanking-api-samples/tree/master/js_example)
- [SDK](https://github.com/enablebanking/enablebanking-api-samples/tree/master/go_example)
- [SDK](https://github.com/enablebanking/enablebanking-api-samples/tree/master/cs_example)
- [SDK](https://github.com/enablebanking/enablebanking-api-samples/tree/master/php_example)
- [SDK](https://github.com/enablebanking/enablebanking-api-samples/tree/master/ruby_example)
- [Postman](https://github.com/enablebanking/enablebanking-api-samples/tree/master/postman_example) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [C L I](https://github.com/enablebanking/enablebanking-cli)
- [Tools](https://github.com/enablebanking/open_banking_eidas_broker)
- [GitHub Organization](https://github.com/enablebanking)
- [Control Panel](https://enablebanking.com/cp/)
- [Sandbox](https://tilisy.com)
- [Pricing](https://enablebanking.com/pricing/)
- [Blog](https://enablebanking.com/blog/)
- [Changelog](https://enablebanking.com/changelog/)
- [Portal](https://enablebanking.com)
- [Authentication](https://enablebanking.com/docs/api/reference/#authentication)
- [Plans](plans/enable-banking-plans-pricing.yml)
- [Rate Limits](rate-limits/enable-banking-rate-limits.yml)
- [Fin Ops](finops/enable-banking-finops.yml)
- [Features](undefined)

## Common Properties

- [Portal](https://enablebanking.com)
- [Documentation](https://enablebanking.com/docs/)
- [Getting Started](https://enablebanking.com/docs/api/getting-started/)
- [Documentation](https://enablebanking.com/docs/api/reference/)
- [Blog](https://enablebanking.com/blog/)
- [Changelog](https://enablebanking.com/changelog/)
- [Pricing](https://enablebanking.com/pricing/)
- [About](https://enablebanking.com/about/)
- [Contact Form](https://enablebanking.com/contact/)
- [Console](https://enablebanking.com/cp/)
- [Demo](https://tilisy.com)
- [GitHub Organization](https://github.com/enablebanking)
- [Code Samples](https://github.com/enablebanking/enablebanking-api-samples)
- [C L I](https://github.com/enablebanking/enablebanking-cli)
- [Tools](https://github.com/enablebanking/open_banking_eidas_broker)
- [Tools](https://github.com/enablebanking/psd2-oidc-mock)
- [LinkedIn](https://www.linkedin.com/company/enable-banking/)
- [Plans](plans/enable-banking-plans-pricing.yml)
- [Rate Limits](rate-limits/enable-banking-rate-limits.yml)
- [Fin Ops](finops/enable-banking-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
