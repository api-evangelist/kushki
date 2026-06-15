# Kushki (kushki)

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
