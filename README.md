# Lounge 55 — Website

Astro one-pager for Lounge 55 VIP Membership.

## Stack
- [Astro](https://astro.build) (static output)
- Vanilla CSS with scoped component styles
- Hosted on Cloudflare Pages via GitHub

---

## Local Development

```bash
npm install
npm run dev
```

Visit `http://localhost:4321`

## Build

```bash
npm run build
# Output goes to ./dist
```

---

## Deploying to Cloudflare Pages (via GitHub)

1. Push this repo to GitHub.
2. Go to [Cloudflare Dashboard](https://dash.cloudflare.com) → **Pages** → **Create a project**.
3. Connect your GitHub account and select this repo.
4. Set the following build settings:

| Setting             | Value           |
|---------------------|-----------------|
| Framework preset    | **Astro**       |
| Build command       | `npm run build` |
| Build output dir    | `dist`          |
| Node.js version     | `18` or `20`    |

5. Click **Save and Deploy**.
6. Under **Custom Domains**, add your domain from Cloudflare DNS.

---

## Updating Content

All content lives in the component files under `src/components/`:

| File                        | What to edit                             |
|-----------------------------|------------------------------------------|
| `src/components/Hero.astro` | Tagline, headline, CTA button links      |
| `src/components/About.astro`| Description text, stats                  |
| `src/components/Membership.astro` | Benefits list, pricing             |
| `src/components/Join.astro` | CTA text, email/contact link             |
| `src/components/Footer.astro` | Copyright, tagline                     |
| `src/layouts/BaseLayout.astro` | Global CSS variables, fonts, meta    |

To change the brand color, update `--orange` in `BaseLayout.astro`.
