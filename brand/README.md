# AppCaddy brand assets

Logos, icons, and banners for AppCaddy. Source masters live in `svg/`. Everything else is exported PNG.

Raw base URL for embedding in other repos and pages:

```
https://raw.githubusercontent.com/appcaddyio/.github/main/brand/
```

## Files

| Folder | Use | Notes |
|---|---|---|
| `svg/` | Scalable masters | `mark`, `icon`, `avatar`, `inverse` are pure vector and portable. `wordmark` and `lockup` carry live text and need the Syne font to render correctly; prefer the PNGs below, or outline the text first. |
| `icon/` | App icon, favicon, PWA | Rounded square. 16 to 1024 px, includes 180 (apple-touch) and 192. |
| `avatar/` | Profile pictures | Circular mark. GitHub org, Buy Me a Coffee, social accounts. |
| `mark/` | Icon only, no tile | `teal` for light backgrounds, `white` for dark. |
| `inverse/` | Icon, teal on light | For placing on the canvas color. |
| `wordmark/` | Text only | See light/dark rule below. |
| `lockup/` | Icon plus wordmark | See light/dark rule below. |
| `banner/` | Social and OG headers | Concepts A, B, C. Each in fb 1640x624, linkedin 1584x396, og 1200x630, x 1500x500. B is the primary, A is the colored variant. |

## Light and dark

`-light` is light-colored artwork, for dark backgrounds. `-dark` is dark artwork, for light backgrounds.

## Colors

Canvas `#F4F5F4` &middot; Ink `#141414` &middot; Accent `#3D7575` &middot; Dark-mode accent `#5FA8A8`

Published by AppCaddy.
