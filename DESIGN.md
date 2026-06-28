---
name: Flags by Otis
description: A 6.5-year-old's hand-drawn flag shop bridging Addis Ababa and Sweden, one flag at a time.
colors:
  paper: "#fdf6e3"
  paper-deep: "#f5e6c8"
  page-bg: "#e8d5b0"
  card: "#fffdf6"
  ink: "#2c1a0e"
  ink-medium: "#4a2e0e"
  ink-muted: "#8a6840"
  ink-faint: "#b0905a"
  border: "#c8a87a"
  border-light: "#e0d0b8"
  accent-red: "#d94f3d"
  accent-red-deep: "#9b2e1f"
  accent-blue: "#3a6ea5"
  accent-green: "#4a8c5c"
  accent-yellow: "#e8b84b"
typography:
  display:
    fontFamily: "'Permanent Marker', cursive"
    fontSize: "clamp(2.4rem, 7vw, 4rem)"
    fontWeight: 400
    lineHeight: 1.1
  headline:
    fontFamily: "'Permanent Marker', cursive"
    fontSize: "1.9rem"
    fontWeight: 400
    lineHeight: 1.2
  title:
    fontFamily: "'Permanent Marker', cursive"
    fontSize: "1.5rem"
    fontWeight: 400
    lineHeight: 1.3
  body:
    fontFamily: "'Caveat', cursive"
    fontSize: "1.2rem"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "'Patrick Hand', cursive"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.5
rounded:
  sharp: "3px"
  slight: "4px"
  pill: "100px"
spacing:
  xs: "6px"
  sm: "14px"
  md: "20px"
  lg: "28px"
  xl: "36px"
  section: "32px"
components:
  button-primary:
    backgroundColor: "{colors.accent-red}"
    textColor: "{colors.card}"
    rounded: "{rounded.slight}"
    padding: "16px 32px"
    typography: "{typography.headline}"
  badge:
    backgroundColor: "{colors.accent-red}"
    textColor: "{colors.card}"
    rounded: "{rounded.pill}"
    padding: "5px 14px"
  flag-card:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.sharp}"
    padding: "13px 11px 11px"
  flag-card-selected:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.sharp}"
  paper-section:
    backgroundColor: "{colors.paper}"
    rounded: "{rounded.slight}"
    padding: "36px 28px"
  input:
    backgroundColor: "{colors.card}"
    textColor: "{colors.ink}"
    rounded: "{rounded.sharp}"
    padding: "10px 14px"
    typography: "{typography.body}"
---

# Design System: Flags by Otis

## 1. Overview

**Creative North Star: "The Letter from Addis"**

This design system is built around one physical sensation: opening an envelope from far away and finding something made by hand inside. Every surface is paper. Every shadow is an object resting on a desk. Every font is a pen Otis picked up. The page does not simulate a shop; it simulates correspondence.

The system is warm, earnest, and intentionally imprecise. Sections tilt slightly. Cards lift and tilt when you touch them. The fonts are handwritten. The color palette comes from the flags Otis draws, not from a brand identity document. This is not a designed product; it is a documented child's workshop. The primary audience is Swedish grandparents, aunts, and uncles who love Otis and want something made by his hands.

The system explicitly rejects: Etsy-adjacent handmade-goods aesthetic (beige rustic grids, marketplace distance); charity and NGO visual language (polished, cause-driven, donation-page tone); children's app and edtech design (bubbly primary colors, patronizing energy); generic e-commerce conversion design (cold product grids, add-to-cart patterns). If it looks like any of those, it has failed.

**Key Characteristics:**
- Every content block is a physical sheet of paper, sitting on a warm kraft-paper desk
- Hard-offset zero-blur shadows only: objects rest on surfaces, they do not float above them
- Three-voice typography system: Permanent Marker (proud), Caveat (conversational), Patrick Hand (careful)
- Four accent colors, each locked to one role: Red (action), Blue (value/focus), Green (price), Yellow (highlight)
- Imperfection is load-bearing: rotations, tilts, and the tape-strip motif signal a real human made this

## 2. Colors: The Four-Flag Palette

The palette is drawn from the flags themselves. Red and yellow from the Ethiopian and Swedish flags; blue from the Swedish sky; green from the Ethiopian hills. Nothing was chosen by a designer.

