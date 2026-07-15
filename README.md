# Last Wishes SG — landing site (lastwishes.sg)

Calm, independent lead-generation site for Singapore families planning columbarium / funeral wishes. Built as the destination for cold Google Search ad traffic.

## Pages
- `index.html` — landing page + free-checklist offer + WhatsApp CTA
- `checklist.html` — the full free family checklist (the lead magnet, published openly)
- `avoid-scams.html` — "8 red flags & how to avoid funeral scams" consumer guide (trust builder)
- `styles.css` — shared styling

## Before going live
1. **WhatsApp number:** set to `6590107246` (+65 90107246).
2. **Brand name:** "Last Wishes SG", on domain `lastwishes.sg` — chosen 2026-07-15 from real Google (SG) autocomplete data: families search questions ("what to do when someone dies singapore", "my last wishes"), not the word "columbarium".
3. **UEN / business name:** still `[YOUR BUSINESS NAME]` / `[YOUR UEN]` placeholders in each footer — fill in once ACRA-registered.

## Positioning guardrails (from the vault)
- Independent personal guidance — **no** corporate Nirvana logo/branding, no "authorised agent" hero claim, no certification claims.
- Calm, non-price-first, respectful of public options.
- Scam guide names **tactics/red flags only** — never a specific company — and cites CCCS/CASE. Not legal advice.

## Deploy (Vercel + lastwishes.sg)
Static site with `vercel.json` (clean URLs: `/checklist`, `/avoid-scams`; the `.html` paths redirect).
1. Push repo to GitHub, import into Vercel (framework preset: Other, no build step).
2. In Vercel → Domains, add `lastwishes.sg` (and `www.lastwishes.sg` → redirect to apex), then set the DNS records Vercel shows at the .sg registrar.
3. Point the Google Search ads at `https://lastwishes.sg/`.
