# Kushki (kushki)
Kushki is an Ecuador-headquartered LatAm fintech operating as a regional non-banking acquirer for the Andean and Pacific Alliance markets — Ecuador, Colombia, Peru, Chile, Mexico, and Brazil. The Kushki API unifies card payments, scheduled and one-click subscriptions, bank transfers (PSE, Webpay Transferencia, SPEI, PIX), cash vouchers (OXXO, PagoEfectivo, Boleto), payouts/dispersions, and card-present (Kushki One POS) behind a single REST surface.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Payments, LatAm, Andean Region, Card Payments, Subscriptions, Cash, Bank Transfers, Payouts, PSE, Webpay, SPEI, PIX, OXXO, PagoEfectivo, Fintech, Ecuador, Colombia, Peru, Chile, Mexico, Brazil

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## Environments

| Environment | Base URL |
|---|---|
| Production | `https://api.kushkipagos.com` |
| UAT / Sandbox | `https://api-uat.kushkipagos.com` |
| Staging | `https://api-stg.kushkipagos.com` |

## Authentication

Kushki uses a split-key model. Tokenization runs in the browser or mobile app with a `Public-Merchant-Id`; charges, captures, voids, refunds, subscriptions, and payouts run server-side with a `Private-Merchant-Id`. Never expose the private key in client code.

| Header | Where used | Purpose |
|---|---|---|
| `Public-Merchant-Id` | Browser / mobile SDK | Card tokenization, transfer initialization |
| `Private-Merchant-Id` | Server | Charges, captures, voids, refunds, subscriptions, payouts, branches |

## Regional Rails

| Country | Currencies | Rails |
|---|---|---|
| Ecuador | USD | Card, Cash (Efectivo EC), Transfer, Payout |
| Colombia | COP | Card, PSE, Cash, Payout |
| Peru | PEN, USD | Card, Cash (PagoEfectivo), Transfer, Payout |
| Chile | CLP | Card (Webpay), Webpay OneClick, Webpay Transferencia, Payout |
| Mexico | MXN, USD | Card, SPEI, Cash (OXXO / 7-Eleven), Payout |
| Brazil | BRL | Card, PIX, Boleto, Payout |

## APIs

### Kushki Card Payments API
Charge, void, refund, capture, and pre-authorize card transactions. Cards are tokenized client-side via Kushki.js Hosted Fields or the iOS / Android SDKs.

- [OpenAPI](openapi/kushki-card-payments-api-openapi.yml)
- [JSON Schema — Token](json-schema/kushki-token-schema.json)
- [JSON Schema — Charge](json-schema/kushki-charge-schema.json)
- [JSON-LD](json-ld/kushki-context.jsonld)
- [Naftiko Capability — Tokens](capabilities/card-payments-tokens.yaml)
- [Naftiko Capability — Charges](capabilities/card-payments-charges.yaml)
- [Naftiko Capability — Pre-Authorization](capabilities/card-payments-preauthorization.yaml)
- [Example — Create Card Charge](examples/kushki-create-card-charge-example.json)

### Kushki Subscriptions API
Scheduled and one-click recurring card subscriptions. Monthly, weekly, biweekly, quarterly, and yearly periodicity.

- [OpenAPI](openapi/kushki-subscriptions-api-openapi.yml)
- [JSON Schema — Subscription](json-schema/kushki-subscription-schema.json)
- [Naftiko Capability — Subscriptions](capabilities/subscriptions-subscriptions.yaml)
- [Example — Create Subscription](examples/kushki-create-subscription-example.json)

### Kushki Transfer Payments API
Bank-rail transfers — PSE (Colombia), Webpay Transferencia (Chile), SPEI (Mexico), PIX (Brazil), and direct debit (Ecuador / Peru).

- [OpenAPI](openapi/kushki-transfer-payments-api-openapi.yml)
- [Naftiko Capability — Transfers](capabilities/transfer-payments-transfers.yaml)
- [Example — Initialize Transfer Charge](examples/kushki-init-transfer-charge-example.json)

### Kushki Cash Payments API
Cash vouchers redeemable at OXXO and 7-Eleven (Mexico), PagoEfectivo (Peru), Boleto (Brazil), and Ecuadorean / Colombian correspondent networks.

