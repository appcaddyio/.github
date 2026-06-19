# AppCaddy brand assets

Logos, icons, and banners for AppCaddy. One folder per type; each holds the vector master (`.svg`) plus its PNG exports. Every file is `appcaddy-` named.

Raw base URL for embedding in other repos and pages:

```
https://raw.githubusercontent.com/appcaddyio/.github/main/brand/
```

## Folders

| Folder | What's in it | Use |
|---|---|---|
| `icon/` | `appcaddy-icon.svg`, PNG 16 to 1024, `appcaddy-favicon.ico`, `appcaddy-maskable-192/512.png` | App icon, favicon, PWA. Rounded square. |
| `wordmark/` | `appcaddy-wordmark-{light,dark}.svg` + PNG 80/160/320 | Text only. Set in DM Sans 700, outlined to curves. |
| `lockup/` | `appcaddy-lockup-{light,dark}.svg` + PNG 96/200/400 | Icon plus wordmark together. |
| `mark/` | `appcaddy-mark-{teal,white}.svg` + PNG 256/512/1024 | Icon glyph only, no tile. |
| `inverse/` | `appcaddy-inverse.svg` + PNG 128 to 1024 | Teal glyph on the canvas color. |
| `avatar/` | `appcaddy-avatar.svg` + PNG 128 to 1024 | Circular profile pictures. |
| `banner/` | `appcaddy-banner-{A,B,C}-{fb,linkedin,og,x}-<WxH>.png`, plus `appcaddy-banner-minimal-*` | Social and OG headers. B is the primary, A is the colored variant. |
| `store/` | `appcaddy-feature-graphic-1024x500.png` | Play Store feature graphic. |

## Light and dark

`-light` is light-colored artwork, for dark backgrounds. `-dark` is dark artwork, for light backgrounds.

## Typeface

The wordmark is set in DM Sans 700. "App" uses Ink, "Caddy" uses Accent.

## Colors

Canvas `#F4F5F4` &middot; Ink `#141414` &middot; Accent `#3D7575` &middot; Dark-mode accent `#5FA8A8`

## Web favicon

Copy the icon files into the site root (rename `appcaddy-favicon.ico` to `favicon.ico`), then add to `<head>`:

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
