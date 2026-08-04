# Kushki (kushki)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Kushki is an Ecuador-headquartered LatAm fintech operating as a regional non-banking acquirer for the Andean and Pacific Alliance markets — Ecuador, Colombia, Peru, Chile, Mexico, and Brazil. The Kushki API unifies card payments, scheduled and one-click subscriptions, bank transfers (PSE, Webpay Transferencia, SPEI, PIX), cash vouchers (OXXO, PagoEfectivo, Boleto), payouts/dispersions, and card-present (Kushki One POS) behind a single REST surface. Authentication is split across a Public-Merchant-Id (used in the browser to tokenize cards) and a Private-Merchant-Id (used server-side to charge). PCI DSS Level 1, 3DS 2.0, multi-layer anti-fraud, hosted fields, Kajita payment forms, Smartlinks, and e-commerce plugins (Shopify, VTEX, WooCommerce, Magento, PrestaShop) round out the platform.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/apis.yml)

## Scope

- **Position:** Producing
- **Access:** 3rd-Party

## Tags

- Payments
- LatAm
- Andean Region
- Card Payments
- Subscriptions
- Cash
- Bank Transfers
- Payouts
- PSE
- Webpay
- SPEI
- PIX
- OXXO
- PagoEfectivo
- Fintech
- Ecuador
- Colombia
- Peru
- Chile
- Mexico
- Brazil

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### Kushki Card Payments API

Charge, void, refund, capture, and pre-authorize card transactions via the Kushki Card REST API. Card numbers are tokenized client-side (Kushki.js Hosted Fields or mobile SDKs) so PAN never touches the merchant server. One-step and two-step (auth/capture) flows, deferred payments with months and rate-of-interest, partial refunds, and 3DS 2.0 authentication are supported across Ecuador, Colombia, Peru, Chile, Mexico, and Brazil.

