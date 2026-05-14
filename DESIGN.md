---
name: Pangolin Design System
version: 0.1.0
status: independent-design-study
description: Ubuntu-inspired, Carbon-style static design system for Linux-flavored product interfaces.
license: MIT
fonts:
  sans:
    family: Ubuntu Sans
    source: Google Fonts
    fallback: "-apple-system, BlinkMacSystemFont, Segoe UI, system-ui, sans-serif"
  mono:
    family: Ubuntu Sans Mono
    source: Google Fonts
    fallback: "ui-monospace, JetBrains Mono, SF Mono, Menlo, Consolas, monospace"
colors:
  aubergine:
    "10": "#F5EAF1"
    "20": "#E0BFD6"
    "30": "#B98AAA"
    "40": "#8E5279"
    "50": "#77216F"
    "60": "#5A0F4D"
    "70": "#44032E"
    "80": "#2C001E"
    "90": "#1A0011"
    "100": "#0D0008"
  orange:
    "10": "#FFEFE6"
    "20": "#FFD4BD"
    "30": "#FFAE85"
    "40": "#FF7848"
    "50": "#E95420"
    "60": "#C8420A"
    "70": "#A8370A"
    "80": "#7E2807"
    "90": "#511904"
  warm:
    "10": "#FAF7F4"
    "20": "#F2EEE9"
    "30": "#E8E2DA"
    "40": "#DCD4CA"
    "50": "#BFB5A8"
    "60": "#8E867E"
    "70": "#6B6259"
    "80": "#4A433C"
    "90": "#2C2722"
    "100": "#1B1612"
  status:
    error: "#C8240F"
    errorText: "#A41C0B"
    errorBg: "#FBE5E0"
    warning: "#E68B00"
    warningText: "#B86D00"
    warningBg: "#FCEFD3"
    success: "#1D7A4B"
    successText: "#155A37"
    successBg: "#E0F0E5"
    info: "#2563CB"
    infoText: "#1B4FA8"
    infoBg: "#E5EEFB"
  accents:
    magenta: "#A21F6F"
    teal: "#117C7C"
    sage: "#5E8C61"
    prussian: "#1B3A4B"
semanticColors:
  paper:
    background: "{colors.warm.10}"
    layer1: "#FFFFFF"
    layer2: "{colors.warm.10}"
    textPrimary: "{colors.warm.100}"
    textSecondary: "{colors.warm.70}"
    borderSubtle: "{colors.warm.30}"
    borderStrong: "{colors.warm.60}"
    focus: "{colors.orange.50}"
    primaryAction: "{colors.aubergine.80}"
    accentAction: "{colors.orange.50}"
  terminal:
    background: "{colors.aubergine.90}"
    layer1: "{colors.aubergine.80}"
    layer2: "{colors.aubergine.70}"
    textPrimary: "{colors.warm.10}"
    textSecondary: "{colors.warm.40}"
    borderSubtle: "{colors.aubergine.60}"
    focus: "{colors.orange.40}"
    primaryAction: "{colors.orange.50}"
spacing:
  "0": 0
  "01": 2px
  "02": 4px
  "03": 8px
  "04": 12px
  "05": 16px
  "06": 24px
  "07": 32px
  "08": 40px
  "09": 48px
  "10": 64px
  "11": 80px
  "12": 96px
  "13": 160px
radii:
  none: 0
  xs: 3px
  sm: 6px
  md: 8px
  lg: 12px
  xl: 16px
  pill: 999px
typography:
  scale:
    label:
      fontSize: 12px
      lineHeight: 1.5
      fontWeight: 500
    body:
      fontSize: 14px
      lineHeight: 1.5
      fontWeight: 400
    bodyMd:
      fontSize: 16px
      lineHeight: 1.5
      fontWeight: 400
    lede:
      fontSize: 20px
      lineHeight: 1.4
      fontWeight: 400
    heading3:
      fontSize: 32px
      lineHeight: 1.2
      fontWeight: 500
    heading1:
      fontSize: 42px
      lineHeight: 1.1
      fontWeight: 300
    display:
      fontSize: 76px
      lineHeight: 1
      fontWeight: 200
shadows:
  "01": "0 1px 2px rgba(44, 0, 30, 0.06), 0 1px 1px rgba(44, 0, 30, 0.04)"
  "02": "0 2px 6px rgba(44, 0, 30, 0.08), 0 1px 2px rgba(44, 0, 30, 0.06)"
  "03": "0 8px 24px rgba(44, 0, 30, 0.10), 0 2px 6px rgba(44, 0, 30, 0.06)"
  "04": "0 20px 60px rgba(44, 0, 30, 0.16), 0 4px 12px rgba(44, 0, 30, 0.08)"
motion:
  fast: 70ms
  default: 110ms
  moderate: 150ms
  popover: 240ms
  slow: 400ms
  skeleton: 700ms
