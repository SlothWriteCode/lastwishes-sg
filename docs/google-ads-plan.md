# Google Ads Campaign Plan — Family Wishes SG

_Date: 2026-07-04 · Goal of first test: validate that cold searchers click AND opt in on WhatsApp at a sane cost — NOT to make money in week one._

> **Primary conversion (updated):** a **WhatsApp "tour enquiry"** (free private Nirvana tour) is now the main conversion to track; the checklist opt-in is the softer secondary conversion. Track both, but optimise toward tour enquiries. Ad copy should offer the **free private tour** as the lead hook, with the checklist as the low-commitment alternative. Disclose "Nirvana agent" honestly in ad copy where natural — do not imply neutrality.

> **Important framing:** We are **not competing on price.** Some of the keywords below are price-searches (e.g. "columbarium price") because that's what worried families type — but the ad and landing page **redirect them away from price** to calm right-fit guidance. We meet them where they search, then reframe. See "Non-price angle" below.

---

## 1. Campaign settings

| Setting | Value | Why |
|---|---|---|
| Campaign type | **Search only** | Highest intent; cheapest to learn from. No Display/PMax yet — too broad for a small budget. |
| Networks | Google Search only — **turn OFF Search Partners & Display** | Stops budget leaking to low-quality placements. |
| Location | **Singapore only** | Your entire market. |
| Language | English (add Chinese later) | Start simple. |
| Devices | All (expect mostly mobile) | Page is mobile-first. |
| Ad schedule | Start all-day; review after data | See when opt-ins actually happen. |

## 2. Budget & bidding

- **Budget:** ~**S$10–15/day** for **~2–3 weeks** = the S$100–300 test.
- **Bidding:** start on **"Maximize clicks" with a max CPC cap (~S$2.00–2.50)** OR **Manual CPC**. Do **not** start on "Maximize conversions" — it needs conversion history you don't have yet. Switch to conversion-based bidding only after ~15–30 tracked opt-ins.
- Confirm real CPCs in **Keyword Planner** before launch; SG funeral keywords may run ~S$2–6.

## 3. Ad groups & keywords (tightly themed)

Use **phrase match** `"..."` and a few **exact** `[...]` to start. **Avoid broad match** on a small budget — it wastes money.

**AG1 — Columbarium (general/commercial)**
`"columbarium singapore"`, `"columbarium niche"`, `"niche for ashes singapore"`, `[columbarium niche singapore]`

**AG2 — Public vs private / comparison**
`"government vs private columbarium"`, `"public columbarium singapore"`, `"private columbarium singapore"`, `"choosing a columbarium"`

**AG3 — Pre-planning & wishes (best fit for the checklist)**
`"funeral pre planning singapore"`, `"funeral planning checklist"`, `"plan funeral ahead singapore"`, `"funeral wishes"`

**AG4 — Ashes options**
`"what to do with ashes singapore"`, `"sea scattering singapore"`, `"keep ashes at home singapore"`, `"inland ash scattering"`

**AG5 — After a death / process (informational, high checklist fit)**
`"what to do when someone dies singapore"`, `"death certificate singapore process"`, `"funeral steps singapore"`

**AG6 — Price-searchers → reframe (optional, watch cost)**
`"columbarium price singapore"`, `"cost of columbarium niche"` — send to the checklist page; ad copy shifts them from "cheapest" to "what to ask before you pay".

> Each ad group points to the most relevant page: AG3/AG5 → `checklist.html`; AG1/AG2/AG6 → `index.html`; a scam-aware variant → `avoid-scams.html`.

## 4. Negative keywords (add at campaign level)

`free`* , `job`, `jobs`, `vacancy`, `hiring`, `salary`, `pet`, `dog`, `cat`, `hdb resale`, `wikipedia`, `meaning`, `definition`, `history`, `movie`, `netflix`, `grave plot` (if not offered), `muslim burial` (if not served), `christian burial` (if not served), `course`, `diploma`

\* consider keeping "free" if you want the free-checklist searchers; test both.

