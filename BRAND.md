# proJeKt: humAnIty — Brand Specification v1.0
**JRK Enterprises | PROVISIONAL | June 6, 2026**
**Status:** PROVISIONAL — inherits MASTER wall authority
**CHANGELOG entry required for all changes**

---

## Purpose

This file is the canonical brand reference for proJeKt: humAnIty and all rooms under JRK Enterprises. Every document, README, page, and output that carries the project name should inherit from here — not invent its own visual grammar.

---

## Color Palette

Derived from the JRK Enterprises logo: deep forest green → warm gold gradient on near-black.

| Token | Hex | Use |
|-------|-----|-----|
| `--jrk-gold` | `#C9922A` | Primary headers, lettering, badges |
| `--jrk-green` | `#2D5A27` | Secondary accent, node lines |
| `--jrk-black` | `#0D0D0D` | Base background (dark contexts) |
| `--jrk-parchment` | `#E8D9B5` | Body text on dark, warm neutral |
| `--jrk-ember` | `#C94A2A` | 🔺🔺 VELA / Red channel — action, operations |
| `--jrk-sky` | `#2A5FC9` | 🔊🔊 ECHO / Blue channel — broadcast, signal |
| `--jrk-white-layer` | `#F0EDE6` | ◉ WHITE Architect — doctrine, governance |
| `--jrk-ochre` | `#C97A2A` | Eight-layer stack warm accent |

---

## Typography

### Font Stack

```
Headers:   Georgia, "Times New Roman", serif
Body:      system-ui, -apple-system, sans-serif
Code/tags: "Courier New", Courier, monospace
```

### Rationale
Georgia matches the hand-inked woodcut/parchment display lettering visible in the Triangle Architecture and Eight-Layer Stack illustrations. It gives the project a serious, documentary weight without being corporate. System-ui keeps body text clean and fast-loading everywhere.

---

## Channel Symbol Grammar

These symbols are the visual shorthand for the three operating channels. Use them consistently — they are not decorative, they are navigational.

| Channel | Symbol | Color | Function |
|---------|--------|-------|----------|
| VELA | 🔺🔺 | Ember `#C94A2A` | Red — operations, outreach, execution, pipelines |
| WHITE ARCHITECT | ◉ | White-layer `#F0EDE6` | Governance, doctrine, rules, guardrails |
| ECHO | 🔊🔊 | Sky `#2A5FC9` | Blue — broadcast, public signal, narrative |

**Note on the Architect symbol:** The intended glyph is an eye within a horizontally oval black Q — representing the watching, witnessing, non-commanding posture of the White governance layer. Until a custom SVG is finalized, `◉` is the canonical placeholder. It reads correctly in all GitHub contexts.

---

## Image Assets (Root-Level)

All images live at repository root. They are shared between the README and the GitHub Pages site (`index.html`). Do not move or rename without updating both.

| File | Use | Position in README |
|------|-----|--------------------|
| `hero.png` | Full-width title image — Joe + Librain porch scene | Top of README, before all text |
| `logo.jpg` | JRK Enterprises card logo | Below "What This Is" section |
| `triangle-architecture.png` | Triangle Architecture diagram | Below "The Triangle" / channel section |
| `eight-layer-stack.png` | Eight-Layer AI Infrastructure Economy | Below the layer table in "Eight-Layer" section |

**Raw URL pattern:**
```
https://raw.githubusercontent.com/thejkunkel-cmd/jrk-enterprises/main/[filename]
```

---

## Badge Grammar (shields.io)

Use these for version, status, and date signals at the top of README.

```markdown
![Version](https://img.shields.io/badge/version-0.1_PROVISIONAL-C9922A?style=flat-square&labelColor=0D0D0D)
![Status](https://img.shields.io/badge/status-PROVISIONAL-C94A2A?style=flat-square&labelColor=0D0D0D)
![Date](https://img.shields.io/badge/updated-June_6_2026-2D5A27?style=flat-square&labelColor=0D0D0D)
```

---

## Voice & Tone (Brand Adjacent)

- Serious without being cold
- Human-first — the framework exists because people matter, not despite them
- Warmth is not weakness; the porch image is intentional doctrine
- "No emergency required" is a brand statement, not a footnote
- Goes dark when needed. Friendly about having a big brain.

---

## Inheritance Rules

1. Every room README should open with the channel symbol for that room (🔺🔺 Red, 🔊🔊 Blue, ◉ White)
2. Color references in any document should use token names from this file, not raw hex
3. New images go to root unless there is a structural reason for a subfolder — log it in CHANGELOG
4. This file is PROVISIONAL until Joe explicitly locks it

---

*MASTER authority: Joe Kunkel / JRK Enterprises*
*All changes require a CHANGELOG entry.*
