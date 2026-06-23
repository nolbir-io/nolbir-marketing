# Paid ads

Platform-specific paid ad creative and audience configuration for Own. Source-of-truth for what we run on Google Ads, Meta, and Yandex.

## Folder layout

```
paid-ads/
  README.md                          # this file — conventions
  YYYY-MM-<objective>.md             # one file per campaign batch (objective + month)
  _archive/                          # closed / superseded batches
```

## Naming convention

- One file per campaign objective per batch: `paid-ads/2026-06-brand-awareness.md`.
- File month = the month the batch *starts*.
- Each ad inside a file gets a stable ID: `<PLATFORM>-<OBJECTIVE>-NN`, e.g. `META-AWR-01`, `GADS-AWR-03`, `YDX-AWR-02`.

## What each batch file holds

1. **Campaign header** — objective, KPI, phase tie-in, languages, market.
2. **Audience configuration** — per platform: geo, demographics, interests, custom/lookalike, exclusions, recommended objective + bid strategy.
3. **Ad creative** — organized by angle, then by platform, with character counts validated against each platform's limits.
4. **Production + tracking notes** — UTM scheme, localization status, brand-review status.

## Character-count rule

Every headline / description / primary-text line carries its character count in parentheses, e.g. `(28)`. Anything over a platform limit is flagged and trimmed inline. English is the source language; **Cyrillic (Russian/Uzbek) counts differ and must be re-validated after localization** in each platform's preview tool before launch.

## Voice and proof rules

All creative must clear `brand-voice/voice-guide.md`, including its positive-sum, partner-focused marketplace stance. No fabricated stats or testimonials. Numeric claims must be structural facts (e.g. "every order in Uzbekistan is reported to the OFD") or marked `[PROOF — to collect]`.

## Languages

English source. Translate Uzbek (primary) + Russian (secondary) per `brand-voice/language-matrix.md` before publish. Yandex creative is drafted Russian-first because the network skews Russian-language in the CIS; Uzbek variants follow.

## Status workflow

`Draft` → `In review` (brand-review check) → `Approved` → `Live` → `Archived`.
