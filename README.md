# pocketzineclub.com

Marketing landing page for **Pocket Zine** — a local-first publishing tool for
illustrators, photographers, writers and indie publishers.

- **Landing:** https://pocketzineclub.com (this repo)
- **App:** https://pocketzine.app (separate repo)

## Stack

A single static `index.html` — no build step, no dependencies. Fonts load from
Google Fonts; everything else is inline CSS + a little vanilla JS (scroll reveals
and the animated ASCII book).

## Develop

Open `index.html` directly in a browser, or serve the folder:

```sh
python3 -m http.server 8000
# → http://localhost:8000
```

## Deploy

Static host (Cloudflare Pages, Netlify, Vercel — no framework). Publish the repo
root; there is no build command and no output directory.

## Structure

```
index.html        landing page (all sections + inline styles/script)
landing/logo.svg  Pocket Zine wordmark
landing/zines/    gallery / template imagery
```

## TODO before launch

- [ ] Replace the imagery in `landing/zines/` with real Pocket Zine exports.
      The current files are placeholder reference art and are NOT cleared for
      public use.
- [ ] Point the **Donate** button (`href="#donate"`) at a real URL.
- [ ] Fill in footer links (Manifesto / Changelog / Roadmap / socials).
