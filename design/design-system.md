# LAOS Brand — Design System

> A 3,000-year inversion made visible.
> The laurel was exclusive. The intelligence doesn't have to be.

## Core Metaphor

The imperial laurel → the sovereign laós. LAOS dissolves the crown and
distributes sovereignty to every operator. The design system lives at
the tension between **authority** (purple, gold, structured grids,
editorial serifs) and **access** (warm paper, open space, human scale,
clean sans).

This is not a "democratize AI" brand. This is an inversion of hierarchy.
Every token, every rule, every component serves that idea.

## Palette

### Primary — Imperial Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--laos-clr-accent` | `#3B1F5E` | Laurel purple — flagship accent, primary CTAs, brand mark |
| `--laos-clr-gold` | `#C8A951` | Antique gold — secondary accent, highlights, data emphasis |
| `--laos-clr-ink` | `#0A0A0A` | Near-black — body text, dark mode surface |
| `--laos-clr-paper` | `#F7F5EE` | Warm cream — light mode background, card surfaces |

### Light Mode — Surface & Text

| Token | Hex | Role |
|-------|-----|------|
| `--laos-clr-surface` | `#FFFFFF` | Page background |
| `--laos-clr-surface-elevated` | `#F7F5EE` | Card / panel background |
| `--laos-clr-surface-raised` | `#FFFFFF` | Modal / dropdown |
| `--laos-clr-text-primary` | `#0A0A0A` | Body text |
| `--laos-clr-text-secondary` | `#5A5A5A` | Supporting text |
| `--laos-clr-text-accent` | `#3B1F5E` | Accent text (links, highlights) |
| `--laos-clr-text-inverse` | `#F7F5EE` | Text on dark surfaces |
| `--laos-clr-border` | `#D4D0C8` | Default borders, dividers |
| `--laos-clr-border-accent` | `#3B1F5E` | Accent borders, focus rings |

### Dark Mode — Surface & Text

| Token | Hex | Role |
|-------|-----|------|
| `--laos-clr-surface` | `#0A0A0A` | Page background |
| `--laos-clr-surface-elevated` | `#1A1A1A` | Card / panel background |
| `--laos-clr-surface-raised` | `#252525` | Modal / dropdown |
| `--laos-clr-text-primary` | `#F7F5EE` | Body text |
| `--laos-clr-text-secondary` | `#9C9C9C` | Supporting text |
| `--laos-clr-text-accent` | `#B896E0` | Accent text (lighter for legibility on dark) |
| `--laos-clr-text-inverse` | `#0A0A0A` | Text on light surfaces |
| `--laos-clr-border` | `#2A2A2A` | Default borders, dividers |
| `--laos-clr-border-accent` | `#B896E0` | Accent borders, focus rings |

### Semantic

| Token | Hex | Role |
|-------|-----|------|
| `--laos-clr-success` | `#2D6A4F` | Positive actions, confirmation |
| `--laos-clr-warning` | `#D4A017` | Caution, attention needed |
| `--laos-clr-error` | `#B71C1C` | Destructive actions, errors |
| `--laos-clr-info` | `#1A3A8A` | Informational, neutral updates |

## Typography

### Font Stack

| Role | Family | Weights | Fallback |
|------|--------|---------|----------|
| Heading (editorial) | **Playfair Display** | 400, 600, 700, 900 | Georgia, serif |
| Body (clean) | **Inter** | 300, 400, 500, 600, 700 | system-ui, sans-serif |
| Display (deck) | **Inter Tight** | 400, 500, 600, 700, 800, 900 | Inter, sans-serif |
| Monospace | **JetBrains Mono** | 400, 500 | Consolas, monospace |

### Type Scale

