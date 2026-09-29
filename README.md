# ITKeepers Website V1

A fast, prerendered Astro redesign built around **“Your IT person is a team.”** It preserves the existing ITKeepers navy/cyan palette while making the operating model the main differentiator.

## Local development

```bash
npm install
npm run dev
npm run build
```

Node.js **22.x** is the production runtime target.

## Cloudflare Pages

This repository is configured for Cloudflare Pages.

- Production branch: `main`
- Build command: `npm run build`
- Build output directory: `dist`
- Node.js: `22.x`
- Wrangler Pages output: `./dist`

Cloudflare Pages should be connected to the GitHub repository `jimmynDev/itkeepers-website`. Once Git integration is enabled, every push to `main` should trigger a production build automatically.

## Routes

Home; Managed IT; Microsoft & Cloud; Cybersecurity; Networks & Infrastructure; Backup & Recovery; How We Work; Our Team; Contact; Privacy.

## Design rules

Editorial hierarchy, real operational explanations, no fabricated testimonials or counters, no fake live monitoring, and no stock employees.

## Security

The site is static/prerendered and contains no credentials or client infrastructure data. Security headers are defined in `public/_headers`. See `SECURITY.md` for the hardening baseline.

## Next priorities

Add approved team photography and roles; confirm approved scale evidence; wire a secure server-side contact form; map redirects from the current site; run accessibility/performance/cross-browser QA; copy the approved logo into the repository when its source asset is available; verify production TLS/HSTS and privacy handling.
