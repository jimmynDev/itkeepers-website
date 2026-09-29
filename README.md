# ITKeepers Website V1

A fast, prerendered Astro redesign built around **“Your IT person is a team.”** It preserves the existing ITKeepers navy/cyan palette while making the operating model the main differentiator.

## Local development

```bash
npm install
npm run dev
npm run build
```

Node.js **22.x** is the production runtime target.

## Cloudflare deployment

The connected Cloudflare project uses the current **Workers Git build pipeline with static assets**.

- Production branch: `main`
- Build command: `npm run build`
- Deploy command: `npx wrangler deploy`
- Astro output directory: `dist`
- Static assets source: `./dist`
- Node.js: `22.x`

`wrangler.toml` declares `[assets] directory = "./dist"`, allowing Cloudflare's Git integration to deploy the prerendered Astro site after every push to `main`.

## Routes

Home; Managed IT; Microsoft & Cloud; Cybersecurity; Networks & Infrastructure; Backup & Recovery; How We Work; Our Team; Contact; Privacy.

## Design rules

Editorial hierarchy, real operational explanations, no fabricated testimonials or counters, no fake live monitoring, and no stock employees.

## Security

The site is static/prerendered and contains no credentials or client infrastructure data. Security headers are defined in `public/_headers`. See `SECURITY.md` for the hardening baseline.

## Next priorities

Add approved team photography and roles; confirm approved scale evidence; wire a secure server-side contact form; map redirects from the current site; run accessibility/performance/cross-browser QA; copy the approved logo into the repository when its source asset is available; verify production TLS/HSTS and privacy handling.
