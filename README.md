# single0

Personal homepage for **single0.com** — Singleton YE.
Bilingual (EN / 中文, auto-detects mainland-China IPs via `/cdn-cgi/trace`), fully static.

## Structure
- `public/` — the static site (`index.html`, `styles.css`, `assets/`)
- `wrangler.toml` — Cloudflare Worker config, static-assets only (`[assets] directory = "./public"`)

## Deploy
Deployed on Cloudflare via **Workers Builds** connected to this repo.
Push to `main` → auto `npx wrangler deploy`. Live at https://single0.com