### Primary
- **Warm Writing Paper** (`#fdf6e3`, oklch 97% 0.022 85): The primary surface for all content sections. The page is a stack of papers.
- **Wax Seal Red** (`#d94f3d`, oklch 55% 0.178 25): Primary action color. Badge, submit button, and selection indicator. The red Otis reaches for when he means it. Never decorative.

### Secondary
- **Swedish Blue** (`#3a6ea5`, oklch 48% 0.118 254): Price highlights, focus indicators, interactive emphasis. The Sweden-Ethiopia bridge in one color. Used only for value and state.
- **Ethiopian Green** (`#4a8c5c`, oklch 54% 0.098 151): Price totals and currency display. Otis's home country, made visible.

### Tertiary
- **Afternoon Yellow** (`#e8b84b`, oklch 78% 0.132 82): Section title underlines and the tape-strip motif. The lightest accent; purely structural.

### Neutral
- **Kraft Canvas** (`#e8d5b0`, oklch 87% 0.04 80): The page background. A desk surface, not a digital canvas.
- **Aged Paper** (`#f5e6c8`, oklch 93% 0.03 82): Recessed surfaces: the note callout, the selected-flags display.
- **Indian Ink** (`#2c1a0e`, oklch 17% 0.038 55): Primary text on all surfaces. Warm near-black; never pure black.
- **Well-Worn Handle** (`#4a2e0e`, oklch 24% 0.055 54): Form labels and heading contexts. Darker than running text, not quite ink.
- **Dried Ink** (`#8a6840`, oklch 50% 0.068 65): Secondary text: SEK conversions, footnotes, footer. Receding information.
- **Cork Board** (`#b0905a`, oklch 64% 0.072 68): Empty-state and placeholder text. Present but barely.
- **Envelope Crease** (`#c8a87a`, oklch 73% 0.07 73): Form input borders and image frames. Where paper meets paper.
- **Stationery Edge** (`#e0d0b8`, oklch 85% 0.035 77): Flag image borders. The lightest structural line.
- **Pressed Red Shadow** (`#9b2e1f`, oklch 38% 0.135 25): Submit button shadow only. Never on text or backgrounds.

### Named Rules
**The Four-Flag Rule.** Red is action. Blue is value. Green is price. Yellow is highlight. Each accent appears in exactly one role. Never repurpose an accent for a different role; never use all four in the same visual region.

**The No-White Rule.** Pure `#fff` is forbidden. Card backgrounds, button text, and input backgrounds use `#fffdf6` (token: `card`), a barely-perceptible warm tint that keeps every surface inside the parchment family.

## 3. Typography

**Display Font:** Permanent Marker (Google Fonts)
**Body Font:** Caveat (Google Fonts)
**Label Font:** Patrick Hand (Google Fonts)

**Character:** A three-pen system. Permanent Marker is the deliberate display hand: Otis writing the title of his drawing, pressing hard. Caveat is the flowing body hand: Otis explaining something quickly, in a rush. Patrick Hand is the careful label hand: Otis writing the price in his neatest script. The three voices have a built-in social hierarchy and must not swap roles.

### Hierarchy
- **Display** (Permanent Marker, 400, `clamp(2.4rem, 7vw, 4rem)`, lh 1.1): Page title only. Once per page.
- **Headline** (Permanent Marker, 400, `1.9rem`, lh 1.2): Section titles, always with the yellow underline bar. The `::after` strip is inseparable from this role.
- **Title** (Permanent Marker, 400, `1.5rem`, lh 1.3): Prominent numeric values: exchange rate, price total. Colored in context: blue for rates, green for totals.
- **Body** (Caveat, 400/600, `1.2–1.35rem`, lh 1.55–1.6): All general content, form inputs, testimonial quotes. Weight 600 for flag names and emphasized content. Max line length 72ch.
- **Label** (Patrick Hand, 400, `1rem`, lh 1.5): SEK conversions, rate source notes, footer, helper text. Information that belongs in the margin.

### Named Rules
**The Three Voices Rule.** Permanent Marker is for things Otis is proud of. Caveat is for things Otis is telling you. Patrick Hand is for details you might need but that require no emphasis. Permanent Marker in body copy is forbidden. Patrick Hand in headings is forbidden.

**The Underline Rule.** Every Headline-role element receives a centered yellow bar: `80px × 4px`, `#e8b84b`, `border-radius: 2px`, 8px gap below the text. This is not optional decoration; it is the visual definition of a section heading in this system.

