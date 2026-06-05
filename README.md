# Own — Go-to-Market & Marketing Operating System

> Help Uzbekistan's merchants **own** their commerce instead of renting it from marketplaces.

This repository is the **marketing and go-to-market (GTM) brain** for **Own**, an e-commerce infrastructure company building the commerce operating system for merchants in Uzbekistan. It is a **documentation repository** — there is no application code here. Everything is Markdown: strategy, playbooks, campaigns, brand voice, competitive research, content drafts, and the measurement system used to take Own from its first design partners to **1,000 merchants**.

If this is your first time here, read this page top to bottom, then open [`docs/playbook/README.md`](docs/playbook/README.md).

---

## What is Own?

**One-liner:** Own helps Uzbekistan merchants launch reliable e-commerce infrastructure faster, with hands-on onboarding and operational clarity.

- **Category:** E-commerce infrastructure / merchant operating system (B2B SaaS with high-touch onboarding in early phases).
- **The thesis:** E-commerce in Uzbekistan is maturing. The company that wins will be the **full-stack operating system** merchants rely on from launch to transaction — storefront, Telegram, local payments (Humo / Uzcard / Payme / Click), delivery (BTS, Yandex), fiscalization, and data residency as **one designed experience**, not a dozen duct-taped plugins.
- **The wedge:** Be **10x better at one job** — *time from signed → live → transacting* — for a narrow merchant ICP, then expand surface area once activation is repeatable.
- **The moat:** Local depth and trust — the rails, compliance, and operational data a foreign giant structurally cannot replicate fast.
- **The goal:** **1,000 merchants** via phased GTM execution (first 10 → 100 → 1,000).

For the full product context (audience, personas, objections, positioning), see [`.agents/product-marketing-context.md`](.agents/product-marketing-context.md).

---

## How this repository is organized

The repo has two layers:

1. **`docs/` — the strategy and operating system.** The playbook (phases), the 6-month execution plan, and strategy notes. This is where decisions are made and tracked.
2. **Root workstream folders — the workshops.** Each functional area (brand, campaigns, competitive research, content, analytics, SEO, sales) has its own folder with a `README.md` explaining its purpose. The playbook **pulls from** these folders and **pushes decisions back** into them.

```
.
├── README.md                       ← you are here
├── brief.md                        ← short pointer into the playbook
├── CONTRIBUTING.md                 ← how to update docs (ownership, review, naming)
├── founder-team-thesis-alignment.md← founding-team alignment worksheet
│
├── docs/                           ← STRATEGY & OPERATING SYSTEM
│   ├── playbook/                   ← phased GTM playbook (start here)
│   │   ├── README.md               ← playbook index + phases 0–3
│   │   ├── phase-0-foundation.md
│   │   ├── phase-1-first-10.md
│   │   ├── phase-2-first-100.md
│   │   ├── phase-3-first-1000.md
│   │   ├── operating-cadence.md    ← weekly/monthly/quarterly rituals
│   │   ├── governance-raci.md      ← decision rights
│   │   └── open-questions-register.md ← unresolved assumptions + decisions
│   ├── plan-6m/                    ← month-by-month execution roadmap (M1–M6)
│   └── strategy/                   ← strategy notes (e.g. operating-principles.md)
│
├── brand-voice/                    ← how Own sounds (voice guide, language matrix)
├── brand-review/                   ← how content gets checked (rubric, review log)
├── campaigns/                      ← campaign briefs per phase + calendar
├── competitive-analysis/           ← market map, signals tracker
├── competitive-brief/              ← battlecard template
├── competitor-profiles/            ← Shopify / WooCommerce / Uzbekistan landscape + raw research
├── content-creation/               ← drafts: paid ads, social (Instagram, LinkedIn)
├── landing-pages/                  ← landing page copy (e.g. merchant signup)
├── performance-analytics/          ← KPI tree, funnel definition, experiments log, reporting
├── sales-enablement/               ← sales decks and collateral
└── seo-audit/                      ← keyword universe + technical audit
```

> Almost every folder contains its own `README.md` describing its purpose and what belongs in it. When in doubt, open the folder's README first.

---

## The playbook: the road to 1,000 merchants

The core of this repo is a **phased GTM playbook**. Each phase answers the same five questions: **Goal · ICP focus · Motion · Channels & content · Exit criteria.**

| # | Phase | Goal |
|---|-------|------|
| 0 | [Foundation](docs/playbook/phase-0-foundation.md) | Sharpen positioning, ICP, and offer enough to sell. |
| 1 | [First 10 — Design partners](docs/playbook/phase-1-first-10.md) | Hand-pick 10 merchants who co-build with us. |
| 2 | [First 100 — Early adopters](docs/playbook/phase-2-first-100.md) | Prove the motion repeats without the founder in every conversation. |
| 3 | [First 1,000 — Scaled](docs/playbook/phase-3-first-1000.md) | Industrialize a channel mix for predictable acquisition. |

Running alongside the phases is a **[6-month execution roadmap](docs/plan-6m/README.md)** (Month 01 → Month 06), which translates strategy into monthly priorities.

The strategic spine is [`docs/strategy/operating-principles.md`](docs/strategy/operating-principles.md) — "the Own play": **Apple's integrated craft × Google's default distribution + data flywheel × Shopify's mission and aligned incentives**, all built on a local moat.

---

## How to use this repo (by role)

- **New to the project?** Read this README → [`docs/playbook/README.md`](docs/playbook/README.md) → the current phase doc.
- **Founder / strategy:** [`founder-team-thesis-alignment.md`](founder-team-thesis-alignment.md) and [`docs/strategy/operating-principles.md`](docs/strategy/operating-principles.md).
- **Running execution week to week:** [`docs/plan-6m/`](docs/plan-6m/) + [`docs/playbook/operating-cadence.md`](docs/playbook/operating-cadence.md).
- **Writing copy or content:** start in [`brand-voice/`](brand-voice/), draft in [`content-creation/`](content-creation/), then check against [`brand-review/`](brand-review/).
- **Researching the market:** [`competitive-analysis/`](competitive-analysis/), [`competitor-profiles/`](competitor-profiles/), [`competitive-brief/`](competitive-brief/).
- **Measuring results:** [`performance-analytics/`](performance-analytics/) (KPI tree, funnel definition, experiments log).

---

## Working conventions

A few conventions keep this repo coherent (full version in [`CONTRIBUTING.md`](CONTRIBUTING.md)):

- **One document, one purpose.** Keep docs focused; use kebab-case filenames.
- **Every active doc names a single owner (DRI)** and, where relevant, a success metric and review cadence.
- **Decisions are tracked, not silently overwritten.** When an assumption changes, log it in [`docs/playbook/open-questions-register.md`](docs/playbook/open-questions-register.md) and keep changelog rows where present.
- **Strategy and execution stay in sync.** Every strategy change should show up in the execution docs (and vice versa).
- **`[unknown]` / `[to-validate]` markers are intentional.** They flag open questions that still need a decision — don't delete them, resolve them.

---

## Status

Working scaffold. The phase structure (10 → 100 → 1,000) is a default to be revised once real ICP, timeline, and budget numbers are agreed. Several top-level unknowns (north-star metric, timeline, geographic scope, language posture) are tracked in the [playbook index](docs/playbook/README.md) and the [open-questions register](docs/playbook/open-questions-register.md).