| Level | Size | Weight | Line Height | Tracking | Usage |
|-------|------|--------|-------------|----------|-------|
| Hero | `clamp(48px, 9.6vw, 128px)` | 900 (Playfair) / 800 (Inter Tight) | 0.95 | -0.02em | Landing page hero, cover slide |
| Display | `clamp(36px, 5.6vw, 80px)` | 700 | 1.05 | -0.015em | Section headings, statement slides |
| H2 | `clamp(28px, 2.8vw, 48px)` | 700 | 1.1 | -0.01em | Major section titles |
| H3 | `24px` | 600 | 1.2 | — | Card titles, sub-sections |
| H4 | `20px` | 600 | 1.3 | — | Minor headings |
| Body | `16px` / `1rem` | 400 | 1.6 | — | Paragraphs |
| Body Small | `14px` | 400 | 1.5 | — | Supporting text, captions |
| Label | `11px` | 500 | 1.3 | `0.08em` uppercase | Badge, tag, meta |
| Code | `14px` | 400 | 1.5 | — | Inline code, terminal blocks |
| Data | `12px` | 500 (JetBrains Mono) | 1.3 | — | Charts, tables, KPIs |

## Spacing & Grid

### Base Unit

**8px** — all spacing values are multiples of 8.

| Token | Value |
|-------|-------|
| `--laos-space-1` | 4px (half) |
| `--laos-space-2` | 8px |
| `--laos-space-3` | 12px |
| `--laos-space-4` | 16px |
| `--laos-space-5` | 24px |
| `--laos-space-6` | 32px |
| `--laos-space-7` | 48px |
| `--laos-space-8` | 64px |
| `--laos-space-9` | 96px |
| `--laos-space-10` | 128px |

### Grid

| Context | Columns | Gap | Max Width |
|---------|---------|-----|-----------|
| Web / landing page | 12 | 24px | 1280px |
| Deck / presentation | 16 | 0 (hairline) | 1920px |
| Dashboard | 12 | 16px | 1440px |

### Breakpoints

| Name | Width | Target |
|------|-------|--------|
| Mobile | `< 640px` | Phones |
| Tablet | `640px – 1024px` | Tablets, small laptops |
| Desktop | `1024px – 1440px` | Standard monitors |
| Wide | `> 1440px` | Large screens, deck projection |

## Token Naming Convention

```
--laos-{category}-{property}-{variant}
```

### Categories

| Category | Prefix | Examples |
|----------|--------|---------|
| Color | `clr` | `--laos-clr-accent`, `--laos-clr-surface-elevated` |
| Typography | `type` | `--laos-type-family-heading`, `--laos-type-size-hero` |
| Spacing | `space` | `--laos-space-4`, `--laos-space-8` |
| Border | `border` | `--laos-border-radius-sm`, `--laos-border-width-default` |
| Shadow | `shadow` | `--laos-shadow-sm`, `--laos-shadow-lg` |
| Motion | `motion` | `--laos-motion-fast`, `--laos-motion-ease-out` |
| Layout | `layout` | `--laos-layout-max-width`, `--laos-layout-grid-gap` |
| Z-index | `z` | `--laos-z-dropdown`, `--laos-z-modal` |

## Borders & Radius

| Token | Value | Usage |
|-------|-------|-------|
| `--laos-border-radius-none` | `0` | Swiss layout, deck cards, tech specs |
| `--laos-border-radius-sm` | `4px` | Buttons, inputs, subtle cards |
| `--laos-border-radius-md` | `8px` | Cards, modals, panels |
| `--laos-border-radius-lg` | `12px` | Elevated containers |
| `--laos-border-width-default` | `1px` | Default borders |
| `--laos-border-width-thick` | `2px` | Accent borders, focus rings |

## Shadows

| Token | Value |
|-------|-------|
| `--laos-shadow-sm` | `0 1px 2px rgba(10,10,10,0.08)` |
| `--laos-shadow-md` | `0 4px 12px rgba(10,10,10,0.1)` |
| `--laos-shadow-lg` | `0 8px 32px rgba(10,10,10,0.14)` |
| `--laos-shadow-glow` | `0 0 20px rgba(59,31,94,0.25)` |
| `--laos-shadow-glow-gold` | `0 0 20px rgba(200,169,81,0.25)` |