## 5. Ad copy — Responsive Search Ads (RSA)

Provide ~10 headlines + 4 descriptions per ad group; Google mixes them. Keep it **calm, non-price, no grief-exploitation**.

**AG3 (pre-planning) example RSA:**
- Headlines: `Free Family Planning Checklist` · `Plan Calmly, No Pressure` · `Singapore Funeral Wishes Guide` · `Compare Options Before You Decide` · `What To Ask Before You Pay` · `A Real Person, Not A Sales Call` · `Public vs Private, Explained` · `Record Your Family's Wishes` · `No Calls · No Pressure` · `Get It On WhatsApp`
- Descriptions: `A free, calm checklist for Singapore families. Compare options and record wishes — no pressure.` · `Understand public, private, home and scattering options before deciding. Ask anything on WhatsApp.` · `Independent guidance. My first job is to help you understand what fits — not to sell you.` · `Know the right questions to ask before paying anyone. Free checklist, no sign-up.`

**AG6 (price-searchers) reframe RSA:**
- Headlines: `Before You Compare Prices…` · `What To Ask Before You Pay` · `Avoid Hidden Funeral Fees` · `Compare The Right Option First` · `Free Checklist For Families` · `Calm, No-Pressure Guidance`
- Descriptions: `Price matters — but compare the right type of option first. Free checklist shows you how.` · `Know the hidden fees and questions that protect your family before paying anyone.`

## 6. Ad assets / extensions (do all — they're free and lift CTR)

- **Sitelinks:** Free Checklist · Public vs Private · How to Avoid Scams · Ask on WhatsApp
- **Callouts:** No sales calls · No pressure · Independent guidance · Free checklist · Reply on WhatsApp
- **Structured snippets** (Services): Pre-planning, Options comparison, Wishes recording, Family guidance
- Skip call extension unless you want phone calls; the funnel is WhatsApp.

## 7. Conversion tracking — set up BEFORE launch (non-negotiable)

Without this you can't optimize. Steps:
1. Create a **Google Ads conversion action** = "WhatsApp click" (category: Contact/Lead).
2. Add the **Google tag (gtag.js)** to all pages (in `<head>`).
3. Fire the conversion **on click of every `wa.me` button** (onclick event → `gtag('event','conversion',{...})`).
4. (Cleaner) send WhatsApp clicks to a `/thanks` page and count the pageview as the conversion.
5. Verify with Google Tag Assistant before spending.

> I can add the gtag + click-event code to the site once you have your Google Ads conversion ID.

## 8. KPIs & decision rules

Track daily:
- **CTR** (search target: aim >3–5%)
- **Avg CPC** (vs your Keyword Planner estimate)
- **WhatsApp opt-ins** and **cost per opt-in** ← the number that matters
- **Opt-in → real conversation rate**

**Decision after ~2–3 weeks / S$100–300:**
- Reasonable cost-per-opt-in + real conversations → **validated, scale budget** and add Chinese ads / more keywords.
- Clicks but ~0 opt-ins → **landing/trust problem** (usually identity/photo) — fix page, don't add spend.
- Few clicks / low CTR → **ad or keyword problem** — tighten copy/keywords.

## 9. Pre-launch checklist

- [ ] Website blockers fixed (see `website-audit.md`: identity, tracking, PDF+reply plan)
- [ ] Real domain live
- [ ] Conversion tracking verified
- [ ] Keyword Planner CPC/volume checked
- [ ] Negatives added
- [ ] RSAs + all assets set
- [ ] Budget cap + max CPC set
- [ ] WhatsApp Business greeting/auto-reply ready

## Compliance (confirmed)

Keyword-based **Search** ads for funeral/columbarium are **allowed**. The bereavement restriction only bans *personalized/remarketing/Customer-Match audience targeting* — we don't use it. Keep ad copy respectful (no fear/grief exploitation). Sources: Google Advertising Policies — "Restricted targeting in personalised advertising" and "Sensitive events".
