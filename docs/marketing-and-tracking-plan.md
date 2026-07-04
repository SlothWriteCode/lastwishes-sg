# Marketing & Tracking Plan — SEO, channels, and "don't waste money"

_Date: 2026-07-04 · Companion to `google-ads-plan.md`, `website-audit.md`, `options-landscape.md`. Principle: **set up measurement BEFORE spending, and agree the fail-fast rules up front** so a loss gets cut early instead of bleeding._

---

## PART A — Measurement first (this is how money is not wasted)

Rule: **no dollar of ad spend and no hour of SEO goes out until tracking is live.** If you can't measure it, you can't tell success from failure — and that's how budgets disappear.

### A1. The tracking stack (all free)
| Tool | What it tells you | Covers |
|---|---|---|
| **Google Analytics 4 (GA4)** | Visitors, where they came from, what they clicked, conversions | All traffic |
| **Google Search Console (GSC)** | Which searches show/click your site, ranking position, indexing | SEO |
| **Google Ads conversion tracking** | Which keyword/ad produced a WhatsApp lead | Ads |
| **WhatsApp-click events** | The core conversion — tour enquiry + checklist | Both |
| **UTM tags on every link** | Exact source of each visit (`?utm_source=google&utm_medium=cpc&utm_campaign=tour`) | Everything |
| **Weekly scoreboard** (one spreadsheet) | The 6 numbers below, tracked over time | Whole business |

### A2. The ONE number that matters
**Cost per WhatsApp lead** (a tour enquiry). Everything else is diagnostic. Secondary: lead → reply → tour booked → sale.

### A2b. Anchor your kill line to YOUR economics (do this first — fixes audit #1)
A "good" or "bad" cost-per-lead is meaningless until you know what a customer is worth. Plug in two numbers:

```
Max you can pay per lead  =  commission per sale  ×  lead→sale close rate  ×  0.5
                             (the 0.5 keeps roughly half as profit/margin buffer)
```

**Fill these in:**
- Commission per Nirvana sale: **S$[____]**   ← ask/estimate
- Lead → sale close rate: **[____]%**   ← rough guess is fine (e.g. 1 in 20 = 5%)

**Worked example** (illustrative only — replace with your real numbers):
- Commission S$2,000 × close rate 5% (1 in 20) × 0.5 = **max ~S$50 per lead** and still profitable.
- Commission S$2,000 × close rate 10% (1 in 10) × 0.5 = **max ~S$100 per lead**.
- Commission S$800 × close rate 5% × 0.5 = **max ~S$20 per lead** → this offer needs cheap leads to work.

**Then set the kill line at that number**, not the placeholder S$40–50 elsewhere in this doc. If your real max is S$100, don't kill a S$60 channel; if it's S$20, S$60 is already a loss.

### A2c. YOUR numbers (owner input: close rate 5%; commission varies by product)
Because commission depends on what sells, here's the ceiling **at a 5% close rate**, per *serious* lead (a real WhatsApp conversation from the lead log — not a raw click):

| Avg commission / sale | Break-even per lead (5%) | **Profitable target per lead (×0.5)** |
|---|---|---|
| S$500 | S$25 | **≤ S$12** |
| S$1,000 | S$50 | **≤ S$25** |
| S$2,000 | S$100 | **≤ S$50** |
| S$3,000 | S$150 | **≤ S$75** |
| S$5,000 | S$250 | **≤ S$125** |

**What this means for you:**
- **Cheap niches (low commission) barely support paid ads** — you'd need very cheap leads. The **higher-value sales are where ads clearly pay off.** So in your lead log, note *which product* each lead is interested in; a lead leaning toward an expensive niche is worth far more.
- **Conservative planning number for the first test:** assume ~S$1,000–1,500 average commission → aim to keep **cost per serious lead under ~S$25–35**. Translate to clicks: if ~1 in 8–10 clicks becomes a serious lead, your **max CPC ≈ S$3** — matches the S$2–2.50 cap in the ads plan.
- **The first test's real job:** discover your *actual* average sale value and close rate. Plan cautious, then let the lead log replace these estimates with real ones and reset the kill line.

### A2d. Recommended kill line for the first paid test
- Judge only after **~50–100 clicks** (fewer is statistical noise).
- **Pause** a keyword/ad if cost per *serious* lead is clearly above your target (≈ S$35 on the conservative assumption) and not improving.
- **Hard stop / fix the page** if **~80–100 clicks produce 0 serious leads** — that's a trust/offer problem, not budget.

### A3. Define the funnel as tracked events
```
Impressions → Clicks → Landing views → WhatsApp click (LEAD)
   → Reply → Tour booked → Sale
```
Track the drop-off at each arrow. The stage where people fall off tells you *what* to fix (traffic vs page vs offer vs your reply).

### A4. "Track my fail" — pre-agreed kill criteria
Decide these NOW, in the cold light of day, so you don't rationalise later. Suggested triggers:

**Google Ads**
- Spent **S$60 / ~30+ clicks with 0 WhatsApp leads** → **pause**. Problem is the page/offer, not the budget. Fix before spending more.
- **CTR < 2%** → ad copy or keyword problem (rewrite / tighten keywords).
- **Clicks fine, 0 leads** → landing-page trust/offer problem.
- **Cost per lead > ~S$40–50** and not improving after optimisation → this channel/keyword isn't viable; stop.

