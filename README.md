# Kushki

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
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

**Areas:** Payments · Latin America · Andean Region · Card Payments · Subscription · Cash · Bank Transfers · Payouts · PSE · Webpay · SPEI · Pix

## Kushki on APIs.io

Everything profiled for Kushki is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/kushki/](https://apis.io/providers/kushki/)** — or go straight to one of the APIs or properties below.

### APIs (12)

- [Kushki Subscriptions API](https://apis.io/apis/kushki/kushki-subscriptions-api/) — Create, update, retrieve, charge, and cancel scheduled card subscriptions and one-click recurring payments. Plans support monthly, weekly, daily, biweekly,…
- [Kushki Payouts API](https://apis.io/apis/kushki/kushki-payouts-api/) — Disburse funds to suppliers, partners, payroll, marketplace sellers, and refunds via bank transfer, card push, or cash pickup. Supports same-day and…
- [Kushki Webhooks](https://apis.io/apis/kushki/kushki-webhooks/) — Real-time event notifications for approved, declined, voided, refunded, and captured transactions across every product (card, transfer, cash, subscription,…
- [Kushki Branches API](https://apis.io/apis/kushki/kushki-branches-api/) — Branch / sucursal management
- [Kushki Card Present Charges API](https://apis.io/apis/kushki/kushki-card-present-charges-api/) — Sale, void, and settlement for card-present
- [Kushki Cash API](https://apis.io/apis/kushki/kushki-cash-api/) — Cash voucher generation and lookup
- [Kushki Charges API](https://apis.io/apis/kushki/kushki-charges-api/) — Direct charge against a previously created card token
- [Kushki Pre-Authorization API](https://apis.io/apis/kushki/kushki-pre-authorization-api/) — Two-step authorize + capture flow
- [Kushki Terminals API](https://apis.io/apis/kushki/kushki-terminals-api/) — Kushki One terminal management
- [Kushki Tokens API](https://apis.io/apis/kushki/kushki-tokens-api/) — Card tokenization (client-side via Kushki.js, returns a one-time transactionToken)
- [Kushki Transfer API](https://apis.io/apis/kushki/kushki-transfer-api/) — Bank-rail transfer charges
- [Kushki Voids and Refunds API](https://apis.io/apis/kushki/kushki-voids-and-refunds-api/) — Void or refund a previously captured charge

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Kushki Agentic Access](https://apis.io/agentic-access/kushki/kushki-agentic-access/)

#### JSON Schema (4)

The data models the API reads and writes.

- [Kushki Charge](https://apis.io/schemas/kushki/kushki-charge/)
- [Kushki Subscription](https://apis.io/schemas/kushki/kushki-subscription/)
- [Kushki Card Token](https://apis.io/schemas/kushki/kushki-token/)
- [Kushki Webhook Event](https://apis.io/schemas/kushki/kushki-webhook-event/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Kushki Context](https://apis.io/jsonld/kushki/kushki-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Kushki Vocabulary](https://apis.io/vocabularies/kushki/kushki-vocabulary/)

#### Examples (6)

Example requests and responses.

- [Kushki Create Card Charge Example](https://apis.io/examples/kushki/kushki-create-card-charge-example/)
- [Kushki Create Cash Voucher Example](https://apis.io/examples/kushki/kushki-create-cash-voucher-example/)
- [Kushki Create Subscription Example](https://apis.io/examples/kushki/kushki-create-subscription-example/)
- [Kushki Init Payout Example](https://apis.io/examples/kushki/kushki-init-payout-example/)
- [Kushki Init Transfer Charge Example](https://apis.io/examples/kushki/kushki-init-transfer-charge-example/)
- [Kushki Webhook Event Example](https://apis.io/examples/kushki/kushki-webhook-event-example/)

#### Collections (16)

Postman and Open Collection request collections.

- [Kushki Card Payments Branches API](https://apis.io/collections/kushki/open-kushki-branches-api/)
- [Kushki Card Payments API](https://apis.io/collections/kushki/open-kushki-card-payments-api/)
- [Kushki Card Present API](https://apis.io/collections/kushki/open-kushki-card-present-api/)
- [Kushki Card Payments Branches Card Present Charges API](https://apis.io/collections/kushki/open-kushki-card-present-charges-api/)
- [Kushki Card Payments Branches Cash API](https://apis.io/collections/kushki/open-kushki-cash-api/)
- [Kushki Cash Payments API](https://apis.io/collections/kushki/open-kushki-cash-payments-api/)
- [Kushki Card Payments Branches Charges API](https://apis.io/collections/kushki/open-kushki-charges-api/)
- [Kushki Merchants and Branches API](https://apis.io/collections/kushki/open-kushki-merchants-api/)
- [Kushki Card Payments Branches Payouts API](https://apis.io/collections/kushki/open-kushki-payouts-api/)
- [Kushki Card Payments Branches Pre-Authorization API](https://apis.io/collections/kushki/open-kushki-pre-authorization-api/)
- [Kushki Card Payments Branches Subscriptions API](https://apis.io/collections/kushki/open-kushki-subscriptions-api/)
- [Kushki Card Payments Branches Terminals API](https://apis.io/collections/kushki/open-kushki-terminals-api/)
- [Kushki Card Payments Branches Tokens API](https://apis.io/collections/kushki/open-kushki-tokens-api/)
- [Kushki Card Payments Branches Transfer API](https://apis.io/collections/kushki/open-kushki-transfer-api/)
- [Kushki Transfer Payments API](https://apis.io/collections/kushki/open-kushki-transfer-payments-api/)
- [Kushki Card Payments Branches Voids and Refunds API](https://apis.io/collections/kushki/open-kushki-voids-and-refunds-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Kushki — jsonschema rules](https://apis.io/rules/kushki/kushki-jsonschema-spectral-rules/)
- [Kushki API Rules](https://apis.io/rules/kushki/kushki-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Kushki Authentication](https://apis.io/security/kushki/kushki-authentication/)
- [Kushki Domain Security](https://apis.io/security/kushki/kushki-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Kushki Plans Pricing](https://apis.io/plans/kushki/kushki-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Kushki Rate Limits](https://apis.io/rate-limits/kushki/kushki-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Kushki Finops](https://apis.io/finops/kushki/kushki-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.kushkipagos.com/)
- [Documentation](https://docs.kushki.com/)
- [Getting started](https://docs.kushki.com/)
- [API reference](https://api-docs.kushkipagos.com/api-reference)
- [Support](https://soporte.kushkipagos.com/)
- [Blog](https://www.kushkipagos.com/blog)
- [GitHub](https://github.com/Kushki)
- [Status](https://status.kushkipagos.com/)

## API Evangelist rating

**Kin Score 44.8** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 62.5 |
| Contract quality | 64.3 |
| Contract governance | 27.3 |
| Operational transparency | 18.4 |
| Developer ergonomics | 75.0 |
| Access clarity | 15.8 |

**Agent readiness 23.0** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | partial |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 15.2** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/kushki/](https://apis.io/providers/kushki/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Kushki: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/kushki/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
