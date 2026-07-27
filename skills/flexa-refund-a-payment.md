---
name: Refund a completed payment
description: Issue a refund against a completed Flexa commerce intent and confirm its status.
api: openapi/flexa-openapi.json
operations:
  - "POST /refunds"
  - "GET /refunds/{id}"
  - "GET /commerce_intents/{id}"
---

# Refund a completed payment with Flexa

Use this skill to return value against a completed commerce intent.

## Authentication
- HTTP Basic Auth with your Flexa API key as the username (no password). Base URL `https://api.flexa.co`.
- Use `secret_test_` keys in test mode; `secret_live_` in production.

## Steps

1. **Identify the commerce intent** — you need the `commerce_intent` id (prefixed `ci_`) of the payment to refund. Optionally verify it first with `GET /commerce_intents/{id}` and confirm its `status` and `amount_received`.

2. **Create the refund** — `POST /refunds`.
   - Body: `commerce_intent` (the `ci_...` id), `amount` (decimal string, up to the amount received), and an optional `reason` (e.g. `return`).
   - A `201` returns a `refund` object (id prefixed `refund_`) with a `status`. Handle `400` (Bad Request) and `403` (Forbidden).

3. **Confirm the refund** — `GET /refunds/{id}` and check `status` (e.g. `succeeded`). Handle `404` if the id is unknown.

## Conventions & error handling
- Errors are **RFC 7807** problem details — see `errors/flexa-problem-types.yml`.
- A refund `belongs_to` exactly one commerce intent (via the `commerce_intent` field) — see `data-model/flexa-data-model.yml`.
- Amounts are decimal strings in the intent's `asset`.