## 4. Elevation

This system uses structural hard-offset shadows with zero blur. The metaphor is papers stacked on a desk. A blurred shadow implies a floating object; a hard-offset shadow implies a resting one. Every shadow in this system has `blur-radius: 0`.

### Shadow Vocabulary
- **Paper Stack** (`3px 3px 0 rgba(44,26,14,0.12), 6px 6px 0 rgba(44,26,14,0.06)`): Two-layer shadow for all main content sections. The doubled offset suggests the thickness of a folded letter.
- **Card Rest** (`2px 2px 0 rgba(44,26,14,0.15)`): Flag cards and testimonial cards at rest. Smaller footprint for lightweight objects.
- **Card Hover** (`4px 6px 0 rgba(44,26,14,0.15)`): Flag card on interaction, paired with `transform: rotate(1deg) translateY(-3px)`. The card lifts and its shadow stretches.
- **Stamp Ink** (`4px 4px 0 #9b2e1f`): Submit button only. The shadow uses the pressed-red token, not neutral ink; the button reads as a wax seal pressing into paper.
- **Stamp Pressed** (`2px 2px 0 #9b2e1f`): Submit button active state. The stamp pushes down; the shadow contracts.

### Named Rules
**The Zero-Blur Rule.** Every `box-shadow` in this system has `blur-radius: 0`. A blurred shadow is prohibited. Achieve additional depth with tonal surface layers, not gaussian blur.

**The Ink Shadow Rule.** Only the submit button uses a colored shadow (`#9b2e1f`). All other shadows use `rgba(44,26,14,...)`. Never apply a colored shadow to a card, section, or input.

## 5. Components

### Buttons
The submit button reads as a rubber stamp pressing into paper. It is the only button in the system; no ghost or secondary variants exist.

- **Shape:** Gently rounded (4px, `{rounded.slight}`)
- **Primary:** Wax Seal Red (`#d94f3d`) background, warm-white (`#fffdf6`) text, Permanent Marker 1.4rem, padding 16px 32px
- **Hover:** `translateY(-2px)`, shadow extends to Stamp Ink hover. Transition: `0.1s ease`.
- **Active:** `translateY(2px)`, shadow contracts to Stamp Pressed. The stamp pushes in.
- **Focus visible:** `outline: 3px solid #3a6ea5`, offset 3px.
- Secondary actions use plain text links in Caveat, never a ghost button variant.

### Flag Cards (Selector)
A small postage stamp you pick up, examine, and set aside or keep.

- **Shape:** Square-edged (3px, `{rounded.sharp}`)
- **Background:** `#fffdf6` at rest and selected (the card surface does not change color on selection)
- **Rest:** Card Rest shadow
- **Hover:** `transform: rotate(1deg) translateY(-3px)`, Card Hover shadow. Tilts right and lifts.
- **Selected:** `outline: 3px solid #d94f3d`, `transform: rotate(-1deg) scale(1.03)`. Tilts the opposite direction; a checkmark appears top-right. `aria-pressed="true"` required.
- **Image:** 72px tall, `object-fit: cover`, 1px `#e0d0b8` border, `border-radius: 2px`.
- **Transition:** `0.15s ease` on transform and box-shadow only.
- **Accessibility:** Must be `<button>` or carry `role="button"` + `tabindex="0"` + keyboard handler. `aria-pressed` must reflect selection state.

### Paper Sections
Every major content block is a sheet of paper.

- **Background:** Warm Writing Paper (`#fdf6e3`)
- **Shadow:** Paper Stack (two layers)
- **Radius:** 4px (`{rounded.slight}`)
- **Tape Variant:** `::before` pseudo-element, 70px × 26px, `rgba(255,220,100,0.55)`, `border-radius: 2px`, positioned `top: -14px` centered, rotated ±2deg. Indicates something pinned or posted.
- **Padding:** 36px 28px for gallery/testimonial sections; 36px 32px 40px for the order form.

### Inputs and Form Fields
Lined paper waiting to be filled in.

- **Background:** `#fffdf6`
- **Border:** `2px solid #c8a87a` at rest
- **Radius:** 3px (`{rounded.sharp}`)
- **Font:** Caveat 1.2rem, `#2c1a0e`
- **Focus:** Border shifts to `#3a6ea5`, plus `outline: 2px solid #3a6ea5; outline-offset: 2px`. Both the border color shift and the outline are required: the border shift carries the visual character; the outline meets WCAG 2.4.11.
- **Textarea:** Same treatment, `resize: vertical`, `min-height: 90px`.
- **Labels:** Caveat 600, 1.15rem, `#4a2e0e`.

