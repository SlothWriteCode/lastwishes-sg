# Launch notes — 2026-07-15

**The site is LIVE at https://lastwishes.sg** 🎉

## What we did today
1. **Chose the name from real search data.** Google (SG) autocomplete shows families
   search question phrases ("what to do when someone dies singapore", "my last
   wishes", "columbarium singapore price") — nobody knows the word "columbarium"
   until they need it. All question-style `.com`s were already taken; the `.sg`s
   were free. Full DNS/registration details: `domain-and-dns.md`.
2. **Bought `lastwishes.sg`** at Vodien (expires **2027-07-15** — set a renewal
   reminder!).
3. **Rebranded** the site from placeholder "Family Wishes SG" → **Last Wishes SG**
   (headers, footers, titles, AI prompt) and added canonical + Open Graph tags
   pointing at lastwishes.sg (OG tags = the WhatsApp link-preview card).
4. **Deployed to Vercel**: project `lastwishes-sg` under team
   `sloths-projects-5fb96aa3`, imported from this repo. `vercel.json` gives clean
   URLs (`/checklist`, `/avoid-scams`).
5. **Pointed DNS at Vercel** (Tyler edited the Vodien panel): apex A →
   `76.76.21.21`, www CNAME → `cname.vercel-dns.com`. Verified live with HTTPS,
   http→https redirect working, all 3 pages 200.

## Loose ends (small)
- [ ] **www.lastwishes.sg cert** was still being issued at launch — should fix
      itself within hours. If it still errors later: Vercel project → Settings →
      Domains, check `www.lastwishes.sg` status.
- [ ] **Wildcard `*.lastwishes.sg` A record** (→ Vodien 103.11.189.189) may not
      have been deleted — re-check the Vodien DNS panel and delete it.

## Next steps, in order of impact
1. [ ] **Footer placeholders**: replace `[YOUR BUSINESS NAME]` / `[YOUR UEN]` in
       all 3 pages once ACRA-registered.
2. [ ] **Tracking before ads**: GA4 property + Search Console (verify domain) +
       Google Ads conversion for WhatsApp-click. See
       `marketing-and-tracking-plan.md`.
3. [ ] **The S$100–300 Google Search test** per `google-ads-plan.md`, pointing at
       `https://lastwishes.sg/`. Check real volumes/CPCs in Keyword Planner first
       (free with the Ads account).
4. [ ] **Sendable checklist PDF** (the "Send this to my WhatsApp" promise).
5. [ ] **WhatsApp Business** setup for +65 90107246.

## How to deploy changes
Vercel CLI is authenticated on the Mac (user `slothwritecode-3238`). From the
repo root:

```
git push                          # keep GitHub in sync
npx vercel deploy --prod --yes    # deploy to production
```

(Mac has Node 18; Vercel CLI warns it wants Node 20 but works. Pushing to GitHub
alone does NOT auto-deploy — the project was linked via CLI, not Git import. If
you want push-to-deploy, connect the Git repo in Vercel → Project → Settings →
Git.)