components:
  button:
    radius: "{radii.sm}"
    heightDefault: 32px
    heightSmall: 24px
    heightLarge: 40px
    variants: [primary, secondary, tertiary, ghost, danger, accent]
  card:
    radius: "{radii.md}"
    border: "1px solid {semanticColors.paper.borderSubtle}"
    padding: "{spacing.06}"
  table:
    fontSize: "{typography.scale.body.fontSize}"
    headerFontSize: "{typography.scale.label.fontSize}"
    mobileBehavior: horizontal-scroll-inside-component
breakpoints:
  docsCollapse: 960px
  dashboardCollapse: 900px
  brandGridCollapse: 800px
  desktopDemoCollapse: 760px
  mobileSystem: 720px
  dashboardSingleColumn: 560px
  narrowPhone: 420px
legal:
  affiliation: independent
  useOfficialBrandAssets: false
  bundledFontBinaries: false
  requiredLanguage:
    - Ubuntu-inspired
    - Carbon-style
  forbiddenProductNaming:
    - Ubuntu Carbon
    - Official Ubuntu
    - Official Carbon
---

# Pangolin Design System

Pangolin is an independent design-system study for Linux-flavored product interfaces. It blends an Ubuntu-inspired warmth with Carbon-style density and structure, while keeping its own name, mark, and product identity.

Use this file as the design source of truth when extending `index.html`, `pangolin/*.css`, or the demo pages in `demos/`.

## 1. Visual Theme

Pangolin should feel warm, precise, operational, and Linux-native.

The default experience is a warm paper interface: off-white backgrounds, aubergine structure, Ubuntu-orange focus/accent moments, and dense enterprise layouts that remain calm. The darker terminal theme uses aubergine as the primary atmosphere with orange as the active spark.

Do not make it look like an official Ubuntu, Canonical, IBM, or Carbon product. Use those references as descriptive influence only.

## 2. Color System

Use semantic tokens from `pangolin/tokens.css` in component CSS. Avoid hard-coding raw palette values unless building illustrative demos or charts.

Primary raw palettes:

- Aubergine: brand spine and dark surfaces.
  - `--pg-aubergine-80: #2C001E`
  - `--pg-aubergine-50: #77216F`
  - `--pg-aubergine-90: #1A0011`
- Orange: focus, selected state, sparing CTA, charts.
  - `--pg-orange-50: #E95420`
  - `--pg-orange-40: #FF7848`
  - `--pg-orange-30: #FFAE85`
- Warm neutrals: replace cool grays everywhere.
  - `--pg-warm-10: #FAF7F4`
  - `--pg-warm-30: #E8E2DA`
  - `--pg-warm-70: #6B6259`
  - `--pg-warm-100: #1B1612`

Semantic usage:

- Page background: `--pg-bg`
- Card/surface layers: `--pg-layer-01`, `--pg-layer-02`, `--pg-layer-03`
- Primary text: `--pg-text-primary`
- Secondary text: `--pg-text-secondary`
- Borders: `--pg-border-subtle-01`, `--pg-border-subtle-02`, `--pg-border-strong-01`
- Focus: `--pg-focus`, always orange
- Status: `--pg-support-success`, `--pg-support-warning`, `--pg-support-error`, `--pg-support-info`

Use orange sparingly. It should indicate action, focus, selection, or important data. Do not flood entire pages with orange.

## 3. Typography

Fonts are loaded through Google Fonts in `pangolin/base.css`; no font binaries are bundled.

Font stacks:

- Sans/display: `Ubuntu Sans`
- Mono: `Ubuntu Sans Mono`
- Fallbacks: system UI and common monospace fonts

Type scale follows Carbon productive sizing:

- `--pg-fs-01: 12px` labels/captions
- `--pg-fs-02: 14px` dense body and tables
- `--pg-fs-03: 16px` standard body
- `--pg-fs-05: 20px` ledes
- `--pg-fs-08: 32px` compact section headings
- `--pg-fs-10: 42px` chapter headings
- `--pg-fs-12: 76px` display only

Typography rules:

- Use light or regular weights for large editorial copy.
- Use 500/600 for labels, controls, table headers, and card titles.
- Keep body copy readable with `line-height: 1.45-1.6`.
- Use uppercase tracking only for overlines, tiny metadata, and system labels.
- Do not use negative letter spacing on compact controls or small UI labels.

## 4. Layout And Spacing

Use the 4px-based Carbon spacing scale from `--pg-space-01` through `--pg-space-13`.

Core rhythm:

- 8px: icon-label gaps and dense inline spacing
- 12px: form control inner spacing
- 16px: default card/control grouping
- 24px: panel padding
- 32-48px: major group spacing
- 64-96px: chapter and page spacing

Desktop docs layout:

- Sticky top bar.
- Left table of contents hidden below 960px.
- Main content maxes out inside a generous centered grid.

Mobile:

- Treat mobile as a designed layout, not squeezed desktop.
- Collapse grids to one column.
- Reduce chapter spacing.
- Make dense tables/charts scroll inside their own panels.
- Keep touch targets comfortable and avoid root-level horizontal scroll.

## 5. Shape, Depth, And Motion

Radii:

- `0`: table cell shared edges only
- `3px`: tags and tiny chips
- `6px`: inputs and buttons
- `8px`: cards and tiles
- `12px`: dialogs, windows, sheets
- `16px`: illustration/hero panels
- pill: avatars, toggles, badges

Depth:

- Use warm aubergine-tinted shadows from `--pg-shadow-01` through `--pg-shadow-04`.
- Never use pure black shadows on paper surfaces.
- Cards should feel grounded, not floating decoratively.

Motion:

- Use short productive durations: 70-150ms for interaction, 240ms for popovers, 400-700ms only for large transitions/skeletons.
- No bounce, overshoot, or playful elastic motion.

## 6. Components

Follow existing CSS classes in `pangolin/components.css`.

Buttons:

- Base: `.pg-btn`
- Variants: primary, secondary, tertiary, ghost, danger, accent
- Sizes: sm, default, lg
- Primary uses aubergine in paper theme.
- Accent uses orange and should be reserved for important CTAs.
- Icon buttons should use familiar icons and fixed square dimensions.

Forms:

- Inputs keep Carbon-like field structure: subtle border, stronger bottom/interactive edge, orange focus ring.
- Use labels and helper text consistently.
- Keep form rows dense but not cramped.

Cards/tiles:

- Use cards for repeated items, framed examples, modals, and real panels.
- Avoid nested cards inside cards unless representing a real product surface.
- Do not turn every page section into a floating card.

Tables:

- Tables are dense and product-oriented.
- Use `14px` body with `12px` headers.
- On mobile, `.pg-table` scrolls horizontally inside the component.
- Preserve row hover and selected states.

Navigation:

- Top/app bars should be restrained.
- Mobile nav should become horizontal or collapse, not squeeze.
- The demo back button uses `.pg-demo-back`.

## 7. Demo Surface Rules

Dashboard demo:

- Data-dense SaaS/observability UI.
- Prioritize KPIs, charts, alerts, and tables.
- Mobile turns sidebar into a top nav, stacks KPIs, and keeps data tables contained.

Desktop demo:

- Yaru-adjacent window chrome without using official Ubuntu assets.
- Settings panes should feel utilitarian and OS-native.
- Mobile stacks the window layout and turns side nav into horizontal nav.

Mobile demo:

- Presents phone-like surfaces.
- Keep screenshots/phone frames inspectable.
- Avoid shrinking text below practical mobile readability.

## 8. Responsive Behavior

Breakpoints currently used:

- 960px: main docs TOC hidden, doc layout becomes one column.
- 900px: dashboard demo collapses sidebar.
- 800px: brand grids collapse.
- 760px: desktop demo window stacks.
- 720px: index mobile system and table containment.
- 560px: dashboard KPIs become single column.
- 420px: narrow-phone adjustments.

Rules:

- Text must not overlap or clip.
- Long data and tables scroll inside local containers.
- Avoid root horizontal scrolling.
- Avoid viewport-scaled font formulas except for true hero/display text.
- Keep buttons and controls stable in size.

## 9. Accessibility

Requirements:

- Preserve visible focus states with orange focus rings.
- Keep text contrast high on both paper and terminal themes.
- Use semantic HTML where possible: buttons for actions, anchors for navigation.
- Add `aria-label` for icon-only controls.
- Maintain sufficient target size on mobile.
- Do not rely on color alone for critical status; pair with text or symbols.

## 10. Legal And Attribution Guardrails

Pangolin is independent. Do not imply affiliation, sponsorship, or endorsement by Canonical, Ubuntu, IBM, or Carbon.

Rules:

- Product/repo title should be `Pangolin Design System`, not `Ubuntu Carbon` or similar.
- Use `Ubuntu-inspired` and `Carbon-style` only as descriptive language.
- Do not add official Ubuntu, Canonical, IBM, or Carbon logos/assets.
- Do not bundle font binaries unless licence files and notices are restored.
- Keep `README.md` and `THIRD_PARTY_NOTICES.md` aligned with any new third-party dependency or visual asset.

## 11. Agent Prompt Guide

When extending this repo:

- Read `pangolin/tokens.css` and `pangolin/components.css` before adding new styles.
- Prefer existing token names and component classes.
- Keep changes scoped and avoid global visual rewrites.
- Build the actual usable UI, not a marketing landing page, unless explicitly requested.
- Verify at desktop and mobile widths with screenshots.
- If adding a new demo, include a back button to `../index.html#demos`.

Good prompt:

> Add a new analytics detail demo using Pangolin tokens. It should feel like the dashboard demo, be responsive, and avoid new brand/legal references.

Bad prompt:

> Make it look exactly like Ubuntu Settings or Carbon's website.
