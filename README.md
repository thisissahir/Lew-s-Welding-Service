# Lew's Welding Service — Website

Single-page marketing site for **Lew's Welding Service**, Tyler, Texas (est. 1928).
Static HTML/CSS with no build step.

- **Live business:** 1716 E Erwin St, Tyler, TX 75702 · (903) 597-6685
- **Hours:** Mon–Fri, 7:00 AM – 3:00 PM

## Structure

```
index.html      # the entire site (inline CSS + minimal JS)
brand/          # logo set (SVG + PNG variants)
vercel.json     # clean URLs, security headers, asset caching
*.mp4, *.jpg    # video and image assets
```

## Deploy to Vercel

There is **no build step** — Vercel serves the static files as-is.

### Option A — Connect the GitHub repo (recommended)
1. Go to [vercel.com/new](https://vercel.com/new) and import
   `thisissahir/Lew-s-Welding-Service`.
2. Framework Preset: **Other**. Leave Build Command and Output Directory **empty**.
3. Click **Deploy**. Every push to `main` auto-deploys after that.

### Option B — Vercel CLI
```bash
npm i -g vercel
vercel        # preview deploy
vercel --prod # production deploy
```

## Custom domain (lewswelding.com)

The site's canonical URL is `https://lewswelding.com/`. After the first deploy:
Vercel → Project → **Settings → Domains** → add `lewswelding.com`, then point the
domain's DNS at Vercel per the on-screen instructions.

## Local preview

No server needed — open `index.html` in a browser, or:
```bash
npx serve .
```
