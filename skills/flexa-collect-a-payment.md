---
name: Collect a digital-currency payment
description: Create and monitor a Flexa commerce intent to collect a crypto/digital-asset payment from a customer.
api: openapi/flexa-openapi.json
operations:
  - "POST /commerce_intents"
  - "GET /commerce_intents/{id}"
  - "GET /events"
---

# Collect a digital-currency payment with Flexa

Use this skill to collect a payment using a Flexa **commerce intent** — the core resource that represents an attempt to collect a digital-currency payment.

## Authentication
- Authenticate with HTTP Basic Auth: send your Flexa API key as the **username** (no password).
- Base URL: `https://api.flexa.co`.
- Use a `secret_test_`-prefixed key to run against **test mode** (settle in valueless Flexa Credit / CR); use `secret_live_` only after your business is approved.

## Steps

1. **Create the commerce intent** — `POST /commerce_intents`.
   - Provide either your `brand` or `mid`, the `asset` (e.g. `iso4217/USD`), and the `amount` to collect. The response includes an `id` (prefixed `ci_`), a `status`, and a `display_id`.
   - A `201` means it was created; handle `400` (RFC 7807 Bad Request) and `403` (Forbidden — key not enabled for API-only integration).

2. **Present payment to the customer** — the customer fulfills the intent through a Flexa-hosted commerce page or Flexa-enabled wallet app. If you created a `link`, direct them to its `url` (`https://pay.flexa.co/...`).

3. **Confirm completion** — either:
   - Poll `GET /commerce_intents/{id}` and check `status` (e.g. `pending` → completed), or
   - Consume `GET /events` filtered with the `types` query for `commerce_intent.succeeded` / `commerce_intent.canceled`.

## Conventions & error handling
- Errors are **RFC 7807** problem details (`type`, `title`, `status`, `detail`) — see `errors/flexa-problem-types.yml`.
- List responses use a Collection envelope with `has_more`.
- Amounts are decimal strings; timestamps are Unix epoch integers.
- Idempotency: not documented by Flexa — avoid blind retries of `POST /commerce_intents`; instead re-fetch by `id` to reconcile.
