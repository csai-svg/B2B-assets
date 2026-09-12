# B2B-assets

Shared, canonical product photo host for the Optum and Deloitte B2B
merchandise storefronts (`csai-svg/optum-B2B`, `csai-svg/deloitte-B2B`).

Published via GitHub Pages. Both storefronts' master sheet (`Image URL`
column) points here instead of Google Drive, so images get real cache
headers and don't hit Drive's rate limits — see each site's
`apps-script-feed/Code.gs` and `scripts/migrate_images.py`.

- `img/<SKU>.webp` — one WebP per product, max 1000px wide, quality 80.
- `manifest.json` — `{sku: canonical_url}`, used to bulk-update the sheet.

Regenerate/update via `optum-B2B/scripts/migrate_images.py --out <this repo>`.
