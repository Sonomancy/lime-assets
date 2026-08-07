# lime-assets

Self-hosted static assets for LIME, served via GitHub Pages at **https://assets.lime.online**.

Any file committed here is live at `https://assets.lime.online/<path>` — no per-file setup.

## Logos — `logos/`

Master logo is 1182x500 (no tagline) or 2542x500 (with tagline). PNGs have transparent
backgrounds. **Use PNG in email** — SVG is not supported by Outlook or Gmail.

| File | URL |
|---|---|
| `lime-logo-green.png` / `.svg` | https://assets.lime.online/logos/lime-logo-green.png |
| `lime-logo-black.png` / `.svg` / `.jpg` | https://assets.lime.online/logos/lime-logo-black.png |
| `lime-logo-white.png` / `.svg` | https://assets.lime.online/logos/lime-logo-white.png |
| `lime-logo-green-tagline.png` / `.svg` | https://assets.lime.online/logos/lime-logo-green-tagline.png |
| `lime-logo-black-tagline.png` / `.svg` / `.jpg` | https://assets.lime.online/logos/lime-logo-black-tagline.png |
| `lime-logo-white-tagline.png` / `.svg` | https://assets.lime.online/logos/lime-logo-white-tagline.png |

White logos are for dark backgrounds — they are invisible on white, and the PNG transparency
will look like a blank box in any client that strips it. Prefer green or black for email.

`logos/print/` holds the CMYK vector PDFs (same six variants) for print and artwork handoff.

## Department thumbnails — `thumbnails/`

180x180 PNGs: `accounting` `b2b` `b2c` `compliance` `cr` `csuite` `energy` `installations`
`it` `logo` `marketing` `ops` `qc` `sales`

e.g. https://assets.lime.online/thumbnails/sales.png

## Banners — `banners/`

| File | Size | URL |
|---|---|---|
| `email-banner.png` | 1197x236 | https://assets.lime.online/banners/email-banner.png |
| `youtube-banner.png` | 2560x1440 | https://assets.lime.online/banners/youtube-banner.png |
| `button.png` | 200x50 | https://assets.lime.online/banners/button.png |

## Email signature

- `lime-email-signature.jpg` — signature footer banner, 1200x465
- `ces-lime-sig/` — CES signature image set

## Solar email templates — `solar-emails/`

Images and the solar/battery storage guide PDF used by the solar email sequence.

## Using these in email HTML

Always pin an explicit width, or Outlook will render the image at its full pixel size:

```html
<img src="https://assets.lime.online/logos/lime-logo-green.png"
     width="240" alt="LIME"
     style="width:240px;max-width:100%;height:auto;display:block;border:0;">
```
