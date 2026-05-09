# Uzbekistan E-Commerce Landscape — Deep Research v1

**Generated:** 2026-05-09
**Author of this pass:** desk research via web search + page fetches inside Cursor (no Firecrawl / DataForSEO in this run)
**Raw sources:** [`raw/_desk-research/2026-05-09/uzbekistan-sources.md`](raw/_desk-research/2026-05-09/uzbekistan-sources.md)
**For:** NOLBIR (see `.agents/product-marketing-context.md`)

> Treat numbers as **ranges from public secondary sources**. Different reports (KPMG, ECDB, Statista, Asia-Plus) use different methodologies and years. Validate before quoting externally.

---

## TL;DR for NOLBIR

1. **Uzbekistan e-commerce is small but growing fast.** Total online retail moved from ~$311M (2022) to roughly **$1B (2023–2024)** to publicly cited **~$2.6B in 2025**, with KPMG projecting **$1.8–2.2B by 2027** at **~41–47% CAGR**. Online share of retail is still only **~5–10% (2025)** vs ~16% in Russia and ~14% in Kazakhstan — so the headroom is real.
2. **The market is consolidating around a few platform giants.** Uzum (local unicorn, full ecosystem), Wildberries, Ozon, AliExpress, plus Yandex services in delivery. The Competition Committee has already labelled multiple players “dominant” and is enforcing antitrust compliance.
3. **The merchant tooling layer is fragmented and immature.** Storefront builders (Robosell, OsonDokon, Magicstore, Magicbot, Delever) are mostly **Telegram-bot-first** or **vertical (HoReCa)**. A real “Shopify of Uzbekistan” for serious SMB merchants is **not yet locked in**.
4. **Telegram is the de facto first storefront** for many SMBs (~18M active users, ~740M channel reach reported in vendor materials). Any merchant infra that ignores Telegram will lose to one that integrates it natively.
5. **Payments rails are local (UZCARD + HUMO) and consolidated** around Click and Payme. Foreign processors are not realistic without partners.
6. **Logistics are oligopolistic.** Uzum Tezkor, Yandex Eats, Express24 (now consolidated with Yandex) and BTS Express dominate. FBS-style models are emerging.
7. **Regulatory pressure is rising for foreign operators** (12% VAT on B2C digital services since 2020; **Resolution 885** from Dec 2024 requires e-commerce operators to be **Uzbek resident legal entities** from **July 1, 2025**). This **structurally favours local infrastructure**.

**NOLBIR’s strategic window:** be the **operational e-commerce backbone for serious local merchants** in the gap between (a) marketplace dependence and (b) DIY Telegram bots / global SaaS that doesn’t fit local rails or rules.

---

## 1. Market sizing and trajectory

| Metric | Value | Source / year |
|--------|-------|---------------|
| E-commerce GMV | ~$311M | 2022 (KPMG) |
| E-commerce GMV | ~$1B | 2023–2024 (Asia-Plus / Wildberries-cited reports) |
| E-commerce revenue | ~$2,649M | 2025 (ECDB) |
| Forecast | $1.8–2.2B by **2027** | KPMG (2022–2027 CAGR 41.4–47.4%) |
| Online share of retail | ~5–10% | 2025 |
| Online share of retail (2027 forecast) | ~9–11% | KPMG |
| Internet penetration | ~77% (2022) → ~87% (2023) | KPMG |

**Reading this:**
- The “$1B vs $2.6B in the same year” gap reflects different definitions (cross-border platform GMV vs total online consumer spending) and different reporters. Use **directional growth**, not single point claims.
- Even at the conservative end, the market is **multiplying ~5–7x in 5 years**. Late entrants will face platform lock-in fast.

---

## 2. Marketplaces (the “demand side” NOLBIR’s merchants depend on)

| Player | Type | Notes (public reporting) |
|--------|------|--------------------------|
| **Uzum Market** | Local marketplace + ecosystem | First Uzbek tech unicorn; ~17,000+ sellers, 1M+ SKUs; FBS model launched late 2024; bank, BNPL, delivery (Tezkor) all in-house; >50% of population reportedly using services |
| **Wildberries** | Cross-border marketplace (RU origin) | Major channel for Uzbek goods; 2024 sales ~$673M; 2025 9-month sales +37% YoY; **export channel** to RU/KZ/BY/KG/AM as much as a domestic one |
| **Ozon** | Cross-border marketplace (RU origin) | Active in Uzbekistan as one of the “top” marketplaces |
| **AliExpress** | Cross-border marketplace | Long-standing inbound demand for cheap goods |
| **Zoodmall / ZoodPay** | Marketplace + BNPL | Active in 2024 (Q1 NMV +71%, MAU ~800K), but Competition Committee opened a case against ZoodPay; treat status as **monitor closely** |

