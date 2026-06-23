# Social posts

Channel-specific post drafts for Own. Source-of-truth for what we publish on Instagram and LinkedIn.

## Folder layout

```
social/
  README.md                # this file — conventions
  calendar.md              # master cross-channel timeline
  instagram/
    YYYY-MM.md             # all Instagram posts in a given campaign batch
  linkedin/
    YYYY-MM.md             # all LinkedIn posts in a given campaign batch
  telegram/
    YYYY-MM.md             # all Telegram posts in a given campaign batch
  x/
    YYYY-MM.md             # all X posts in a given campaign batch
  facebook/
    YYYY-MM.md             # all Facebook posts in a given campaign batch
  _archive/                # closed months / superseded drafts
```

## Naming convention

- One file per channel per campaign-batch month: `social/instagram/2026-06.md`
- File month = the month the batch *starts*. If a few posts in the batch publish in early next month, they stay in the start-month file. A new file is created when the next month has its own batch worth of posts.
- Each post inside the file gets a stable ID: `IG-YYYY-MM-NN` / `LI-YYYY-MM-NN` / `TG-YYYY-MM-NN` (Telegram) / `X-YYYY-MM-NN` (X) / `FB-YYYY-MM-NN` (Facebook).

## Post header format

Every post inside a monthly file starts with this header so it's greppable and shows up cleanly in the calendar:

```
### IG-2026-06-01 · Carousel · Draft · Marketplace-escape
Publish: 2026-06-08
Campaign: Phase 1 — First 10
```

**Fields:**

- **ID** — `IG-YYYY-MM-NN` / `LI-YYYY-MM-NN` / `TG-YYYY-MM-NN` / `X-YYYY-MM-NN` / `FB-YYYY-MM-NN`. Stable across edits.
- **Format** — Carousel · Single · Reel · Quote · Long-form · Text · Poll · Thread
- **Status** — Draft · In review · Approved · Scheduled · Published · Archived (or Planned for future-dated stubs)
- **Theme** — short tag. Either a campaign-specific theme (e.g. Marketplace-escape, Local-rails, Team-credibility) or, for the four-pillar batch, one of **Craft** (Apple — feature/product) · **Default** (Google — educational) · **Movement** (Shopify — updates) · **Listen** (feedback) — see `docs/strategy/operating-principles.md`.
- **Publish** — target publish date in ISO format
- **Campaign** — which phase brief or campaign this post supports

## Status workflow

`Draft` → `In review` (brand-review check) → `Approved` → `Scheduled` (in the publishing tool) → `Published` → `Archived` (moved to `_archive/` after the month closes)

## Voice and proof rules

All posts must clear `brand-voice/voice-guide.md`. No fabricated stats or testimonials. Numeric claims must be structural (e.g. "marketplaces take commission on every order") or marked `[PROOF — to collect]`.

## Languages

English source. Translate Uzbek (primary) + Russian (secondary) per `brand-voice/language-matrix.md` before publish. Native review required for regulatory terms (fiscalization, data residency, BNPL).

## When to start a new file

- A new calendar month has its own batch worth of posts → new `YYYY-MM.md`
- A campaign-batch grows past ~20 posts in one file → split by theme into `2026-06-marketplace-escape.md` etc.

## Index updates

When you add or change a post, update `social/calendar.md` so the cross-channel timeline stays current.
