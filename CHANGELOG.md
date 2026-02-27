# GATT Data Changelog

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