**Implication for NOLBIR:**
- Many merchants will **not abandon marketplaces** — they need them for traffic.
- Real value lives in **multichannel inventory + order management**: marketplaces *and* own store, including Telegram, with one source of truth.
- “Independence from Wildberries / Uzum margins” is a credible **emotional pain** for ambitious SMBs.

---

## 3. Local merchant SaaS / storefront builders (NOLBIR’s nearest competitors)

| Platform | Wedge | Notable scale claims (vendor-reported) | Tells us |
|----------|-------|----------------------------------------|----------|
| **Robosell** (`robo.uz`) | Site + Telegram bot in 15 min, multi-country | 10K+ users, 20K+ sites/bots | Closest “generalist” builder competitor |
| **OsonDokon** (`osondokon.uz`) | AI-powered builder, 5-min setup, multi-language UZ/RU/EN | Integrations with Payme/Click/Stripe, Telegram mini-app | AI-native pitch; lower switching cost |
| **Magicstore / Magicbot** (`magicstore.dev`, `magicbot.uz`) | Telegram store in 5–15 min, AI assistant, integrates with Payme/Click/Uzum/Alif/Octo/Mohirpay | 500+ stores, 50K+ orders | Pure Telegram-first wedge |
| **Delever** (`delever.uz`) | HoReCa: site + bot + app under merchant brand, POS + delivery | 1,200+ businesses, +45% revenue claim | Vertical (food); proves vertical depth wins |
| **Click Business mini-apps** | Storefront via Click SuperApp | Distribution via Click | Demonstrates how payments players bundle commerce |
| **Botcommerce (IT Park)** | No-code social commerce (Telegram + WhatsApp) | Pandemic-era origin; expansion plans | Confirms social-commerce demand |

**Pattern:** All of these are either (a) **Telegram-first / no-code**, (b) **vertical** (HoReCa), or (c) **bundled with payments**. **None is a serious end-to-end commerce backbone for SMBs scaling to multi-channel + own logistics + ERP-grade ops.** That is the gap NOLBIR can credibly own.

---

## 4. Payment rails

| Element | Reality |
|---------|---------|
| Local card schemes | **UZCARD** and **HUMO** dominate — anything for local merchants must support both |
| Top consumer/merchant gateways | **Click** (claims ~20M users, ~30K merchants) and **Payme** — both offer free merchant onboarding, QR payments, banking-day settlement |
| BNPL | **Uzum Nasiya** (cited 40% market share), Alifpay, Zood — installments are a major **conversion lever**, not a nice-to-have |
| International cards | Possible via local acquirers + Stripe-style integrations (e.g. OsonDokon mentions Stripe), but secondary |
| Settlement | Typically T+1 banking day for Click/Payme |

**Implication for NOLBIR:** “Payments out of the box with Click + Payme + UZCARD/HUMO + at least one BNPL” is **table stakes**. Skipping BNPL is a real conversion hole.

---

## 5. Logistics

| Layer | Players |
|-------|---------|
| Marketplace-tied delivery / pickup | **Uzum Tezkor** (declared dominant April 2025), **Wildberries** PVZ network |
| Independent last-mile / on-demand | **Yandex Go** (Market + courier + intercity), formerly **Express24** (Yandex acquired its assets Oct 2024 — both declared dominant for food delivery) |
| 3PL / fulfilment | **BTS Express** (3PL, 34 settlements, 24/7) |
| FBS for marketplaces | **Uzum Market FBS** launched Oct 2024 — sellers ship from their own warehouses while Uzum handles storefront and last mile |

**Implication for NOLBIR:**
- The **dominance rulings** mean major couriers face antitrust scrutiny — partnerships are possible but pricing power is shifting.
- A merchant backbone that **abstracts shipping providers** (BTS, Yandex, Uzum, custom couriers) is more defensible than one tied to a single carrier.
- Multi-warehouse + FBS workflows are now a **legitimate selling point** for tools.

---

## 6. Regulation (this is a moat, not just a constraint)

- **VAT 12% on B2C digital services from foreign providers** (since Jan 2020). 60+ foreign internet companies are now registered. Tax authority is actively enforcing in 2024–2025.
- **Resolution 885** (Dec 26, 2024) — from **July 1, 2025**, e-commerce operators (electronic trading platforms, order aggregators) **must be Uzbek resident legal entities**, follow local rules on data, consumer rights and retail trade, and use **separate bank accounts** for e-commerce flows.
- Self-employed e-commerce sellers will be tracked as **turnover taxpayers** based on account credit data — this raises both compliance burden and demand for **clean financial reporting tooling**.

**Implication for NOLBIR:**
- Foreign SaaS (Shopify, BigCommerce, etc.) becomes structurally harder to use as a **system of record** for Uzbek merchants.
- A **locally registered, locally compliant** infrastructure provider has a defensible position.
- “We help you stay compliant with the new e-commerce operator rules” is a real selling line, not marketing fluff — verify legal phrasing with counsel before publishing.

---

