# kredytowespory.pl — static landing

Static site for **kredytowespory.pl** (LexKredyt / Anastasiia Kondratenko, NIP 5214148547).
Deploy via **Cloudflare Pages drag-and-drop** (no build step).

## Stack
- Pure static HTML + native JS
- Tailwind CSS via CDN (`https://cdn.tailwindcss.com`)
- Google Fonts (Inter + Lora)
- **Web3Forms** backend for form submissions (access key embedded in HTML)

## Pages
| URL | File | Lang |
|---|---|---|
| `/` | `index.html` | UA (primary) |
| `/ru/` | `ru/index.html` | RU mirror |
| `/dyakuyemo` | `dyakuyemo.html` | UA thank-you |
| `/ru/spasibo` | `ru/spasibo.html` | RU thank-you |
| `/polityka-prywatnosci` | `polityka-prywatnosci.html` | PL master |
| `/polityka-cookies` | `polityka-cookies.html` | PL |
| `/regulamin` | `regulamin.html` | PL |
| `/ua/polityka-prywatnosti` | `ua/polityka-prywatnosti.html` | UA |
| `/ua/polityka-cookies` | `ua/polityka-cookies.html` | UA |
| `/ua/regulamin` | `ua/regulamin.html` | UA |
| `/ru/politika-konfidentsialnosti` | `ru/politika-konfidentsialnosti.html` | RU |
| `/ru/politika-cookies` | `ru/politika-cookies.html` | RU |
| `/ru/usloviya` | `ru/usloviya.html` | RU |

## Deployment
1. Zip the entire `kredytowespory-site/` directory
2. Open Cloudflare Dashboard → Pages → Upload assets
3. Drag the zip / folder
4. Bind domain `kredytowespory.pl`
5. Cloudflare will auto-pick `_headers` and `robots.txt`

## Brand colors
- Navy `#0F2A5A`
- Gold `#FBBF24`
- Cream `#FFF8E7`
- Bordeaux `#7A1F2B`

## Form backend
Web3Forms POST → `https://api.web3forms.com/submit`
Access key: `e4a2412e-aa13-4f00-b48e-05ab359880e5`
Email destination: configured on Web3Forms dashboard (kontakt@kredytowespory.pl)

## Compliance
All 12 mandatory fixes from `compliance_audit.md` applied. See parent agent report.

© 2026 LexKredyt
