# Made Thought — Design Language

This document encodes the decisions behind how MT work looks — the micro-level craft that separates MT from generic design output.

---

## The modularity principle

MT presentations are **assembled, not designed**. Every slide is built from a fixed vocabulary of components. There are no one-off layouts. This constraint produces consistency, speed, and quality — the same reason Massimo Vignelli worked with a grid and the same typefaces for decades.

The components are:

**L1 Primitives** — The atoms: text nodes, backgrounds, footers.

**L2 Element Kit** — Reusable sub-slide elements:
- *Typographic expressions:* Stat Callout, Numbered Item, Quote Block, Kicker Headline, Pull Quote, Definition Pair
- *Diagram atoms:* Arrow (4 directions), Bracket (H/V), Connector Rule, Node Dot, Node Rect, Labelled Connector, Dot Chain
- *Data atoms:* KPI Block, Progress Bar, Comparison Row, Metric + Delta
- *Media slots:* Image 1:1, 4:3, 16:9, 3:4, 9:16, Full Bleed
- *Page furniture:* Pagination, Section Marker, Running Head, MT Logo Lockup, Bleed Bar, Divider Rule

**L3 Templates** — Complete slide layouts (33 types). Every slide maps to exactly one template.

**L4 Slide Library** — Finished, content-populated slides.

---

## The 33 template types

### Light templates (content slides)

| # | Template | Primary use |
|---|----------|-------------|
| 1 | Big Title | Opening chapter slide — large headline + 3-column body |
| 2 | Text Intro | Narrative slide — eyebrow + body + numbered list |
| 3 | 6-Card Grid | Evidence grid — 3×2 numbered cards |
| 4 | Stats | Numbers slide — headline + 3 large statistics |
| 5 | 2×2 Matrix | Framework — 4-quadrant model |
| 6 | 2×2 Matrix (empty) | Framework without body text — header + quadrant labels only |
| 7 | Today–Tomorrow | Comparison — 2-column contrast |
| 8 | 4 Recommendations | Action slide — 2×2 numbered recommendation cards |
| 9 | Competitor Grid | Competitive landscape — 2×3 image grid + labels |
| 10 | Analysis | Dual-column analysis — two themes with eyebrow + body |
| 11 | Messaging Matrix | Grid — multiple messages mapped across dimensions |
| 12 | Section Divider (light) | Chapter break in light mode |
| 13 | Numbered Section | Sequential content with step numbers |
| 14 | Process Circles | Horizontal flow diagram — circular step sequence |
| 15 | Brand Framework | Pillared framework — 4–5 principles in a row |
| 16 | Positioning Statement | Large centred quote with attribution |
| 17 | Title + Body | Prose slide — headline + long-form body |
| 18 | Body Text | Text-only — dense body copy, minimal header |
| 19 | 4-Column Grid | Data or concept — 4 equal columns |
| 20 | 3-Column Grid | Balanced content — 3 equal columns |

### Dark templates (structural slides)

| # | Template | Primary use |
|---|----------|-------------|
| 21 | Cover | First slide — logo + headline |
| 22 | Section Divider (dark) | Chapter break — Display/Mega single word or phrase |
| 23 | Brand Profile | Single brand deep-dive — name (display) + 2×2 attributes |
| 24 | Persona Map | Audience map — personas with dots on a spectrum |
| 25 | Split Image + Copy | Image left, copy right, dark background |
| 26 | Positioning Cards | Values or principles on dark cards |
| 27 | TOC | Table of contents — numbered list of sections |
| 28 | End Slide | Final slide — "MADE THOUGHT" logotype only |

### Mixed templates (light + dark panels)

| # | Template | Primary use |
|---|----------|-------------|
| 29 | Reference Board | Curated references — numbered items + image grid |
| 30 | Persona Board | Consumer profile — image grid + dark panel with persona details |
| 31 | Image Grid 4×2 | Visual-heavy — 4×2 image mosaic |
| 32 | Image Grid 2×2 | Visual-heavy — 2×2 image grid |
| 33 | Image Gallery | Full-width image with caption |

---

## Composition rules

### The reading path

MT slides are designed so the eye travels: **Page Title (top-left) → Display headline → Eyebrow labels → Body copy → Footer**.

Never interrupt this path with competing visual weight. If there's a stat, it's the hero. If there's a quote, it's the hero. One hero per slide.

### Column width formula

For N equal columns inside the 1800px content area with 24px gaps:
```
column width = (1800 - (24 × (N - 1))) / N

2 columns:  888px
3 columns:  584px
4 columns:  432px
```

### When to use dark vs. light

| Slide type | Theme |
|------------|-------|
| Cover | Dark |
| Section divider | Dark |
| End slide | Dark |
| Brand Profile | Dark |
| Persona Board (panel) | Mixed |
| Split Image (dramatic) | Dark right panel |
| All content slides | Light |

Rule of thumb: if the slide is **structural** (it punctuates, opens, or closes something), it's dark. If the slide **delivers content**, it's light.

### Stat slides

When presenting numbers, the number IS the design. The display type (Items MT Light, 180px or 68px) is the visual. There is no chart, no graph, no infographic. The number + a 1-line label is sufficient.

### Quote slides

Quotes use Display/M (46px) or Display/XL (68px) Items MT Light in italic. Attribution is 28px Futura PT Book uppercase with tracking. The quote is never in a speech bubble, box, or decorative container.

### Image slides

Images sit in slots — they do not break the grid. Image slots have defined aspect ratios: 1:1, 4:3, 16:9, 3:4, 9:16, Full Bleed. Full bleed images occupy the entire slide or one panel of a split layout.

---

## What makes a slide MT

Ask these questions before calling a slide finished:

1. **Is the hierarchy clear in 2 seconds?** Eye lands on the biggest thing first.
2. **Does every element earn its place?** Could anything be removed without losing meaning?
3. **Is the footer present?** Always.
4. **Are all fills token-bound?** No hardcoded hex values.
5. **Does the layout use the grid?** Columns are equal-width. Gaps are 24px.
6. **Is the typeface correct at this size?** Items MT ≥46px. Futura PT ≤28px.
7. **Is the slide using its template correctly?** Big Title doesn't have 4 columns. Stats don't have body paragraphs.

---

## Modularity in practice

If a brief requires a slide type that doesn't exist in the 33 templates, the correct response is:

1. First, check if an existing template can be adapted (change content, not structure).
2. If not, compose from two adjacent templates (e.g. Big Title header + 6-Card Grid body).
3. Only as a last resort, create a new pattern — and document it.

The system exists to prevent one-off decisions. One-off decisions look right in isolation and wrong in a deck.
