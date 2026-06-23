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
### IG-2026-06-01 · Carousel · Draft · Multi-channel
Publish: 2026-06-08
Campaign: Phase 1 — First 10
```

**Fields:**

- **ID** — `IG-YYYY-MM-NN` / `LI-YYYY-MM-NN` / `TG-YYYY-MM-NN` / `X-YYYY-MM-NN` / `FB-YYYY-MM-NN`. Stable across edits.
- **Format** — Carousel · Single · Reel · Quote · Long-form · Text · Poll · Thread
- **Status** — Draft · In review · Approved · Scheduled · Published · Archived (or Planned for future-dated stubs)
- **Theme** — short tag. Either a merchant-outcome / campaign theme (e.g. Multi-channel, Earn-more, Retention, Customer-service, Tech-partner, Local-rails, Team-credibility) or, for the four-pillar batch, one of **Craft** (Apple — feature/product) · **Default** (Google — educational) · **Movement** (Shopify — updates) · **Listen** (feedback) — see `docs/strategy/operating-principles.md`. Keep the positive-sum, partner-focused stance from `brand-voice/voice-guide.md`.
- **Publish** — target publish date in ISO format
- **Campaign** — which phase brief or campaign this post supports

## Status workflow

`Draft` → `In review` (brand-review check) → `Approved` → `Scheduled` (in the publishing tool) → `Published` → `Archived` (moved to `_archive/` after the month closes)

## Voice and proof rules

All posts must clear `brand-voice/voice-guide.md`, including its positive-sum, partner-focused marketplace stance. No fabricated stats or testimonials. Numeric claims must be structural (e.g. "every order in Uzbekistan is reported to the OFD") or marked `[PROOF — to collect]`.

## Languages

Each post carries **three versions inline — EN (source) · RU · UZ** — under one shared visual direction. These are **transcreations, not translations**: each version is written to read natively in its own language, expressing the same meaning rather than mirroring the English word-for-word. Keep all three concise and clear-cut — no padded long-form.

Format inside a post: keep the `**Visual direction (shared):**` block once (the picture does not change across languages — only the text layer does), then stack `**🇬🇧 EN**` / `**🇷🇺 RU**` / `**🇺🇿 UZ**` blocks with the hook, slides/script, caption, and CTA in each. Add a `Localization:` line to the header (e.g. `Localization: EN source · RU + UZ transcreated · native review pending`).

Uzbek is written in Latin script. A native reviewer validates meaning and tone — especially regulatory terms (fiscalization, data residency, BNPL) — before status moves past In review. See `brand-voice/language-matrix.md`.

## When to start a new file

- A new calendar month has its own batch worth of posts → new `YYYY-MM.md`
- A campaign-batch grows past ~20 posts in one file → split by theme into `2026-06-multi-channel.md` etc.

## Index updates

When you add or change a post, update `social/calendar.md` so the cross-channel timeline stays current.
