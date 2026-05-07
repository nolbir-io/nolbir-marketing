# performance-analytics

How NOLBIR knows whether marketing is working — the KPI tree, the dashboards, the weekly read.

## Purpose

Define the metrics, instrument them, and report on them. Receives campaign goals from `campaigns/`, content output from `content-creation/`, and feeds learnings back to all three.

## Key questions to answer

- What's the north star — signed merchants, activated merchants, transacting merchants, GMV, something else?
- What does the funnel look like end-to-end — from "first touch" to "transacting merchant"? What are the conversion rates we'd accept at each stage?
- How do we attribute — last-touch, first-touch, multi-touch, self-reported? What's good enough at this stage?
- What's the reporting cadence — weekly ops review, monthly business review, quarterly?
- What's a "leading indicator" we can react to in days, not months?

## Unknowns — needs playbook

- [unknown] Definition of "merchant" milestone (signed vs. live vs. transacting)
- [unknown] Data sources — CRM, GA / analytics, payment data, manual tracker
- [unknown] CAC and payback targets
- [unknown] Reporting tools and ownership

## What goes here next

- `kpi-tree.md` — north star → inputs → leading indicators
- `funnel-definition.md` — stages, definitions, target conversion
- `dashboards/` — specs for whatever tool we use
- `weekly-report-template.md` — the standing read
- `experiments-log.md` — what we tested, what we learned
