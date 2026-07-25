# Design System

> Visual and interaction standards for every product in the ecosystem.

This document is the single source of truth for colors, typography, spacing, and components. Every project should follow it.

---

## Colors

### Background

| Token | Value | Usage |
|-------|-------|-------|
| `bg-primary` | `#0B0B0C` | Main canvas |
| `bg-secondary` | `#111111` | Cards, elevated surfaces |
| `bg-tertiary` | `#171717` | Hover states, subtle separation |

### Text

| Token | Value | Usage |
|-------|-------|-------|
| `text-primary` | `#F5F5F5` | Headings, body |
| `text-secondary` | `#8B8B8B` | Captions, meta, labels |
| `text-tertiary` | `#5A5A5A` | Disabled, placeholders |

### Border

| Token | Value | Usage |
|-------|-------|-------|
| `border-default` | `#1F1F1F` | Dividers, outlines |
| `border-hover` | `#333333` | Hover borders |

### Accent

| Token | Value | Usage |
|-------|-------|-------|
| `accent` | `#7C5CFC` | Primary actions, links, highlights |
| `accent-soft` | `rgba(124, 92, 252, 0.12)` | Subtle backgrounds |

### Semantic

| Token | Value | Usage |
|-------|-------|-------|
| `success` | `#22C55E` | Positive states |
| `warning` | `#EAB308` | Alerts |
| `error` | `#EF4444` | Errors |

---

## Typography

### Typefaces

- **Primary:** Inter
- **Serif:** IBM Plex Serif (for emphasis and editorial moments)
- **Monospace:** JetBrains Mono or Geist Mono

### Scale

| Token | Size | Weight | Line Height | Usage |
|-------|------|--------|-------------|-------|
| `display` | 72px / 56px mobile | 700 | 1.05 | Hero |
| `h1` | 48px / 36px mobile | 700 | 1.1 | Page titles |
| `h2` | 32px / 26px mobile | 600 | 1.2 | Section titles |
| `h3` | 24px / 20px mobile | 600 | 1.3 | Subsections |
| `body-large` | 18px | 400 | 1.7 | Lead paragraphs |
| `body` | 16px | 400 | 1.6 | Main text |
| `caption` | 13px | 500 | 1.5 | Labels, meta |
| `code` | 14px | 400 | 1.6 | Code blocks |

### Rules

- Use tight line-height for headings.
- Use comfortable line-height for body text.
- Limit to two typefaces per project.
- Use serif sparingly, for emphasis.

---

## Spacing

Base unit: **8px**

| Token | Value |
|-------|-------|
| `space-1` | 4px |
| `space-2` | 8px |
| `space-3` | 16px |
| `space-4` | 24px |
| `space-5` | 32px |
| `space-6` | 48px |
| `space-7` | 64px |
| `space-8` | 96px |
| `space-9` | 128px |

### Section Spacing

- Large sections: `128px` – `160px` vertical padding
- Medium sections: `80px` – `96px`
- Small sections: `40px` – `64px`

---

## Radius

| Token | Value | Usage |
|-------|-------|-------|
| `radius-sm` | 6px | Buttons, inputs |
| `radius-md` | 12px | Cards, blocks |
| `radius-lg` | 16px | Large cards |
| `radius-xl` | 24px | Modals, device frames |
| `radius-full` | 9999px | Pills, badges |

---

## Shadows

Use shadows rarely. Prefer borders and background contrast.

| Token | Value | Usage |
|-------|-------|-------|
| `shadow-sm` | `0 4px 12px rgba(0,0,0,0.2)` | Subtle elevation |
| `shadow-lg` | `0 48px 120px rgba(0,0,0,0.45)` | Device frames, modals |

---

## Buttons

### Primary

- Background: `accent`
- Text: `#FFFFFF`
- Padding: `12px 24px`
- Radius: `radius-md`
- Font: `14px`, weight `600`

### Secondary

- Background: transparent
- Border: `1px solid border-default`
- Text: `text-primary`
- Padding: `12px 24px`
- Radius: `radius-md`

### Ghost

- Background: transparent
- Text: `text-secondary`
- Hover: `text-primary`

---

## Cards

- Background: `bg-secondary`
- Border: `1px solid border-default`
- Radius: `radius-lg`
- Padding: `24px` – `32px`
- Hover: border transitions to `border-hover`

---

## Motion

### Principles

- Motion should be almost invisible.
- Use motion to guide, not decorate.
- Respect `prefers-reduced-motion`.

### Allowed

- `opacity` transitions
- `translateY` entrances
- Subtle `scale` on hover
- `blur` transitions sparingly

### Forbidden

- Bouncing
- Spinning
- Flashing
- Neon glows
- Complex 3D transforms

### Timing

- Fast interactions: `150ms`
- Entrances: `600ms` – `900ms`
- Easing: `cubic-bezier(0.25, 0.1, 0.25, 1)`

---

## Icons

- Use a single icon library per project.
- Default: Lucide or Phosphor Icons.
- Keep consistent stroke width and size.
- Do not mix icon styles.

---

## Code Style

- Use monospace for inline code.
- Code blocks: dark background, `radius-md`, `16px` padding.
- Syntax highlighting optional, keep minimal.

---

## Accessibility

- Minimum contrast ratio: 4.5:1 for text.
- Focus states must be visible.
- Use semantic HTML.
- Add alt text to images.
- Support keyboard navigation.

---

## How to Use

1. Reference these tokens in every new project.
2. Do not introduce new colors or fonts without updating this document.
3. If a component is missing, design it using these tokens and document it here.

---

*This design system is part of the [Personal Operating Manual](https://github.com/eupho808/personal-brand-bible).*
