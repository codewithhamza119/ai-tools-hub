# AI Tools HuB — Project Backup

> Snapshot of the AI Tools HuB website project as of **2026-10-05**.
> The live site is built and maintained inside Muse (artifact slug: `ai-tools-hub`).
> Public URL: https://muse.ai/s/ai-tools-hub-xpxg6c5suqrsl (serves the last user-approved published version; newer builds are staged until approved).
> This repo backup preserves the full project specification: catalog, pricing, design system, features, and integrations.

## What's here

- `CATALOG.md` — complete product catalog: every plan, regular vs discounted price, duration, warranty, and key terms.
- `SITE-SPEC.md` — design system, page sections, features (AI assistant, languages, cart, checkout), integrations, and change history.
- `assets/` — user-supplied brand/product artwork used on the site (see paths).

## How the site is updated

The website is generated via Muse's artifact system. Every change (products, prices, design, features)
goes through the site builder — there is no manual HTML editing. To update the live site:

1. Tell Muse (Partner) what to change, in any language.
2. Review the staged build via the preview card.
3. Approve publishing to update the public link.

## Tech notes

- Static storefront (English by default, with a client-side Roman Urdu toggle).
- Product data (prices, warranties) is part of the build; keep `CATALOG.md` in sync when prices change.
- Checkout is order-via-WhatsApp: customer pays (Easypaisa / IBAN / Binance), then shares the payment screenshot on WhatsApp.
