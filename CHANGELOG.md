# GATT Data Changelog

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
