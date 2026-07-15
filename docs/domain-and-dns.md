# lastwishes.sg — domain registration & DNS

_Recorded 2026-07-15, from the Vodien control panel after purchase._

## Registration
- **Domain:** lastwishes.sg
- **Registrar:** Vodien (SGNIC-accredited)
- **Created:** 2026-07-15 · **Expires:** 2027-07-15 (renew ~S$50/yr — set a reminder)
- **Registrant / Admin / Billing / Tech contact:** Tyler Wong

## Name servers (Vodien default — DNS is managed in the Vodien panel)
| # | Name server | IPs |
|---|---|---|
| 1 | ns1.vodien.com | 162.159.24.10, 2400:cb00:2049:1::a29f:180a |
| 2 | ns2.vodien.com | 162.159.25.66, 2400:cb00:2049:1::a29f:1942 |

## DNS records as purchased (Vodien defaults, "Premium")
| Type | Host | TTL | Value |
|---|---|---|---|
| A | lastwishes.sg | 14400 | 103.11.189.189 (Vodien hosting — NOT our site) |
| A | localhost.lastwishes.sg | 14400 | 127.0.0.1 |
| A | mail.lastwishes.sg | 14400 | 103.11.189.189 |
| A | *.lastwishes.sg | 14400 | 103.11.189.189 |
| CNAME | www.lastwishes.sg | 14400 | lastwishes.sg |
| CNAME | ftp.lastwishes.sg | 14400 | lastwishes.sg |
| MX | lastwishes.sg | 14400 | mail.lastwishes.sg |

## Changes needed to serve the site from Vercel
Do these in the Vodien DNS panel **after** adding the domain to the Vercel
project (Vercel → Project → Settings → Domains → add `lastwishes.sg` and
`www.lastwishes.sg`; Vercel shows the authoritative values — trust its screen
if it differs from below):

1. **Edit the apex A record:** `lastwishes.sg` → change `103.11.189.189` to
   Vercel's IP (currently `76.76.21.21`).
2. **Edit the www CNAME:** `www.lastwishes.sg` → change `lastwishes.sg` to
   `cname.vercel-dns.com`.
3. **Delete the wildcard** `*.lastwishes.sg` A record (otherwise random
   subdomains show Vodien's parking/hosting page).
4. Leave `mail` A + MX records only if using Vodien email on this domain;
   they don't affect the website either way. Delete `ftp` and `localhost`
   records — unused defaults.

TTL is 14400s (4 h), so changes can take up to ~4 h to propagate — edit
records early, verify with `dig lastwishes.sg +short`.

## Deployment target
- **GitHub repo:** https://github.com/SlothWriteCode/lastwishes-sg
- **Host:** Vercel (static, no build step; `vercel.json` handles clean URLs)
- **Primary URL:** https://lastwishes.sg (www redirects to apex)
