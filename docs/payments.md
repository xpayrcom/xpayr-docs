# Payments

## Create Payment Session
`POST /payments`

Required fields:
- `amount`
- `currency`
- `network`

Example body:
```json
{
  "amount": 9.99,
  "currency": "USDC",
  "network": "base",
  "metadata": {
    "order_id": "ORDER-1001"
  },
  "success_url": "https://example.com/success",
  "cancel_url": "https://example.com/cancel"
}
```

## Get Payment Session
`GET /payments/{id}`

## List Payment Sessions
`GET /payments?page=1&limit=25`

## Notes
- Persist `id` and `payment_url` from create response.
- Use webhook events to finalize order state.