### Testimonial Cards (Sticky Notes)
Pinned notes from happy customers, not a review widget.

- **Background:** One of six warm pastel backgrounds by position: yellow (`#fef9c3`), green (`#dcfce7`), blue (`#dbeafe`), pink (`#fce7f3`), orange (`#ffedd5`), soft green (`#f0fdf4`).
- **Rotation:** Each card is rotated by a fixed amount (±0.7–1.5deg), never the same direction twice in a row.
- **Pin Dot:** `::before` pseudo-element, 10px × 10px circle, `rgba(0,0,0,0.15)`, top center.
- **Quote:** Caveat 1.15rem, `#2c1a0e`.
- **Author:** Permanent Marker 0.95rem, `#5c3d1e`.
- **Not interactive.** No hover state. These are pinned, not clickable.

### Badge
Otis's own label pinned to the header.

- **Shape:** Pill (100px, `{rounded.pill}`)
- **Background:** Wax Seal Red (`#d94f3d`)
- **Text:** Permanent Marker 13px, `#fffdf6`
- **Rotation:** Always tilted -2deg. Non-negotiable.

### Section Title
Every section heading is two inseparable parts: the text and the yellow bar beneath it.

- **Font:** Permanent Marker 1.9rem, `#2c1a0e`, center-aligned
- **Underline:** `::after` block, 80px × 4px, `#e8b84b`, `border-radius: 2px`, 8px gap above

## 6. Do's and Don'ts

### Do:
- **Do** use `#fffdf6` (token: `card`) for every card and input background. Pure `#fff` is prohibited.
- **Do** apply hard-offset zero-blur shadows to all elevated surfaces. Every `box-shadow` has `blur-radius: 0`.
- **Do** tilt cards, sections, and the badge slightly. Imperfection is the brand signal; straight-edged layouts break the metaphor.
- **Do** use Permanent Marker for anything Otis is proud of: titles, section headings, prices, the CTA.
- **Do** use Patrick Hand only for receding secondary information: SEK conversions, rate notes, footer copy.
- **Do** enforce the Four-Flag Rule: Red for action, Blue for value/focus, Green for price, Yellow for highlight.
- **Do** ensure every interactive element is at least 44px in touch target size. The primary audience includes older users on phones.
- **Do** attach the yellow underline bar to every Headline-role element. It is not optional.
- **Do** set `aria-pressed` on flag cards and announce selection changes via `aria-live="polite"`.
- **Do** pair the border-color focus shift with an explicit `outline`. Both are required for WCAG 2.4.11.

### Don't:
- **Don't** use `#fff` or `#000` anywhere. Every surface and text must be tinted toward the warm brand hue.
- **Don't** add blur to any shadow. `blur-radius: 0` is absolute. A single blurred shadow breaks the paper metaphor for the entire page.
- **Don't** use `border-left` greater than 1px as a colored stripe on callouts, cards, or alerts. Rewrite with a background tint, full border, or a leading icon.
- **Don't** animate layout properties (width, height, padding, margin). Animate only `transform` and `opacity`.
- **Don't** design like Etsy: no beige rustic grids, no marketplace distance between buyer and maker.
- **Don't** design like a charity or NGO: no polished cause-driven layouts, no donation-page tone.
- **Don't** design like a children's app: no bubbly rounded fonts beyond the existing trio, no patronizing primary-color saturation.
- **Don't** design like generic e-commerce: no cold product grids, no conversion-optimization patterns.
- **Don't** repurpose an accent color. Swedish Blue is not a decorative highlight. Ethiopian Green is not for emphasis text. Afternoon Yellow is not a background.
- **Don't** use `#9b2e1f` (Pressed Red Shadow) anywhere except as the submit button's shadow.
- **Don't** use Permanent Marker for body copy or Patrick Hand for headings. The Three Voices Rule is inviolable.
- **Don't** use gradient text (`background-clip: text` with a gradient). Prohibited in this system.
- **Don't** make anything feel transactional. Placing an order leads to a phone call from a 6-year-old; the form is ceremonial, not a checkout.
