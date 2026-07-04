---
name: Innova AI Demos
description: Calm, light proof-of-concept site - working tools, not slides. Manrope + JetBrains Mono, one cyan accent used sparingly.
colors:
  ground: "#eef2f6"
  ground-2: "#e4eaef"
  surface: "#ffffff"
  surface-2: "#f5f8fa"
  ink: "#182731"
  ink-soft: "#3d4d57"
  ink-mut: "#5f6f78"
  ink-faint: "#6b7780"
  cyan: "#0a7c88"
  cyan-bright: "#12b3c6"
  cyan-soft: "#e7f6f8"
  amber: "#bd7420"
  amber-bright: "#e8893c"
  green: "#1f9564"
  red: "#c34438"
  line: "#e4e9ee"
  line-strong: "#d5dce2"
typography:
  hero:
    fontFamily: "Manrope, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "clamp(28px, 4.4vw, 43px)"
    fontWeight: 700
    lineHeight: 1.12
    letterSpacing: "-0.025em"
  display:
    fontFamily: "{typography.hero.fontFamily}"
    fontSize: "clamp(24px, 3.5vw, 33px)"
    fontWeight: 660
    lineHeight: 1.18
    letterSpacing: "-0.018em"
  body:
    fontFamily: "{typography.hero.fontFamily}"
    fontSize: "15.5px"
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: "normal"
  label:
    fontFamily: "JetBrains Mono, ui-monospace, SFMono-Regular, Menlo, Consolas, monospace"
    fontSize: "12px"
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: "0.14em"
rounded:
  sm: "6px"
  md: "11px"
  lg: "14px"
  xl: "16px"
  device: "20px"
  pill: "999px"
spacing:
  xs: "9px"
  sm: "14px"
  md: "18px"
  lg: "24px"
components:
  button-primary:
    backgroundColor: "{colors.cyan}"
    textColor: "#f2feff"
    rounded: "{rounded.md}"
    padding: "0 18px"
  chip:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.cyan}"
    rounded: "{rounded.pill}"
    padding: "6px 12px"
  input:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.md}"
    padding: "12px 14px"
  card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.xl}"
    padding: "18px"
  tool-card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "18px"
    padding: "24px"
---

# Design System: Innova AI Demos

## 1. Overview

**Creative North Star: "Working Tools, Not Slides"**

This is a calm, light workshop, not a pitch deck. A soft off-white ground holds clean
white surfaces with hairline borders and barely-there shadows; one cool cyan accent does
all the pointing, used sparingly. The whole system is built to make working software feel
credible and quiet - a technician's copilot and a documentation dashboard that read as
real tools someone would open, framed by just enough copy to explain why they exist.

The system rejects the tells of AI-demo marketing and thrown-together prototypes: no dark
hero with purple gradients, no sparkle chrome, no "Powered by AI" badges, no 01/02/03
editorial scaffolding, no low-contrast gray-on-gray. Depth comes from tonal layering
(ground to surface) and precise spacing, not from effects. The one place personality
concentrates is the type: a humanist sans for everything human, a monospace for everything
the machine asserts.

Two demos and the landing frame all get equal craft. The demos must feel usable, not
illustrative; the frame must feel like a confident product site, not a portfolio page.

**Key Characteristics:**
- Light off-white ground, white surfaces, hairline borders, whisper shadows.
- One cyan accent (used sparingly) plus a strict amber/green/red status system.
- Human/machine type duality: Manrope for prose, JetBrains Mono for the machine.
- Calm and restrained - premium through precision, not decoration.
- Honest labeling of real vs illustrative vs production baked into the visuals.

## 2. Colors

A quiet off-white and white base, one cyan voice, and a disciplined status trio.

