# HoneyHole Landing Page

🐟 **Live:** https://honey-hole-landing.vercel.app

A dark-themed, premium landing page for HoneyHole — the offline-first fishing logbook for iOS and Android.

## Quick Start

```bash
# Open in browser
open https://honey-hole-landing.vercel.app

# Local development (any static server)
npx serve .
# or
python3 -m http.server 8000
```

## Tech Stack

- Pure HTML/CSS/JS — no framework
- Inter font from Google Fonts
- Vercel for hosting

## Deployment

Deployed automatically via Vercel + GitHub Actions.

### One-Time GitHub Setup (adds auto-deploy)

1. Go to **vercel.com** → sign in to the `jason-scotts-projects` account
2. Go to **HoneyHole Landing** project → **Settings → Git**
3. Click **Connect Git Repository** → select `theBlackEndDev/honey-hole-site`
4. Done — every push to `main` auto-deploys

### Manual Deploy

```bash
vercel --prod
```

## Project Structure

```
index.html   — full landing page (HTML + CSS + JS)
SPEC.md      — app spec (from The Forge)
README.md    — this file
.github/workflows/deploy.yml — auto-deploy config
```

## Domain Setup (when you own honey-hole.app)

1. Vercel dashboard → HoneyHole Landing → **Settings → Domains**
2. Add `honey-hole.app` and `honey-hole.co`
3. Vercel gives you a DNS record to add at your registrar
4. Point DNS, wait for propagation, done

## Updating the Landing Page

Edit `index.html` directly, then push:

```bash
git add .
git commit -m "feat: update [what changed]"
git push
# Vercel auto-deploys in ~30 seconds
```
