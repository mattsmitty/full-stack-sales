# Full Stack Sales — Website

Static site (11 self-contained HTML pages). No build step, no dependencies to install.

## Deploy on GitHub Pages
1. Create a new GitHub repo (Public).
2. Upload all `.html` files plus this `CNAME`.
3. Repo **Settings → Pages → Source: `main` / root → Save**.
4. Live at `https://<username>.github.io/<repo>/` within ~1 minute.

## Custom domain (fullstacksales.com)
The included `CNAME` file points the site at fullstacksales.com.
At your domain registrar (GoDaddy/Namecheap/etc.), set DNS:

**Apex domain (fullstacksales.com)** — add four A records:
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153

**www subdomain** — add one CNAME record:
www  ->  <username>.github.io

Then in repo Settings → Pages, confirm the custom domain and check "Enforce HTTPS".
DNS can take 10 min to a few hours to propagate.

## Pages
index · services · process · gtm-strategy · linkedin-prospecting ·
fractional-vp-sales · fractional-cmo · growth-analytics · team · about · book

## Notes
- Each HTML file is fully self-contained (CSS, JS, logo, team images inlined).
- External loads: Google Fonts + Calendly widget (both from their CDNs).
- Keep filenames as-is so nav links resolve.
