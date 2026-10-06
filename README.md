# Glacier Santini — Digital Menu

A single-page, phone-first ice cream menu (Lisbon). English / Portuguese switch, vegan filter,
4 categories (each with its own animated header icon), 9 flavours with icons, line-art ice cream background.

## Files
- `index.html` — the whole site (HTML, CSS, JS and the 9 flavour icons embedded). Open it in a browser or upload it to any host.
- `assets/flavour-icons/` — the 9 flavour icons as small .webp files (already embedded in index.html).
- `assets/flavour-icons-original/` — original full-size PNGs.
- `assets/background-pattern.svg` — the line-art background tile (also embedded in index.html).

## Editing
Everything is in `index.html`, inside the `<script>` block:
- `CATS` — categories, items, descriptions and prices (`['Name', price, 'Description', {v:1 = vegan, n:1 = new}]`).
- `FLAVOURS` — the 9 flavours (`['Name', 'Tasting note', {v:1}]`); icons are in `ICONS`, in the same order.
- `NL` — the English → Portuguese dictionary (the variable keeps this name; keys must match the English text exactly). Add an entry for every new text.
- Colours are CSS variables at the top of the `<style>` block (`--tomato`, `--pista`, `--honey`, `--cocoa`, `--paper`, `--ink`).

## Hosting
Upload `index.html` to Netlify, Cloudflare Pages, GitHub Pages or similar. Point your QR code to the URL.
Fonts (Fraunces, Space Mono) load from Google Fonts, so the first visit needs internet access;
system fonts are used as fallback.

## Not included yet
Google review button (needs the shop's Place ID or the "Ask for reviews" link from Google Business Profile),
sold-out states, allergen filters beyond vegan.
