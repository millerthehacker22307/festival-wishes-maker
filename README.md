# Festival Wishes Maker — Festive Season Greeting Cards

A free, one-page web app that lets anyone create a personalised festival greeting card with their name in seconds — no sign-up, no uploads, everything is rendered in the browser.

**Live:** https://festival-wishes-maker.vercel.app/

## What it does

- **Seven festivals:** Dussehra (Tue 20 Oct 2026), Dhanteras (6 Nov), Choti Diwali (7 Nov), Diwali (Sun 8 Nov 2026), Govardhan Puja (9 Nov), Bhai Dooj (10 Nov) and Chhath (Sun 15 Nov) — each festival has its own design pool, wishes (English + Hindi) and artwork, with a season timeline and live countdowns (IST).
- **Original artwork backgrounds:** every backdrop is an illustration created for this site (5 scenes per festival, each in 3 framings — full, zoom and warm), bundled as data URIs in `assets/photos-<festival>.js`. No stock photos.
- **Crore-scale combinations:** 6 colour themes × 21 backgrounds × 6 frames × 6 motifs × 4 arrangements × 6 overlays × 5 headline styles × 6 name styles × 3 layouts per festival — 6,85,84,320+ designs in total, computed live on the page.
- Type a recipient name (shown big) and your own name, pick a ready wish, write your own, or use the **Instant Wish Generator**. Cards render at 1080×1080.
- **Download PNG** or **Share on WhatsApp** (Web Share API with the image file where supported; falls back to a wa.me text share).
- Ready Designs gallery (18 per festival) plus a no-repeat **Surprise Me** randomiser.

## Files

- `index.html` — the entire site (HTML, CSS and JS in one file)
- `assets/photos-<festival>.js` — per-festival artwork bundles (base64 data URIs, lazy-loaded)
- `vercel.json` — minimal config so Vercel serves the folder as a plain static site

## Tech

Plain static HTML/CSS/JS. No backend, no build step, no tracking. Cards are rendered locally in the visitor's browser via `<canvas>`.
