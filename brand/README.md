# AppCaddy brand assets

Logos, icons, and banners for AppCaddy. Vector masters live in `svg/`. Everything else is exported PNG.

Raw base URL for embedding in other repos and pages:

```
https://raw.githubusercontent.com/appcaddyio/.github/main/brand/
```

## Files

| Path | Use | Notes |
|---|---|---|
| `svg/` | Scalable masters | All self-contained vector. `wordmark` and `lockup` are outlined paths (text set in DM Sans 700, converted to curves), so they render the same everywhere with no font installed. |
| `icon/appcaddy-icon-*.png` | App icon, favicon, PWA | Rounded square. 16 to 1024 px, includes 180 (apple-touch) and 192. |
| `icon/favicon.ico` | Classic favicon | Multi-size 16/32/48 in one file. |
| `icon/appcaddy-maskable-*.png` | PWA and Android maskable | Full-bleed teal, glyph inside the safe zone. 512 and 192. |
| `avatar/` | Profile pictures | Circular mark. GitHub org, Buy Me a Coffee, social accounts. |
| `mark/` | Icon only, no tile | `teal` for light backgrounds, `white` for dark. |
| `inverse/` | Icon, teal on light | For placing on the canvas color. |
| `wordmark/` | Text only | PNG at 80/160/320. See light/dark rule below. |
| `lockup/` | Icon plus wordmark | PNG at 96/200/400. |
| `banner/` | Social and OG headers | Concepts A, B, C. Each in fb 1640x624, linkedin 1584x396, og 1200x630, x 1500x500. B is the primary, A is the colored variant. |
| `store/play-feature-graphic-1024x500.png` | Play Store feature graphic | Required for any Play listing. |

## Light and dark

`-light` is light-colored artwork, for dark backgrounds. `-dark` is dark artwork, for light backgrounds.

## Typeface

The wordmark is set in DM Sans 700 at natural spacing. The "App" segment uses Ink, the "Caddy" segment uses Accent.

## Colors

Canvas `#F4F5F4` &middot; Ink `#141414` &middot; Accent `#3D7575` &middot; Dark-mode accent `#5FA8A8`

## Web favicon

Copy the icon files into the site root, then add to `<head>`:

```html
<link rel="icon" href="/favicon.ico" sizes="32x32">
<link rel="icon" href="/appcaddy-icon.svg" type="image/svg+xml">
<link rel="apple-touch-icon" href="/appcaddy-icon-180.png">
<link rel="manifest" href="/site.webmanifest">
<meta name="theme-color" content="#3D7575">
<meta property="og:image" content="https://appcaddy.io/og.png">
```

`site.webmanifest`:

```json
{
  "name": "AppCaddy",
  "icons": [
    { "src": "/appcaddy-icon-192.png", "sizes": "192x192", "type": "image/png" },
    { "src": "/appcaddy-icon-512.png", "sizes": "512x512", "type": "image/png" },
    { "src": "/appcaddy-maskable-512.png", "sizes": "512x512", "type": "image/png", "purpose": "maskable" }
  ],
  "theme_color": "#3D7575",
  "background_color": "#F4F5F4"
}
```

Published by AppCaddy.
