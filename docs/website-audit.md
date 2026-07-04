# Website Audit — Family Wishes SG cold-lead funnel

_Date: 2026-07-04 · Reviewer: honest pre-spend audit_

## Verdict

**It can work — but not as it stands today.** The strategy and content are strong; the *conversion machinery* and *trust proof* are not finished. If you run ads to it right now, you'll likely get clicks but few WhatsApp opt-ins, and you won't be able to tell why. Fix the 3 blockers below first. They're small.

---

## What's already working

- **Right strategy for the market.** The SEO results are saturated with price-first competitors (nirvanafugui.com, singaporefuneralcare.com, funeralguru.com.sg, etc.). Leading with *calm, non-price, family-first* guidance is genuine differentiation, not a me-too page.
- **The lead magnet matches real search intent.** People search "funeral planning checklist", "columbarium singapore", "what to do when someone dies singapore". A free checklist is exactly what they want, and it's useful *before* they're ready to buy — which widens the top of funnel.
- **Low-friction CTA.** WhatsApp is how Singaporeans actually talk to small providers. Click-to-chat beats a form.
- **Trust scaffolding.** Scam guide + CCCS/CASE citations + "ask before paying anyone, including me" is credibility-building and safe.
- **Mobile-ready.** Most SG traffic is mobile; the redesign is responsive with a sticky WhatsApp CTA.

---

## 🔴 Blockers — fix BEFORE spending a cent

1. **No real human identity = trust death for a grief/money purchase.**
   Right now it's an anonymous "Family Wishes SG" with a placeholder silhouette. Cold visitors handing over their parents' funeral decisions will not message a faceless page.
   **Fix:** real photo, real first name, one line of who you are / why you do this. This is the single highest-leverage conversion fix on the whole site.

2. **No conversion tracking = flying blind, guaranteed wasted budget.**
   A `wa.me` click is invisible to Google Ads by default. Without it you cannot see which keyword or ad produced a lead, so you can't cut losers or scale winners — you'll just burn the SGD 100–300 and learn nothing.
   **Fix:** add the Google tag + track WhatsApp-button clicks as a conversion (setup steps in `google-ads-plan.md`).

3. **No sendable checklist file + no reply plan.**
   The CTA promises "message me and I'll send the checklist", but the checklist is a web page, not a file, and there's no plan for replying fast. Cold leads go cold in minutes.
   **Fix:** (a) export the checklist to a shareable PDF ready to send; (b) set a WhatsApp Business greeting/auto-reply and a saved quick-reply with the PDF link; (c) decide who answers and how fast (target: within the hour during the day).

---

## 🟡 Should-fix (raises results, not blockers)

- **Real domain.** A custom domain (e.g. a cheap `.sg`/`.com`) converts and ranks better than a `*.vercel.app`/`*.netlify.app` URL, and looks legitimate in the ad. Google allows subdomains, but a real domain is worth the ~S$10–40/yr.
- **Positioning honesty.** If you are ultimately steering people to one provider (e.g. Nirvana), the "independent" framing must stay truthful — describe yourself accurately (e.g. "I help families compare, and I also work with X") or you risk a misrepresentation problem and broken trust. Decide this now; it affects the ad copy.
- **Light analytics.** Even a privacy-simple analytics tool tells you scroll depth / which page they bounce on. Optional but useful.
- **One thank-you step.** After the WhatsApp click, a simple confirmation/thank-you page makes conversion tracking cleaner and reassures the user.
- **Proof over time.** Add a testimonial or "families I've helped" line once you have one. Not now, but plan for it.

---

## Realistic expectations (do the math before you spend)

Rough, to be confirmed with Google Keyword Planner:

- **CPC** for SG funeral/columbarium commercial keywords is not cheap — plan for roughly **S$2–6 per click** (some high-intent terms higher).
- **SGD 100–300 test ≈ 30–120 clicks.**
- At a **5–15% WhatsApp opt-in rate** (realistic for a good, trusted page), that's ~**3–15 opt-ins**.
- Of those, maybe a handful become real conversations, and **0–2 become customers** in the test window — funeral pre-planning has a long, emotional decision cycle.

**So judge the test by the right metric.** The test's job is to prove **people will click the ad AND opt in on WhatsApp** at a sane cost-per-opt-in — not to make money in week one. If cost-per-opt-in is reasonable and conversations happen, the model is validated and worth scaling. If nobody opts in, we fix the page (usually trust/identity) before spending more.

---

## Compliance check ✅

- **Google Ads:** keyword-based **Search** ads for funeral/columbarium are permitted. Only *personalized/remarketing/Customer-Match targeting on bereavement* is banned — we're not doing that, so we're clear. (Source: Google Advertising Policies — Restricted targeting in personalised advertising; Sensitive events.)
- **PDPA (Singapore):** funnel is inbound (they message you first) → compliant. Do **not** cold-message strangers.
- **Defamation:** scam guide names tactics only, no companies, cites CCCS/CASE → safe.
- **Disclaimers:** "not legal advice / verify with official sources" present on every page → good.

---

## Fix checklist (in priority order)

- [ ] Add real photo + name + one-line bio to the "real person" section
- [ ] Add Google tag + WhatsApp-click conversion tracking
- [ ] Export checklist to a sendable PDF + set WhatsApp Business auto-reply/quick-reply
- [ ] Decide + state the "independent vs affiliated" positioning honestly
- [ ] Buy a real domain and deploy
- [ ] (Optional) thank-you page + light analytics

Sources: Google Advertising Policies (personalised advertising restrictions; sensitive events); Singapore columbarium price guides (govt niches from ~S$500; private S$2k–200k; Nirvana from ~S$8k single / S$12k double).
