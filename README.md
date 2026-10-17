# Festival Wishes Maker — Dussehra & Diwali Greeting Cards

A free, one-page web app that lets anyone create a personalised festival greeting card with their name in seconds — no sign-up, no uploads, everything is drawn in the browser.

**Live:** https://festival-wishes-maker.vercel.app/

## What it does

- **Two festivals:** Dussehra (Vijayadashami, Tue 20 Oct 2026) and Diwali (Sun 8 Nov 2026), with a festival selector at the top — Dussehra is the default because it comes first.
- **7 hand-coded card designs** (3 for Dussehra, 4 for Diwali), all drawn with the HTML canvas API — diyas, marigold toran garlands, rangoli mandalas, bow & arrow, fireworks. No external image files.
- Type a recipient name (optional) and your own name, pick one of 3 wish messages per festival, and the 1080×1080 card updates live.
- **Download PNG** or **Share on WhatsApp** (Web Share API with the image file where supported; falls back to a wa.me text share).
- Live countdown chips for both festivals (IST), plus a strip showing the 5 days of Diwali 2026 (Dhanteras 6 Nov → Bhai Dooj 10 Nov).

## Files

- `index.html` — the entire site (HTML, CSS and JS in one file)
- `vercel.json` — minimal config so Vercel serves the folder as a plain static site

## Tech

Plain static HTML/CSS/JS. No backend, no build step, no tracking. Cards are rendered locally in the visitor's browser via `<canvas>`.
