# M10 / Praneet Kamble portfolio v4 (manga theme, premium pass)

Static single page: index.html, style.css, script.js. No build step. Only external dependency: Google Fonts
(Bebas Neue headings, Inter body, Knewave for the M10 logo, Permanent Marker for brush section titles).

Run locally: `python3 -m http.server 8080` in this folder, open http://localhost:8080 (http, not file://, so the QR demos sync).

## Files
- assets/art/   original manga ink illustrations (WebP, fictional spiky-haired character): hero-main, panel-ideas/code/impact, about-portrait, contact-skyline.
               v4 art is rendered procedurally by _src/v4 (two-layer ink + screentone engine in headless Chrome), not traced or generated from any real person.
- assets/img/   real project screenshots (reused from portfolio-v2)
- demos/        cafe + restaurant QR table-ordering demos (fictional businesses, sample prices)
- screens/      headless Chrome verification screenshots (1440px desktop, 375px mobile)
- _src/         v4 art generator (_src/v4: ink.py, chars.py, scenes.py, run.py) and screenshot script (shoot.py); not needed to host the site
- M10-website-walkthrough-v4.mp4  screen-recorded walkthrough (1440x900, 30fps); not needed to host the site

## What's new in v4
- New ink artwork with screentone shading, rim light and rough brush edges (same filenames and aspect ratios as v3).
- One accent colour (red #ff2b2b on ink, #c8102e on paper) used for underlines, shadows, counters and hover states.
- Motion: staggered scroll reveals, image wipe-ins, hero panel parallax (pointer + scroll), two marquees, magnetic buttons and chips,
  card/service tilt with glare, ink-splash click bursts, animated counters (they count up to the real numbers recounted from the page),
  scroll progress bar, torn-paper section edges, film-grain overlay and an optional cursor ring on mouse devices.
- All motion is switched off under prefers-reduced-motion; touch devices get no tilt, magnet or cursor effects.

## TODO before publishing
- Replace the "Case studies" note when a client agrees to be named.
- Optional: swap assets/art/*.webp for higher-detail artwork (keep filenames and aspect ratios).