**SEO**
- **No GSC impression growth after ~8–10 weeks** of publishing → your pages aren't being seen for anything; change topics/keywords.
- **Ranking stuck > position 20 after 3–4 months** on your target long-tail terms → content isn't good/deep enough, or terms are too competitive.

**Weekly + monthly cadence**
- **Weekly:** update the scoreboard (10 min). Spot leaks early.
- **Monthly:** go/no-go per channel against the above. Kill losers, feed winners.

> The point of failure tracking isn't to feel bad — it's to **fail cheap and fast**, keep the S$40 mistakes from becoming S$400 ones, and pour money only into what's already proving itself.

---

## PART B — SEO plan (the free, slow, compounding channel)

### B0. Honest expectations
- The market is **saturated** with price-first competitors (nirvanafugui, singaporefuneralcare, funeralguru…). You will **not** rank for head terms like "columbarium singapore" for a long time, if ever.
- SEO pays off in **3–6+ months**, not weeks. It is the opposite of ads (slow build vs instant signal).
- **Your realistic SEO wins are long-tail, informational, non-price queries** where your genuinely-useful content beats thin competitor pages. That's where to aim.

### B1. Technical foundation (one-time, finishable — do this once)
- [ ] Real **domain** + HTTPS (static site already = fast, mobile-ready ✓)
- [ ] **sitemap.xml** + **robots.txt**
- [ ] Submit site to **Google Search Console** + **Bing Webmaster**
- [ ] Unique **title + meta description** per page (already in place ✓)
- [ ] **Structured data**: `FAQPage` schema on the guide/checklist, `LocalBusiness` schema once you have UEN/address
- [ ] Clean descriptive URLs, internal links between the 3 pages + future articles

### B2. Keyword targeting — go long-tail (winnable)
Target intent you can actually rank for and that feeds WhatsApp:
- "funeral planning checklist singapore"
- "what to do when someone dies in singapore"
- "public vs private columbarium singapore"
- **"can you buy a columbarium niche in advance singapore"** ← your unique angle (public niches are post-cremation only)
- "questions to ask before buying a columbarium niche"
- "ashes options singapore" / "sea vs inland ash scattering singapore"
- "how to avoid funeral overcharging singapore"

### B3. Content plan (lean — from assets you ALREADY have, don't over-produce)
Turn the vault + `options-landscape.md` into a **small set** of genuinely useful articles, published **steadily** (e.g. 1–2/month), not in a burst:
1. **Public vs Private Columbarium — which fits your family** (uses the sourced landscape)
2. **What to do when someone dies in Singapore** — stage-by-stage (captures urgent searchers)
3. **Ashes options compared** — home / columbarium / sea / inland (all sourced)
4. **Can you plan a columbarium niche in advance?** — the honest pre-planning-is-private-only angle (unique, high-converting)
5. **Questions to ask before buying a niche / avoid overpaying** (links the scam guide)

Each article: calm, sourced, ends with the free checklist + free tour CTA. This is the same content that helps SEO *and* converts — no wasted effort.

### B4. Local SEO — highest-ROI organic move
- **Google Business Profile** (needs a registered business; **no personal face required**). Wins "near me"/maps searches, shows reviews, adds huge trust. Set up once UEN exists.
- Ask happy families for **reviews** — the strongest face-free trust signal there is.

### B5. Off-page / authority (slow, optional)
- A few quality backlinks: relevant SG directories, and **partnerships** (see Part C). Don't buy spammy links.

### B6. SEO milestones
- **Month 1:** technical foundation + GSC live + 2 articles
- **Month 3:** 5–6 articles indexed, impressions climbing in GSC, GBP live
- **Month 6:** ranking on several long-tail terms, first organic WhatsApp leads
- Judge against the SEO kill criteria in A4.

---

## PART C — Other channels (brief, honest)
| Channel | Verdict |
|---|---|
| **Google Business Profile + reviews** | **Do it** — best organic ROI, no face needed |
| **Referral / partnerships** | High-value: eldercare centres, hospices, will-writing lawyers send warm leads. Worth pursuing |
| **Organic social** | You opted out of personal posting — noted. Only revisit via a brand account, not your face |
| **Email / retargeting** | Limited — Google/Meta restrict bereavement audience targeting; skip for now |

---

## PART D — The minimum to actually start (ADHD-friendly — do THIS, not everything)
Do not attempt the whole plan. In order:
1. **Measurement:** GA4 + GSC + Google Ads conversion + UTM links (half a day, one time)
2. **Domain** + sitemap + submit to GSC
3. **Launch the small ad test** (fast signal — the S$100–300 test in `google-ads-plan.md`)
4. **Publish 2 articles** from the list above
5. **Google Business Profile** once UEN is registered
6. **Weekly scoreboard**, judged against the kill criteria in A4

Ads = your fast signal. SEO + GBP = the slow compounding base. Measurement wraps both so nothing is spent blind and every failure is caught cheap.

---

### Weekly scoreboard template (copy into a sheet)
| Week | Ad spend | Clicks | CTR | Landing views | WhatsApp leads | Cost/lead | Tours booked | GSC impressions | Notes/action |
|---|---|---|---|---|---|---|---|---|---|
| | | | | | | | | | |
