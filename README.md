<div align="center">
  <a href="https://xpayr.com">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://xpayr.com/public/images/xpayr-logo-white.png" />
      <source media="(prefers-color-scheme: light)" srcset="https://xpayr.com/public/images/xpayr-logo-black.png" />
      <img src="https://xpayr.com/public/images/xpayr-logo-white.png" alt="XPayr Official Logo" width="220" />
    </picture>
  </a>
  <p>
    <a href="https://xpayr.com"><img src="https://xpayr.com/partner-badge.php?type=powered_by&theme=dark" alt="Powered by XPayr" height="28" /></a>
    <a href="https://mcp.xpayr.com"><img src="https://img.shields.io/badge/MCP_Portal-mcp.xpayr.com-029bfd?style=for-the-badge" alt="XPayr MCP Portal" height="28" /></a>
    <a href="https://docs.xpayr.com"><img src="https://img.shields.io/badge/Docs-docs.xpayr.com-10b981?style=for-the-badge" alt="XPayr Docs" height="28" /></a>
    <a href="https://www.npmjs.com/package/@xpayr/mcp-server"><img src="https://img.shields.io/npm/v/@xpayr/mcp-server?style=for-the-badge&color=cb3837&label=MCP%20NPM" alt="NPM @xpayr/mcp-server" height="28" /></a>
  </p>
  <p>
    <a href="https://xpayr.com"><b>Official Website</b></a> •
    <a href="https://mcp.xpayr.com"><b>AI &amp; MCP Portal (21 Tools)</b></a> •
    <a href="https://docs.xpayr.com"><b>Developer Docs</b></a> •
    <a href="https://xpayr.com/developers"><b>Developer Hub</b></a> •
    <a href="https://xpayr.com/tools/crypto-payment-fee-calculator"><b>0.5% Fee Calculator</b></a>
  </p>
</div>

---

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