## Component Specifications

### Button — Primary

```css
.laos-btn-primary {
  background: var(--laos-clr-accent, #3B1F5E);
  color: var(--laos-clr-text-inverse, #F7F5EE);
  font-family: Inter, system-ui, sans-serif;
  font-weight: 600;
  font-size: 14px;
  padding: 12px 24px;
  border-radius: var(--laos-border-radius-sm, 4px);
  border: 1px solid transparent;
  cursor: pointer;
  transition: background 200ms ease, transform 150ms ease;
}
.laos-btn-primary:hover {
  background: #4D2A75;
}
.laos-btn-primary:active {
  transform: scale(0.97);
}
```

### Button — Secondary (Gold)

```css
.laos-btn-gold {
  background: transparent;
  color: var(--laos-clr-gold, #C8A951);
  border: 1px solid var(--laos-clr-gold, #C8A951);
  font-weight: 500;
  /* same sizing as primary */
}
.laos-btn-gold:hover {
  background: rgba(200,169,81,0.08);
}
```

### Card

```css
.laos-card {
  background: var(--laos-clr-surface-elevated, #F7F5EE);
  border: 1px solid var(--laos-clr-border, #D4D0C8);
  border-radius: var(--laos-border-radius-md, 8px);
  padding: var(--laos-space-5, 24px);
}
```

### Navigation — Top Bar

```css
.laos-nav {
  display: flex;
  align-items: center;
  gap: 24px;
  padding: 16px 24px;
  background: var(--laos-clr-surface, #FFFFFF);
  border-bottom: 1px solid var(--laos-clr-border, #D4D0C8);
}
```

## Motion

| Token | Value |
|-------|-------|
| `--laos-motion-fast` | `150ms` |
| `--laos-motion-normal` | `250ms` |
| `--laos-motion-slow` | `400ms` |
| `--laos-motion-ease-out` | `cubic-bezier(0.22, 1, 0.36, 1)` |
| `--laos-motion-ease-in-out` | `cubic-bezier(0.65, 0, 0.35, 1)` |

- Transitions prefer `transform` and `opacity` for GPU acceleration.
- Staggered reveals use `200ms` delay per element.
- No decorative motion without purpose.

## Usage Rules

### Do
- Use purple (#3B1F5E) as primary accent — CTAs, links, brand marks, icons.
- Use gold (#C8A951) sparingly — data highlights, emphasis, decorative accents.
- Default to warm paper (#F7F5EE) for light mode backgrounds.
- Keep 8px rhythm: every margin, padding, gap is a multiple of 8.
- Use Playfair Display for dramatic headlines and section statements.
- Use Inter for all body text, labels, UI controls.

### Don't
- ❌ Never mix purple and gold equally — one must dominate.
- ❌ Never use purple on purple (insufficient contrast).
- ❌ Never use generic blue SaaS gradients.
- ❌ Never use rounded cards in deck/presentation context (use `border-radius: 0`).
- ❌ Never apply shadows to cards in dense data layouts.
- ❌ Never use lorem ipsum or placeholder copy.

## Accessibility

- All text/background pairs meet WCAG 2.1 AA contrast (4.5:1 normal, 3:1 large).
- Purple on white: contrast ratio ~8.5:1 ✅
- Gold on white: contrast ratio ~2.8:1 ❌ (for body text) — gold is decorative/display only.
- Gold on dark (#C8A951 on #0A0A0A): ~7.2:1 ✅
- Focus rings use `--laos-clr-border-accent` at 2px width.
- Motion respects `prefers-reduced-motion`.

## File Reference

Per `design/source.md`, this document is the active design contract
for all visual artifacts in the `laurentaf/laos-brand` repository.
