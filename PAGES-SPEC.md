# proJeKt: humAnIty — GitHub Pages Design Spec
**Version:** 0.1 PROVISIONAL
**Date:** June 6, 2026
**Status:** DRAFT — not yet implemented
**Inherits:** BRAND.md, MASTER wall, Safety Spine v1.0

---

## Purpose

This file is the architectural spec for the public-facing GitHub Pages site hosted at `index.html` (root). It exists so that every future edit to the site has a reference point — not just a file to poke at. Anyone who opens this file should be able to understand the full design intent, update the site consistently, and not break what came before.

The README is the repo front door. The Pages site is the *human* front door — built for evaluators, partners, and first-time readers who aren't GitHub-native.

---

## Site URL

```
https://thejkunkel-cmd.github.io/jrk-enterprises/
```

Served from: `index.html` at repository root.
Source branch: `main`

---

## Brand Foundation (inherits BRAND.md)

### Color Tokens

```css
:root {
  --jrk-gold:         #C9922A;  /* Primary headers, lettering */
  --jrk-green:        #2D5A27;  /* Secondary accent, node lines */
  --jrk-black:        #0D0D0D;  /* Base background */
  --jrk-parchment:    #E8D9B5;  /* Body text, warm neutral */
  --jrk-ember:        #C94A2A;  /* 🔺🔺 VELA / Red channel */
  --jrk-sky:          #2A5FC9;  /* 🔊🔊 ECHO / Blue channel */
  --jrk-white-layer:  #F0EDE6;  /* ◉ WHITE Architect / doctrine */
  --jrk-ochre:        #C97A2A;  /* Eight-layer warm accent */
  --jrk-surface:      #161616;  /* Card/section surface on black */
  --jrk-border:       #2A2A2A;  /* Subtle separator lines */
}
```

### Font Stack

```css
/* Headers — matches woodcut/parchment illustration lettering */
font-family: Georgia, "Times New Roman", serif;

/* Body — clean, fast, system-native */
font-family: system-ui, -apple-system, BlinkMacSystemFont, sans-serif;

/* Code, labels, tags */
font-family: "Courier New", Courier, monospace;
```

### Channel Symbol Usage

| Symbol | Channel | Where It Appears |
|--------|---------|------------------|
| 🔺🔺 | VELA / Red | Outreach, evaluation, operations sections |
| ◉ | WHITE Architect | Governance, doctrine, start-here sections |
| 🔊🔊 | ECHO / Blue | Attribution, signal, public-facing copy |

---

## Page Structure & Section Map

The site is a single-page document. Sections flow top to bottom. Each section has a named anchor for deep-linking.

```
#hero          — Full-width opening image + title + tagline
#what-this-is  — Core question, project identity, JRK logo
#start-here    — Navigation block for first-time readers
#triangle      — Three-channel architecture + diagram
#eight-layers  — Layer table + eight-layer stack image
#evaluation    — Microsoft vs. Perplexity link block
#attribution   — IP / provenance / unnamed credit system
#contact       — Evaluator access + contact
```

---

## Section-by-Section Spec

### `#hero`
- **Image:** `hero.png` — full viewport width, max-height 600px, object-fit cover
- **Overlay:** Dark gradient bottom 30%, opacity 0.6, so title text is readable
- **Title:** `proJeKt: humAnIty` — Georgia serif, `--jrk-gold`, large display size (clamp 2.5rem–5rem)
- **Tagline:** `Does this AI system honor or extract from the human institutions it enters?` — parchment color, 1.2rem
- **Subline:** `JRK Enterprises · Putnam, Connecticut · PROVISIONAL 2026` — smaller, muted

### `#what-this-is`
- **Symbol:** ◉ inline before section heading
- **Logo:** `logo.jpg` centered, max-width 280px, with subtle gold border-radius card
- **Body:** Georgia serif for first paragraph (doctrine-weight), system-ui for rest
- **Background:** `--jrk-surface`

