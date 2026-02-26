# GATT — Global AI Token Tracker

**The open index tracking the global Token Economy.**  
AI inference as commodity, currency, and geopolitical force.

🌐 **Live Dashboard** → [gf691271.github.io/ai-token-tracker](https://gf691271.github.io/ai-token-tracker/)

---

## What is GATT?

Just as the original GATT (General Agreement on Tariffs and Trade) mapped the flow of physical goods across borders, **GATT tracks the flow of AI tokens** — the first true commodity of the AI Agent era.

Token consumption tells you:
- Which AI vendors are winning the inference war
- Which countries are accelerating (or falling behind) in AI adoption
- How cheap electricity translates into cheap tokens and geopolitical leverage
- What the real compute gap is between the US and China — before and after normalization

> *"Token is the first real commodity of the internet industry. Cross-border, currently untaxed. Short-term: a play on models and inference chips. Long-term: electricity and bandwidth arbitrage."*  
> — [@turingou](https://x.com/i/status/2023513968946672011), 162K impressions

---

## The Token Consumption Index (TCI)

GATT publishes a **three-tier ranking** of global AI vendors by token consumption:

| Tier | Criteria | Vendors |
|------|----------|---------|
| **Tier 1** | Direct data, verified | 11 vendors incl. Google, ByteDance, OpenAI |
| **Tier 2** | Estimated range | 7 vendors incl. Anthropic, Microsoft, DeepSeek |
| **Tier 3** | Data black hole | 11 vendors incl. Tencent, xAI, Ollama |

**Key findings (Feb 2026):**
- 🌍 Global daily tokens: **~100 trillion**
- 🇨🇳 China share by volume: **~55%** — but only ~14% by compute value
- 🇺🇸 US compute value lead: **$35M DEC/day** (OpenAI alone: $32.5M)
- 📈 Fastest-growing: **Doubao** (ByteDance) — 120B/day → 50T/day in 18 months (+417×)

*DEC = Dollar-Equivalent Compute (GATT's normalized unit, benchmarked to GPT-4o)*

---

## Why This Matters

Token consumption is becoming as strategically important as oil consumption was in the 20th century:

- **Governments** will start subsidizing token costs (already happening in China)
- **Countries with cheap electricity** can produce cheap tokens and export AI compute
- **Token trade balance** will become a geopolitical metric alongside GDP
- **The gap between raw volume and compute value** reveals tokenizer efficiency differences between Chinese and Western AI models

---

## Data Sources (MVP)

| Source | Signal |
|--------|--------|
| OpenRouter rankings | Real-time model usage distribution |
| HuggingFace downloads | Open-source adoption velocity |
| Ollama / Docker Hub pulls | Local inference footprint |
| Company disclosures | Official announcements, earnings, blog posts |
| Revenue back-calculation | Inferred token volume from reported revenue |

**V2 sources (planned):** Cloudflare AI Gateway reports · GPU sales data · Electricity consumption by datacenter region

---

## Methodology

### Standardized Token (ST)
All token counts are normalized to **GPT-4o equivalent tokens** to enable apples-to-apples comparison across vendors with different tokenizers. Chinese models (e.g., Doubao, Ernie) use more tokens per Chinese character — raw numbers overstate their volume vs. Western models.

Toggle between **Raw Mode** and **Standardized Mode** in the dashboard.

### DEC (Dollar-Equivalent Compute)
Converts token volume to economic value using each model's API pricing. Reveals the value of compute, not just the quantity.

---

## Dashboard Features

- 📊 **Token Consumption Index** — ranked leaderboard by vendor
- 📈 **Daily trend chart** — China / US / Rest of World over time
- 🌍 **Regional breakdown** — volume vs. compute value comparison
- 🔀 **Raw ↔ Standardized toggle** — see the tokenizer gap
- 🌐 **EN / 中 language toggle**
- 📡 Updated daily

---

## Roadmap

- [ ] **V1** — Static dashboard, manual data updates (current)
- [ ] **V2** — Automated pipeline: OpenRouter + HuggingFace + scraper
- [ ] **V3** — API endpoint for AI agents (`GET /api/tci`)
- [ ] **V4** — Weekly Token Economy Report (newsletter + social)
- [ ] **V5** — Predictive model: token growth by country/vendor

---

## Contributing

Found a data source we missed? Open an issue or PR.  
Especially looking for: official API usage numbers, earnings call transcripts, datacenter energy data.

---

## About

Built by **Frank Gao** — cross-border AI strategist, ex-Alibaba / Microsoft / Nokia.  
Tracking the Token Economy so you don't have to.

🐦 [@goghxiang](https://x.com/goghxiang)

---

*GATT is an independent research project. Not affiliated with the WTO or any AI vendor.*
