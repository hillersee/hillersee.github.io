# hillersee.com

Hillers Electrical Engineering, Inc. — company website. Static HTML/CSS, no JavaScript, no build step.
Hosted free on GitHub Pages from `main`. Custom domain: `www.hillersee.com` (the `CNAME` file; set 2026-11-10 at launch).

Design and copy by Elizabeth Mendoza (27 Colab), built from the prototype in `27colab-shared/hillers/site`
(2026-11-09). Engineering, audits and deployment by Jesus Vasquez (27 Colab).

## Pages (sheet numbers follow nav order)
| Sheet | File | Page |
|---|---|---|
| E-1 | `index.html` | Home |
| E-2 | `about.html` | About |
| E-3 | `services.html` | Services (anchors `#power`, `#controls`, `#facilities`, `#project-services`) |
| E-4 | `market-focus.html` | Market Focus — the 20 utilities and agencies |
| E-5 | `contact.html` | Contact + Location (`#location`) |

Also: `404.html`, `robots.txt`, `sitemap.xml`, `favicon.svg`, `img/og.jpg` (link preview), and four stubs for the
old site's URLs (`index.htm`, `services.htm`, `offices.htm`, `contact.htm`) that forward to the new pages.
Fonts are self-hosted in `fonts/` (Barlow, IBM Plex Sans/Serif/Mono; latin subset, SIL OFL). Tokens at the top of
`css/site.css`.

## Editing
Edit the HTML directly. Keep `width`/`height` on images. If a page is added, update the nav on every page, the
footer "Sheet E-n of N", and `sitemap.xml`.

## Launch checklist
1. Logo and photos are now the client's high-resolution files (2026-11-10: `hee-logo-color.tif` at 300 dpi, background knocked out; four site photos). Export WebP if page weight matters.
2. GoDaddy DNS, web records only: `A` records for the apex → GitHub Pages (185.199.108.153, .109.153, .110.153,
   .111.153); `CNAME www` → `hillersee.github.io`. Do not touch MX, Mimecast, or `ftp.hillersee.com`.
3. Add a `CNAME` file containing `www.hillersee.com` (or set the custom domain in Settings → Pages), then "Enforce HTTPS" once the certificate issues. Do this only after step 2, or the preview URL starts redirecting to a domain that is not pointed here yet.
4. Confirm `https://www.hillersee.com/services.htm` forwards, and `ftp.hillersee.com` still resolves.