- [OpenAPI](openapi/kushki-cash-payments-api-openapi.yml)
- [Naftiko Capability — Cash](capabilities/cash-payments-cash.yaml)
- [Example — Create Cash Voucher](examples/kushki-create-cash-voucher-example.json)

### Kushki Payouts API
Disburse funds to bank accounts, cards, and cash pickup via ACH, PSE, SPEI, PIX, Webpay Transferencia, or intrabank rails. Supports single payouts and batches of up to 1000 beneficiaries.

- [OpenAPI](openapi/kushki-payouts-api-openapi.yml)
- [Naftiko Capability — Payouts](capabilities/payouts-payouts.yaml)
- [Example — Initialize Payout](examples/kushki-init-payout-example.json)

### Kushki Card Present API
In-person EMV chip and contactless transactions through Kushki One terminals and the Raw Card Present API.

- [OpenAPI](openapi/kushki-card-present-api-openapi.yml)
- [Naftiko Capability — Terminals](capabilities/card-present-terminals.yaml)

### Kushki Merchants and Branches API
Manage branches (sucursales) and their per-branch configuration — public/private keys, allowed payment methods, country, currency, anti-fraud rules, and webhook URLs.

- [OpenAPI](openapi/kushki-merchants-api-openapi.yml)
- [Naftiko Capability — Branches](capabilities/merchants-branches.yaml)

### Kushki Webhooks
Real-time event notifications for approved, declined, voided, refunded, and captured transactions across every product. Signed JSON payloads with retry and exponential backoff.

- [JSON Schema — Webhook Event](json-schema/kushki-webhook-event-schema.json)
- [Naftiko Capability — Events](capabilities/webhooks-events.yaml)
- [Example — Webhook Event](examples/kushki-webhook-event-example.json)

## SDKs and Plugins

| Type | Repository |
|---|---|
| PHP SDK | [github.com/Kushki/kushki-php](https://github.com/Kushki/kushki-php) |
| Android SDK (Kotlin) | [github.com/Kushki/kushki-android](https://github.com/Kushki/kushki-android) |
| iOS SDK (Swift) | [github.com/Kushki/kushki-ios](https://github.com/Kushki/kushki-ios) |
| iOS SDK — INTEL | [github.com/Kushki/kushki-ios-intel](https://github.com/Kushki/kushki-ios-intel) |
| iOS SDK — ARM | [github.com/Kushki/kushki-ios-arm](https://github.com/Kushki/kushki-ios-arm) |
| WooCommerce | [github.com/Kushki/kushki-woocommerce](https://github.com/Kushki/kushki-woocommerce) |
| Magento | [github.com/Kushki/kushki-magento](https://github.com/Kushki/kushki-magento) |
| PrestaShop | [github.com/Kushki/kushki-prestashop](https://github.com/Kushki/kushki-prestashop) |
| VTEX | [github.com/Kushki/kushki-vtex](https://github.com/Kushki/kushki-vtex) |
| Backend Examples (Node.js) | [github.com/Kushki/kushki-backend-examples](https://github.com/Kushki/kushki-backend-examples) |

## Operations and Commercial Surface

- [Plans and pricing](plans/kushki-plans-pricing.yml) — bespoke MDR per merchant; contact sales for rates.
- [Rate limits](rate-limits/kushki-rate-limits.yml) — per-key throttling, exponential-backoff guidance.
- [FinOps](finops/kushki-finops.yml) — FOCUS-aligned cost model for payments.
- [Vocabulary](vocabulary/kushki-vocabulary.yml) — domain terms, country rails, document types, events.
- [Spectral rules](rules/kushki-rules.yml) — OpenAPI style and conformance enforcement.

## Resources

- [Portal](https://kushkipagos.com/)
- [Documentation](https://docs.kushki.com/)
- [API Reference](https://api-docs.kushkipagos.com/api-reference)
- [Support](https://soporte.kushkipagos.com/)
- [Status Page](https://status.kushkipagos.com/)
- [GitHub Organization](https://github.com/Kushki)
- [UAT Console](https://uat-console.kushkipagos.com/)
- [LinkedIn](https://www.linkedin.com/company/kushki/)
