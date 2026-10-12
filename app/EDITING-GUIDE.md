# Relay eSIM wholesale landing page

## What's included
- Responsive React landing page at `src/routes/index.tsx`
- Custom responsive styles and light motion in `src/styles.css`
- SEO and social metadata in `src/routes/index.tsx` and `src/app-meta.json`
- Validated contact form that prepares an email in the visitor's default email app

## Before launch
1. In `src/routes/index.tsx`, replace `CONTACT_EMAIL = "wholesale@yourcompany.com"` with the real sales inbox. The form uses `mailto:`; it opens the visitor's email app and does not store submissions on a server.
2. Replace the sample Relay brand and copy that does not reflect the actual business.
3. Confirm coverage, markets, integrations, pricing and commercial terms. No unverified numeric claims are used.
4. Replace the hero image URL in `src/routes/index.tsx` and `src/app-meta.json` with an approved brand image if desired.
5. Update the title and description in `src/routes/index.tsx` and `og_title` / `og_description` in `src/app-meta.json`.

## Minor edits
Edit the relevant heading or paragraph directly in `src/routes/index.tsx`. The hero image is the `<img className="hero-image" ... />` element. Use an HTTPS image URL you are permitted to use. Change brand colors in the `--relay-*` variables near the top of `src/styles.css`. Responsive breakpoints are grouped near the end. Animations respect `prefers-reduced-motion`.

## Run locally
From `app/`, install dependencies with Bun and run `bun run dev`. Check with `bun run typecheck` and `bun run build`.

## Production form option
For submissions that work without an email client, connect the handler to a serverless endpoint or form provider. Keep credentials server-side and add privacy/consent copy appropriate to the business.
