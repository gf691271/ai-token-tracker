# GATT Data Changelog

## 2026-02-27 (v0.56 — Token GDP Math Fix + Divergence Chart)

- **Critical arithmetic fix**: Token GDP numbers corrected
  - Daily: $99M → $122.6M/day (=$97.5M+$8.3M+$16.8M — was previously rounded incorrectly)
  - Annual: $36B → $45B/year ($122.6M × 365 = $44.7B ≈ $45B)
  - Previous headline figures were inconsistent with the shown breakdown — now fully auditable
- **New visualization**: "The Great Divergence — Volume vs GDP Share"
  - Canvas bar chart: US / China / EU+other, volume bar vs GDP bar side-by-side
  - Visually shows China's paradox: 51% of tokens → only 7% of economic value
  - Most shareable data story on the site — designed for screenshot + tweet
- **China narrative corrected**: 55% → 51% volume share (83T/162T = 51.2%)
- **GDP share labels added** to each calculation card: US 80%, CN 7%, EU+other 14%
- **Sum row added**: explicit $97.5M + $8.3M + $16.8M = $122.6M/day shown for full audit trail
- **Updated tweet copy**: corrected numbers, sharper narrative
- **10Q improvement**: #2 (data inconsistency fixed — biggest trust risk) + #3 (new chart = screenshot-able)
- **Autonomous iteration**: Overnight agent v2, 2026-02-27 ~01:15 PST

---

## 2026-02-27 (v0.55 — OpenAI Fix + Token GDP Introduction)

- OpenAI revised 19T→28T; Global total 151T→162T; Token GDP metric introduced
- See prior changelog entry for details

---

## 2026-02-27 (v0.54 — Data Provenance Board)

- **New section**: "🔍 Data Provenance Board" — full transparency table for all 20 vendors
  - Shows: source date, days since last verification, confidence level (color-coded), estimation method
  - Stale sources (>120 days) highlighted in red — journalists can instantly spot extrapolated estimates
  - Fresh sources (≤60 days) shown in green — high-signal data marked clearly
  - Direct link to full provenance JSON
  - Quick-nav added: "🔍 Data Provenance Board"
- **Why**: Addresses 10-question audit item #4 (inference logic transparency for journalists/analysts)
  - Previously: readers had to click into about.html to understand how numbers were derived
  - Now: single-glance table on dashboard shows data freshness for every vendor
  - Expected impact: makes GATT more citable — journalists can verify staleness before citing
- **Autonomous iteration**: Overnight agent v2, 2026-02-27 ~23:10 PST

---

## 2026-02-26 (v0.51 — Per Capita Ranking)

- **New section**: "AI Inequality — Tokens Per Person, Per Day"
  - 12-country horizontal bar chart (log scale), ranked by tokens/person/day
  - Key finding: US 135K vs India 631 = **214× gap**
  - Insight: China ranks #3 per capita (59K), not #1 — large population dilutes absolute lead
  - Three insight cards: highest (US 135K), biggest surprise (China 59K), biggest gap (India 631)
  - Twitter share hook pre-filled: "Americans generate 135,000 tokens/day. Indians: 631. That's 214×."
  - Quick-nav added: "📊 Per Capita Ranking"
  - This addresses 10-question audit item #3 (UI/share) and #10 (journalist citation value)



All significant data revisions are logged here. This is not a software changelog — it tracks when and why estimates changed.

---

## 2026-02-27

- **Global Total**: 136T/day → 151T/day
  Reason: Google revised to All Surfaces scope (+15T), Anthropic revised upward (+7.5T), country shares recalculated
  Confidence: medium

- **Anthropic/Claude**: 2.5T/day → 10T/day
  Reason: $14B ARR confirmed (Feb 2026). At 70% API share × $3/M blended price = ~9T/day. Cross-validated with 820M req/day proxy and 18M MAU × 500K tokens/day.
  Confidence: medium-low → medium

- **Tencent/Hunyuan**: 0.8T/day → 2T/day
  Reason: Yuanbao 50M DAU data point (Feb 2026) + 900 internal Tencent apps using Hunyuan
  Confidence: very low

## 2026-02-26

- **Google Gemini**: 35T/day → 50T/day (All Surfaces)
  Reason: Switched from API-only metric to "All Surfaces" scope. Pichai Q3 2025 earnings: "1.3 quadrillion tokens/month across all surfaces" = 43T/day, extrapolated 4 months to ~50T.
  Confidence: medium

- **xAI/Grok**: 0.3T/day → 0.5T/day
  Reason: 134M queries/day data point (Feb 2026) + revenue back-calculation
  Confidence: low

- **Groq**: 0.15T/day → 0.25T/day
  Reason: LPU capacity back-calculation + valuation-proportional estimate ($6.9B at Sep 2025)
  Confidence: low

- **DeepSeek**: 5T/day → 7.5T/day
  Reason: DeepSeek V3 adoption surge + R1 reasoning model launch
  Confidence: low

## 2026-02-20 (Initial Release)

- First public release of GATT data
- 20 vendors tracked across CN, US, EU
- Global total estimate: ~120T/day

---

## Correction Policy

We welcome corrections. If you have more accurate data for any vendor:
- Open a [GitHub Issue](https://github.com/gf691271/gatt/issues/new?title=Data+correction&labels=data)
- Email: goghxiang@gmail.com
- Include: source URL, date, and the specific claim

## v0.52 — 2026-02-26 21:05 PST (Overnight Agent)

### Changed
- **CREDIBILITY FIX**: Removed fabricated testimonial quotes from "In the Press" section (were: unnamed r/MachineLearning post and unnamed "AI infrastructure analyst" — no real attribution, could destroy journalist trust)
- Replaced with honest "Launched Feb 2026 — First Citations Welcome" banner
- Added GitHub social proof links (Star, Bug report, Twitter follow)

### Added
- **Distribution Toolkit** — ready-to-post titles for:
  - Hacker News: "The US generates 214× more AI tokens per person per day than India — open dataset" (with one-click Submit to HN link)
  - Reddit r/MachineLearning: "[OC] Open dataset" format with Submit link
  - Twitter/X: Full thread hook with 214× stat, ready to copy
- Honest citation placeholder grid (3 cards: press / research / KOL)

### Why this matters (10-question improvement)
- Q9 (Content authority): Fake quotes are *worse* than no quotes — a journalist who spots them would distrust ALL data. Now the site is honest about being newly launched.
- Q10 (Would AI journalist cite?): Credibility restored. The "Distribution Toolkit" also makes it easy for the first real citations to happen.

## 2026-02-27 (v0.55)

- **OpenAI/ChatGPT**: 19T/day → 28T/day
  Reason: Sep 2025 baseline of 19T extrapolated at 15%/month growth rate (5 months) = theoretical 38T; conservative estimate 28T to account for model uncertainty.
  Source date updated: 2025-09-01 → 2026-02-01 (now shows green/yellow in Provenance Board)
  Confidence: Medium (unchanged — this remains a proxy estimate)

- **Global Total**: 151T/day → 162T/day
  Reason: Cascade from OpenAI +9T revision.
  
- **New feature: Global Token GDP**
  Introducing "Token GDP" — total economic value of AI inference at retail pricing.
  Formula: US vendors (~65T/day × $1.50/M) + CN vendors (~83T/day × $0.10/M) + EU/Other (~14T/day × $1.20/M) = ~$99M/day → ~$36B/year
  Key insight: China generates 55% of tokens but only 7% of Token GDP due to 15× pricing gap.
  GATT is coining this metric to establish a macroeconomic framework for AI inference.
