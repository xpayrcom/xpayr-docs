# XPayr Docs

Official public documentation assets for XPayr merchant integrations.

## Scope
This repository is documentation-only and intentionally excludes:
- production backend source code
- merchant/admin panel internals
- database dumps, logs, credentials, and secrets

## Contents
- `postman/` Postman collection and environment for API testing
- `docs/` integration guides (auth, payments, webhooks)
- `guides/` advanced flows such as Agent Commerce mode

## Quick Start
1. Import:
   - `postman/xpayr_gateway_v1.postman_collection.json`
   - `postman/xpayr_gateway_v1.postman_environment.json`
2. Set `bearer_token` to your `sk_test_...` or `sk_live_...` key.
3. Start with `GET /health`, then `POST /payments`.

## Base URL
- Production default: `https://xpayr.com/api/v1`
- Your deployment can use a different base URL if configured.

## Safety
Before each release, run:
```bash
./scripts/scan-sensitive.sh
```

## License
All rights reserved unless a separate license file is added later.
