# Masjid Tawheed — Stakeholder Mockup

A static-HTML redesign concept for [masjidtawheed.net](https://www.masjidtawheed.net/), built to demonstrate proposed improvements to stakeholders.

**This is a mockup, not the live site.**

## Run locally

```bash
# any static server works
python3 -m http.server 8000
# then open http://localhost:8000
```

Or just open `index.html` directly in a browser.

## Deploy

This is a single static page — drop into Vercel, Netlify, GitHub Pages, or Cloudflare Pages with no build step.

### Vercel

```bash
vercel        # first deploy
vercel --prod # subsequent deploys
```

`vercel.json` already configures cleanUrls and asset caching.

## What's included

- Working prayer-time widget (AlAdhan API, Stone Mountain GA, ISNA method — same source as the live site)
- Jumu'ah block with DST-aware schedule
- Real address, hours, donation methods (PayPal + Zelle)
- Schema.org `Mosque` JSON-LD for SEO
- Real masjid logo, brand colors, fluid mobile layout

## Files

- `index.html` — entire site (HTML + CSS + JS, no build step)
- `assets/logo.png` — masjid logo
- `vercel.json` — caching headers
- `robots.txt` — noindex (so this draft doesn't get indexed)
