# Webhooks

## Configure Webhook URL
- `POST /webhooks`
- URL must be HTTPS

## Test Delivery
- `POST /webhooks/test`

## Signature Verification
Incoming payloads include:
- `X-XPayr-Signature: sha256=<hmac>`
- `X-XPayr-Event: <event_type>`

Verify HMAC SHA-256 using your webhook secret against the raw request body.

## Core Events
- `payment.pending`
- `payment.processing`
- `payment.completed`
- `payment.failed`
- `payment.expired`

## Recommendation
- Treat webhook delivery as source of truth for payment status transitions.