### Primary
- **Signal Cyan** (#0a7c88): The single accent, used sparingly for links, eyebrows, the
  emphasized clause in headlines, accent rules, buttons, and interactive/focus states.
  Tuned to pass WCAG AA (4.9:1) as text on white. **Bright Cyan** (#12b3c6) is a
  non-text sibling reserved for fills, dots, and the brand mark; **Cyan Soft** (#e7f6f8)
  is a tint background for chips and code.

### Secondary / Status (functional, not decorative)
- **Amber** (#bd7420) / bright (#e8893c): "review / caution" status and the brand-mark arc.
- **Green** (#1f9564): "current / safe / online".
- **Red** (#c34438): "stale / stop". The rarest color; its scarcity is the alarm.

### Neutral
- **Ground** (#eef2f6) / **Ground-2** (#e4eaef): The page and its recessed zones.
- **Surface** (#ffffff) / **Surface-2** (#f5f8fa): Cards, devices, and inner surfaces.
- **Ink** (#182731), **Ink-soft** (#3d4d57), **Ink-mut** (#5f6f78), **Ink-faint**
  (#6b7780): Text from primary headings down to labels. Ink-faint is tuned to 4.6:1 on
  white so even labels pass AA.
- **Line** (#e4e9ee) / **Line-strong** (#d5dce2): Hairline dividers and stronger strokes.

### Named Rules
**The One Voice Rule.** Cyan is the only brand accent, and it stays rare - links,
eyebrows, one headline clause, buttons, accent rules. Amber/green/red are functional
status only, never emphasis or decoration.

**The AA Floor Rule.** Any text color must clear 4.5:1 on its actual surface. Never
reintroduce the old brighter cyan (#0d97a8) or faint label gray (#87949d) for text - both
fail AA on white.

## 3. Typography

**Display / Body Font:** Manrope (with system-sans fallback)
**Label / Mono Font:** JetBrains Mono (with ui-monospace fallback)

**Character:** Manrope is a clean humanist sans with tight, confident headlines;
JetBrains Mono is the "machine" voice reserved for anything that should read as precise
truth - codes, statuses, citations, data, timestamps. The duality is the system's
signature.

### Hierarchy
- **Hero** (Manrope 700, clamp(28px, 4.4vw, 43px), line-height 1.12, ls -0.025em): The
  landing headline only, with one cyan `<em>` clause.
- **Display / Lede** (Manrope 660, clamp(24px, 3.5vw, 33px), ls -0.018em): Per-page lede
  headlines; ~62ch max, cyan emphasis clause.
- **Body** (Manrope 400, 15.5px, line-height 1.55): Lede and card prose; kept ~58-60ch.
- **Eyebrow / Label** (JetBrains Mono 600, 12px, uppercase, ls 0.14em, cyan): Section
  labels. Keep them short - long uppercase runs hurt readability.
- **Micro-label** (JetBrains Mono, 9.5-11px): Dense in-component labels inside the
  device, KPI keys, table headers, tags. Deliberately small; appropriate for tool chrome.

### Named Rules
**The Instrument-Voice Rule.** Machine-truth (codes, statuses, citations, data) is set in
JetBrains Mono; human sentences in Manrope. The split is how the UI signals what is
grounded.

**The Short-Eyebrow Rule.** Eyebrows stay under ~30 characters. If a label needs a
sentence, it is not an eyebrow.

## 4. Elevation

A light, mostly-flat system. Depth is built from tonal layering (ground -> surface) and
hairline borders; shadows are a whisper, used to lift the interactive demo surfaces (the
Field Assist device, the DocSync impact panel, hover states) a hair off the page. Nothing
casts a heavy drop.

### Shadow Vocabulary
- **shadow-sm** (`0 1px 2px rgba(20,40,50,.05)`): Resting cards and tiles.
- **shadow** (`0 1px 2px rgba(20,40,50,.04), 0 14px 34px -20px rgba(20,40,50,.22)`):
  Devices, bot bubbles, active panels.
- **shadow-lift** (`0 2px 4px rgba(20,40,50,.05), 0 22px 48px -26px rgba(20,40,50,.28)`):
  The chat device and tool-card hover - the most any element lifts.

### Named Rules
**The Whisper Rule.** Shadows stay soft and low-contrast; if a shadow reads as a hard
drop, it is wrong for this light system. Prefer a border plus a faint lift over a strong
shadow.

## 5. Components

### Buttons
- **Shape:** 11px radius (`rounded.md`).
- **Primary (Ask / send):** Signal Cyan fill, near-white text (#f2feff), weight 600.
- **Hover / Focus:** Background deepens (#0a6f7a) over 0.15s; global `:focus-visible`
  gives a 2px cyan ring, offset 2px.

### Chips (suggestion)
- **Style:** White fill, Line-strong border, cyan mono text, fully rounded (999px).
- **Hover:** Border becomes cyan, fill shifts to Cyan Soft (#e7f6f8).

### Cards / Containers
- **Corner Style:** 16px cards (`rounded.xl`), 14px feature/step tiles, 18px tool cards,
  20px device.
- **Background:** Solid white surface on the off-white ground.
- **Shadow Strategy:** shadow-sm at rest; see Elevation. Tool cards lift to shadow-lift on
  hover and gain a cyan border + `translateY(-3px)`.
- **Border:** 1px Line.
- **Internal Padding:** 16-24px.

### Inputs / Fields
- **Style:** White fill, 1px Line-strong stroke, 11px radius, Ink-faint placeholder.
- **Focus:** Border shifts to cyan with a 3px `rgba(18,179,198,.14)` glow.

### Status Pills
- Mono uppercase, tinted background per state: safe/current (green), caution/review
  (amber), stop/stale (red), missing (neutral). Dot + label. Used in Field Assist
  severity and DocSync coverage.

### Section Markers
- Feature/step cards lead with a short cyan **accent rule** (22x2px bar), never numbered
  01/02/03 labels. The bar gives rhythm without the AI-editorial scaffold.

### Signature Components
- **Field Assist device:** a white "device" (top bar with status dots + pulsing online
  dot, scrolling thread, composer with suggestion chips). Bot answers are structured:
  title + mono code chip, numbered steps, a severity pill, and a collapsible cited source
  quoting the manual. Preserve **answer -> steps -> severity -> citation**.
- **DocSync dashboard:** KPI row, spec-change rail, impact panel with a red/green diff
  patch, an affected-docs list with per-language tags, and a product x language coverage
  matrix of status dots. Preserve the **change -> blast radius -> drafted fix** flow.

## 6. Do's and Don'ts

### Do:
- **Do** keep it light, calm, and restrained; premium comes from precision and negative
  space, not effects.
- **Do** hold cyan as the only brand accent and keep it rare (The One Voice Rule); reserve
  amber/green/red for status.
- **Do** set machine-truth (codes, statuses, citations, data) in JetBrains Mono and human
  prose in Manrope (The Instrument-Voice Rule).
- **Do** keep every text color above 4.5:1 on its actual surface (The AA Floor Rule).
- **Do** lead feature/step cards with the short cyan accent rule, not numbers.
- **Do** label real vs illustrative vs production honestly, in the UI.

### Don't:
- **Don't** ship AI-demo slop: no purple gradients, sparkle emojis, "Powered by AI"
  badges, or fake-futuristic chrome.
- **Don't** reintroduce 01/02/03 numbered section markers or tracked-eyebrow clichés.
- **Don't** use the old brighter cyan (#0d97a8) or faint gray (#87949d) as text - both
  fail AA on white.
- **Don't** use long uppercase eyebrows (keep under ~30 chars) or hype-deck superlatives.
- **Don't** let any element cast a hard drop shadow (The Whisper Rule).