## 7. Consumer behaviour signals

- Telegram is huge: vendor materials cite **~18M active users** and **~740M channel reach**; small businesses default to Telegram over websites.
- **Three-language reality:** Uzbek (Latin and Cyrillic), Russian, sometimes English. Robosell, OsonDokon, etc. all advertise UZ/RU support.
- **Trust drivers:** local payment, BNPL, fast delivery, voice-of-friend (Telegram channels), willingness to pay cash on delivery in some segments.
- **Pricing sensitivity is high** but **convenience monetization works** (BNPL, delivery, returns).

---

## 8. Competitive map for NOLBIR

```
                  Marketplace dependency
                         │
           Uzum / WB / Ozon / AliExpress
                         │
                  ┌──────┴──────┐
   Telegram-only  │             │   Multi-channel + own ops
   bots & no-code │             │   (NOLBIR’s play)
                  │             │
          Magicstore /          NOLBIR (proposed)
          Magicbot /            ────────────
          Botcommerce           Robosell (broad/light)
          Robosell (light)      OsonDokon (broad/light, AI)
                  │             Delever (HoReCa, vertical)
                  └──────┬──────┘
                         │
                Foreign SaaS: Shopify / WooCommerce
                (now compliance-disadvantaged after Res. 885)
```

**Where NOLBIR can win:**
- “**Operational backbone** for multichannel SMB commerce in Uzbekistan: own store + Telegram + marketplaces + local payments + local delivery + compliance-ready accounting flows.”
- Phase 1 ICP (per playbook): **digital-first SMB merchants** who already have a Telegram store and either sell on Wildberries/Uzum or want to.

---

## 9. Strategic implications and watch-list

**Implications**
1. **Position against marketplaces, not platforms.** The pain to articulate: margin squeeze, no customer relationship, opaque algorithmic exposure. Backbone tooling lets merchants build a brand and not depend on Uzum/WB rankings.
2. **Telegram is non-negotiable.** First-class Telegram store is required, not a side feature.
3. **Payments + BNPL + multi-marketplace inventory** is the **functional MVP** for a credible merchant backbone.
4. **Compliance is a selling line.** Especially for merchants nervous about Resolution 885 and turnover-tax flows.
5. **Vertical wedge first** (e.g. apparel, beauty, electronics, or food/HoReCa) likely beats horizontal pitch — Delever shows vertical works.
6. **Language posture:** Uzbek-Latin primary, Russian fully mirrored, Cyrillic where needed. Brand voice already says “practical / no hype” — that fits this market.

**Risks / watch-list**
- Uzum extending downstream (their FBS launch is a direct threat to independent backbones).
- Click / Payme launching commerce mini-apps / store builders themselves (Click is already doing this).
- Yandex bundling commerce on top of consolidated logistics.
- Foreign players (Shopify, Wix, etc.) localizing aggressively despite Resolution 885 friction.
- New regulatory turns from the Competition Committee that reshape who can do what.

---

## 10. What to do next (suggested follow-ups)

1. **Pick 3–5 named competitors for full profiles** with the competitor-profiling skill: at minimum **Robosell, OsonDokon, Magicstore, Delever**, and one of **Click Business / Magicbot**. Run Firecrawl + DataForSEO when available.
2. **Talk to 5–10 merchants who currently sell on Telegram + Uzum + Wildberries.** Capture verbatim language for the `.agents/product-marketing-context.md` "Customer Language" section.
3. **Map the regulatory checklist** (VAT, Res. 885, data, tax) into a one-pager you can ship as a lead magnet.
4. **Decide vertical wedge** (apparel? home goods? HoReCa-adjacent? B2B wholesale?) — this drives ICP, partnerships, and integrations.
5. **If you want a second deep-research pass from another model (Claude Code or Gemini)**, give them this document plus `raw/_desk-research/2026-05-09/uzbekistan-sources.md` and ask specifically for: (a) **Uzbek-language sources** I likely under-weighted, (b) **primary government data** from `stat.uz`, `raqobat.gov.uz`, `it-park.uz`, (c) **merchant interviews / forum mining** I cannot do here.

---

## 11. Limitations of this v1

- No Firecrawl / DataForSEO (no domain ranks, backlink data, ranked keywords).
- No Uzbek-language source sweep (Latin or Cyrillic), only what surfaced in English/Russian web search.
- Vendor-reported numbers (Uzum, Wildberries, Magicstore, Robosell) used as positioning evidence, not independent measurement.
- Regulatory reading is **journalist-level**, not legal advice; a Tashkent counsel review is required before publishing claims.
- “What merchants actually say” is missing — primary research (interviews, Telegram channels, reviews) is the most valuable next step.

---

## Raw data sources

See [`raw/_desk-research/2026-05-09/uzbekistan-sources.md`](raw/_desk-research/2026-05-09/uzbekistan-sources.md) for full URL list grouped by topic.
