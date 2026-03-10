# Authentication

XPayr API v1 uses Bearer authentication for protected endpoints.

## Header Format
```http
Authorization: Bearer sk_test_your_key
```

## Key Types
- `sk_test_...` for test mode
- `sk_live_...` for live mode

## Example
```bash
curl -X GET "https://xpayr.com/api/v1/me" \
  -H "Authorization: Bearer $XPAYR_SECRET_KEY"
```

## Best Practices
- Store keys in environment variables, not source code.
- Rotate keys periodically.
- Use separate keys for staging and production.
