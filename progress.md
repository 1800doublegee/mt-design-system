# Progress Note

**Project:** MT Design System / Claude Design Prompt Library
**Date:** 2026-04-19
**Session:** Claude Design prompt suite — Nick OS deck + video

---

## Completed
- [x] Nick OS deck prompt — 26 slides, personalised for Nick Marshall as Managing Partner
  - Templates: Cover (dark+image), Persona Board, Section Dividers ×5, Big Title, Today/Tomorrow ×2, Split Image+Copy, 6-Card Grid ×2, Process Circles, 2×2 Matrix, Brand Framework, Messaging Matrix, 4 Recommendations, Stats, 3-Column Grid, Body Text, Analysis (Today/Tomorrow reprise), Title+Body, Image Gallery, Positioning Statement, End
  - Personalised to Nick's four domains: Clients, New Business, Commercial, Creative Standards
  - Nick's archetype (Sage/Maverick), four conditions approach, uncomfortable truths register
  - Image backplates on dark slides (slides 01, 06, 11, 19) at 20-25% opacity
- [x] Nick OS video prompt — 90-second animated film, 8 scenes
  - No voiceover. Ambient score (Nils Frahm register). Hard cuts, not dissolves.
  - Text-forward, snap-in entrance, hold times explicitly instructed
  - Scene breakdown: Open → Condition → Problem → Clients → New Business → Commercial → Brief → Close
  - Closing quote: "The most dangerous condition for a managing partner isn't being wrong. It's being right — six weeks too late."
- [x] Clarified relationship between Leadership OS and Nick OS decks
  - Leadership OS = universal concept pitch (the why for any senior leader)
  - Nick OS = personalised execution (what it looks like configured for Nick)
  - They work as a pair; Nick OS can be made standalone with ~4 bridging slides

## In Progress
- [ ] Claude Design validation — user is actively testing decks in Claude Design
  - GCL-OS deck pasted first (from prior session)
  - Leadership OS deck ready
  - Nick OS deck + video ready to paste

## Prompt Library (all files in ~/Desktop/MT-Design-System/)
| File | Slides/Scenes | Status |
|------|--------------|--------|
| `GCL-OS-deck-prompt.md` | 20 slides | Complete — user testing |
| `Leadership-OS-deck-prompt.md` | 25 slides | Complete — ready to paste |
| `Nick-OS-deck-prompt.md` | 26 slides | Complete — ready to paste |
| `Nick-OS-video-prompt.md` | 8 scenes / 90s | Complete — ready to paste |

## Next Steps
1. User pastes Nick OS deck prompt into Claude Design — observe output
2. User pastes Nick OS video prompt — test animated video capability
3. Report back: which templates Claude Design handles well, which need prompt refinement
4. Optional: Add 4-5 bridging slides to Nick OS deck so it can stand alone without Leadership OS preamble
5. Consider: MT Templates Codification Figma work — still 45 slides awaiting design-validator pass

## Context for Cold Start
This folder (`~/Desktop/MT-Design-System/`) is a public GitHub repo (`1800doublegee/mt-design-system`) seeded with MT brand assets — tokens (CSS + JSON), typography, spacing, color system, slide templates CSS, L2 element kit components, brand guidelines, design language rules, slide pattern reference. It was built specifically to onboard Claude Design (Anthropic Labs, launched Apr 17 2026) as a capable MT design system interpreter. Claude Design parsed 30 design system items correctly on first read. The folder also stores Claude Design chat prompts for each deck.

## Key Files
- `README.md` — primary brand context document (MT identity, philosophy, typography, color, slide specs, 7 principles)
- `tokens/colors.css` — semantic color tokens, Light + Dark mode
- `tokens/typography.css` — font-face declarations + full text scale classes
- `tokens/spacing.css` — spacing scale + slide geometry variables
- `tokens/tokens.json` — Design Token Community Group format
- `components/slide-base.html` — 1920×1080 slide shell
- `components/slide-templates.css` — all 33 template patterns
- `brand/brand-guidelines.md` — studio identity, methodology, voice, visual do/don't
- `brand/design-language.md` — 33-template index + composition rules
- `brand/slide-patterns.md` — per-pattern selection guide + cheat sheet
- `GCL-OS-deck-prompt.md` — 20-slide deck prompt
- `Leadership-OS-deck-prompt.md` — 25-slide deck prompt
- `Nick-OS-deck-prompt.md` — 26-slide deck prompt
- `Nick-OS-video-prompt.md` — 90-second animated video prompt