- **Human URL:** [https://docs.kushki.com/](https://docs.kushki.com/)
- **Base URL:** `https://api.kushkipagos.com`

#### Tags

- Card Payments
- Payments
- Tokenization
- 3DS
- Refunds
- Captures

#### Properties

- [Documentation](https://docs.kushki.com/)
- [API Reference](https://api-docs.kushkipagos.com/api-reference)
- [OpenAPI](openapi/kushki-card-payments-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kushki-card-payments-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kushki-card-payments-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/kushki-charge-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/kushki-token-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/kushki-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Kushki Subscriptions API

Create, update, retrieve, charge, and cancel scheduled card subscriptions and one-click recurring payments. Plans support monthly, weekly, daily, biweekly, quarterly, and yearly periodicity, fixed or variable amounts, start/end dates, contact details, and Webpay OneClick on the Chile rail.

- **Human URL:** [https://docs.kushki.com/](https://docs.kushki.com/)
- **Base URL:** `https://api.kushkipagos.com`

#### Tags

- Subscriptions
- Recurring Payments
- Payments
- One Click

#### Properties

- [Documentation](https://docs.kushki.com/)
- [OpenAPI](openapi/kushki-subscriptions-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kushki-subscriptions-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kushki-subscriptions-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/kushki-subscription-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Kushki Transfer Payments API

Accept bank-rail transfers across LatAm — PSE in Colombia, Webpay Transferencia in Chile, SPEI in Mexico, PIX in Brazil, and direct debit in Ecuador and Peru. Initiate the charge, return a redirect/QR for the payer, and receive webhook confirmation when the bank settles.

- **Human URL:** [https://docs.kushki.com/](https://docs.kushki.com/)
- **Base URL:** `https://api.kushkipagos.com`

#### Tags

- Bank Transfers
- Payments
- PSE
- Webpay
- PIX
- SPEI

#### Properties

- [Documentation](https://docs.kushki.com/)
- [OpenAPI](openapi/kushki-transfer-payments-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kushki-transfer-payments-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kushki-transfer-payments-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kushki Cash Payments API

Generate cash-payment vouchers redeemable at authorized retail networks — OXXO and 7-Eleven in Mexico, PagoEfectivo in Peru, Boleto in Brazil, Western Union and PagoFacil in Argentina, plus Ecuadorean and Colombian correspondent networks. Returns a barcode/reference plus expiry date.

- **Human URL:** [https://docs.kushki.com/](https://docs.kushki.com/)
- **Base URL:** `https://api.kushkipagos.com`

#### Tags

- Cash
- Payments
- Vouchers
- OXXO
- PagoEfectivo
- Boleto

#### Properties

- [Documentation](https://docs.kushki.com/)
- [OpenAPI](openapi/kushki-cash-payments-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kushki-cash-payments-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kushki-cash-payments-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kushki Payouts API

Disburse funds to suppliers, partners, payroll, marketplace sellers, and refunds via bank transfer, card push, or cash pickup. Supports same-day and standard rails, batch upload, and country-specific compliance metadata (RUT, RFC, CURP, RUC, CPF).

- **Human URL:** [https://docs.kushki.com/](https://docs.kushki.com/)
- **Base URL:** `https://api.kushkipagos.com`

#### Tags

- Payouts
- Dispersions
- Bank Transfers
- Mass Payments

#### Properties

- [Documentation](https://docs.kushki.com/)
- [OpenAPI](openapi/kushki-payouts-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kushki-payouts-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kushki-payouts-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kushki Card Present API

Process in-person EMV chip and contactless transactions through Kushki One terminals and the Raw Card Present API. Includes pairing, terminal management, sale, void, settlement, and an encryption envelope so payment data is sealed end-to-end from the PIN pad.

- **Human URL:** [https://docs.kushki.com/](https://docs.kushki.com/)
- **Base URL:** `https://api.kushkipagos.com`

#### Tags

- POS
- Card Present
- EMV
- Kushki One
- In Person

#### Properties

- [Documentation](https://docs.kushki.com/)
- [OpenAPI](openapi/kushki-card-present-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kushki-card-present-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kushki-card-present-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kushki Webhooks

Real-time event notifications for approved, declined, voided, refunded, and captured transactions across every product (card, transfer, cash, subscription, payout). Webhooks ship a signed JSON payload, include retry with exponential backoff, and target merchant-configured endpoints managed in the Kushki Console.

- **Human URL:** [https://docs.kushki.com/](https://docs.kushki.com/)

#### Tags

- Webhooks
- Notifications
- Events

#### Properties

- [Documentation](https://docs.kushki.com/)
- [JSON Schema](json-schema/kushki-webhook-event-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Postman Collection](collections/kushki-card-payments-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kushki-card-payments-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kushki-card-present-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kushki-card-present-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kushki-cash-payments-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kushki-cash-payments-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kushki-merchants-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kushki-merchants-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kushki-payouts-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kushki-payouts-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kushki-subscriptions-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kushki-subscriptions-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kushki-transfer-payments-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kushki-transfer-payments-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kushki Merchants and Branches API

Manage merchant branches (sucursales) and their per-branch configuration — public/private keys, allowed payment methods, country, currency, anti-fraud rules, and webhook URLs. Used by marketplaces, franchise networks, and aggregators that need to onboard sub-merchants programmatically.

- **Human URL:** [https://docs.kushki.com/](https://docs.kushki.com/)
- **Base URL:** `https://api.kushkipagos.com`

#### Tags

- Merchants
- Branches
- Administration
- Configuration

#### Properties

- [Documentation](https://docs.kushki.com/)
- [OpenAPI](openapi/kushki-merchants-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kushki-merchants-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kushki-merchants-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://kushkipagos.com/)
- [Documentation](https://docs.kushki.com/)
- [API Reference](https://api-docs.kushkipagos.com/api-reference)
- [Getting Started](https://docs.kushki.com/)
- [Support](https://soporte.kushkipagos.com/)
- [Status Page](https://status.kushkipagos.com/)
- [GitHub Organization](https://github.com/Kushki)
- [SDK](https://github.com/Kushki/kushki-php)
- [SDK](https://github.com/Kushki/kushki-android)
- [SDK](https://github.com/Kushki/kushki-ios)
- [SDK](https://github.com/Kushki/kushki-ios-intel)
- [SDK](https://github.com/Kushki/kushki-ios-arm)
- [Plugin](https://github.com/Kushki/kushki-woocommerce)
- [Plugin](https://github.com/Kushki/kushki-magento)
- [Plugin](https://github.com/Kushki/kushki-prestashop)
- [Plugin](https://github.com/Kushki/kushki-vtex)
- [Samples](https://github.com/Kushki/kushki-backend-examples)
- [Samples](https://github.com/Kushki/kushki-demo-php)
- [Docker](https://github.com/Kushki/kushki-docker)
- [Console](https://uat-console.kushkipagos.com/)
- [Console](https://console.kushkipagos.com/)
- [LinkedIn](https://www.linkedin.com/company/kushki/)
- [Twitter](https://twitter.com/kushkipagos)
- [Authentication](https://docs.kushki.com/)
- [Environments](undefined)
- [Regions](undefined)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Plans](plans/kushki-plans-pricing.yml)
- [Rate Limits](rate-limits/kushki-rate-limits.yml)
- [Fin Ops](finops/kushki-finops.yml)
- [Vocabulary](vocabulary/kushki-vocabulary.yml)
- [Spectral Rules](rules/kushki-rules.yml)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