### `#start-here`
- **Symbol:** ◉
- **Style:** Numbered list, each item a gold-accented link card
- **Card style:** `--jrk-surface` bg, `--jrk-gold` left border 3px, padding 1rem, hover lifts with subtle gold glow
- **Links:** Floor Doctrine → Eight-Layer Framework → Microsoft vs. Perplexity

### `#triangle`
- **Symbol:** 🔺🔺 🔊🔊 ◉ all three inline in heading
- **Channel table:** Three columns, each column header colored with its channel color (ember / white / sky)
- **Image:** `triangle-architecture.png` — full section width, max 900px centered
- **Background:** `--jrk-black`

### `#eight-layers`
- **Symbol:** ◉
- **Layer table:** Styled with alternating row tones. Layer 8 (top) has `--jrk-gold` left accent. Layer 1 (bottom) has `--jrk-green` left accent. Layers graduate between.
- **Image:** `eight-layer-stack.png` — full section width, max 900px centered, below table
- **Background:** `--jrk-surface`
- **Caption:** *"The stronger the foundation, the greater the impact."* — italic, parchment, centered

### `#evaluation`
- **Symbol:** 🔺🔺
- **Style:** Bold callout block — `--jrk-ember` left border, dark surface card
- **Content:** Link to `02_evaluation/` with one-sentence description
- **Subtext:** Methodology note — publicly sourced, credited evidence

### `#attribution`
- **Symbol:** 🔊🔊
- **Style:** Clean, dignified — this is the trust section
- **Content:** Unnamed Credit System explanation, link to `PROVENANCE.md`
- **Tone:** No defensiveness. Open hand.

### `#contact`
- **Symbol:** 🔺🔺
- **Content:** Target review date, contact handle (tavar1x)
- **CTA:** One clear line — evaluator packet available on request
- **Background:** `--jrk-black`, gold rule above

---

## Typography Scale

```css
--text-hero:    clamp(2.5rem, 6vw, 5rem);    /* Hero title */
--text-h1:      clamp(1.8rem, 4vw, 3rem);    /* Section headers */
--text-h2:      clamp(1.3rem, 2.5vw, 2rem);  /* Sub-headers */
--text-body:    1.1rem;                       /* Body copy */
--text-small:   0.875rem;                     /* Labels, captions */
--line-height:  1.7;                          /* Body line spacing */
```

---

## Responsive Breakpoints

```css
/* Mobile first */
@media (min-width: 640px)  { /* tablet adjustments */ }
@media (min-width: 1024px) { /* desktop — max content width 1100px centered */ }
```

All images scale fluidly. Tables collapse to card-stack layout on mobile.

---

## Implementation Notes

### What exists now
`index.html` is already live at root and served via GitHub Pages. All four images (`hero.png`, `logo.jpg`, `triangle-architecture.png`, `eight-layer-stack.png`) are at root and referenced correctly.

### What this spec is for
This spec describes the *intended* design state — the full brand-coherent version. The current `index.html` may not yet implement all of the above. This file is the target, not a description of current reality.

### Implementation order (next session)
1. Audit current `index.html` against this spec — note gaps
2. Apply color tokens as CSS variables to `:root`
3. Apply font stack to headers and body
4. Style the `#start-here` card links with gold left-border treatment
5. Style the layer table with graduated row accents
6. Add `#triangle` channel table with column-level color
7. Add hero overlay gradient for text legibility
8. Test responsive layout on mobile

### Do not change
- Image filenames or paths — they are shared with README
- Section anchor IDs — they are used for deep-linking
- The `index.html` filename — it is the Pages entry point

---

## CHANGELOG Entry Required

Any change to `index.html` that materially alters layout, color, or section order must be logged in `CHANGELOG.md` with:
- Date
- What changed
- Why
- Status (PROVISIONAL / VALIDATED / FINAL)

---

*MASTER authority: Joe Kunkel / JRK Enterprises*
*This file is PROVISIONAL. Nothing here is final until explicitly locked.*
*All changes require a CHANGELOG entry.*
