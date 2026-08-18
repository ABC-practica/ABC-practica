# Design Tokens

## Overview

This document defines the shared design tokens (colors, typography, spacing, and other design properties) used across all applications in our organization. All teams should reference these tokens to maintain visual and functional consistency.

---

## Color Palette

### Primary Colors by App

Each application has its own primary color while maintaining consistent secondary, semantic, and neutral colors across the organization.

#### Archeology App (Terracotta / Earth)

| Token Name | Hex Value | RGB | Usage |
|---|---|---|---|
| `color-primary` | `#C85A32` | `rgb(200, 90, 50)` | Primary buttons, links, active states |
| `color-primary-light` | `#FBECE5` | `rgb(251, 236, 229)` | Light backgrounds, hover states |
| `color-primary-dark` | `#8C3717` | `rgb(140, 55, 23)` | Pressed states, dark mode primary |

#### Biology App (Emerald / Flora)

| Token Name | Hex Value | RGB | Usage |
|---|---|---|---|
| `color-primary` | `#1B8755` | `rgb(27, 135, 85)` | Primary buttons, links, active states |
| `color-primary-light` | `#E8F6EF` | `rgb(232, 246, 239)` | Light backgrounds, hover states |
| `color-primary-dark` | `#0E5233` | `rgb(14, 82, 51)` | Pressed states, dark mode primary |

#### Geology App (Slate Blue / Mineral)

| Token Name | Hex Value | RGB | Usage |
|---|---|---|---|
| `color-primary` | `#4F6B7E` | `rgb(79, 107, 126)` | Primary buttons, links, active states |
| `color-primary-light` | `#EEF3F6` | `rgb(238, 243, 246)` | Light backgrounds, hover states |
| `color-primary-dark` | `#2D3E4A` | `rgb(45, 62, 74)` | Pressed states, dark mode primary |

### Secondary Colors

| Token Name | Hex Value | RGB | Usage |
|---|---|---|---|
| `color-secondary` | `#D97706` | `rgb(217, 119, 6)` | Secondary actions, accents (Amber) |
| `color-secondary-light` | `#FEF3C7` | `rgb(254, 243, 199)` | Secondary backgrounds |

### Semantic Colors

| Token Name | Hex Value | Usage |
|---|---|---|
| `color-success` | `#16A34A` | Success messages, positive states |
| `color-warning` | `#EA580C` | Warning messages, caution states |
| `color-error` | `#DC2626` | Error messages, destructive actions |
| `color-info` | `#2563EB` | Informational messages |

### Neutral Colors

| Token Name | Hex Value | Usage |
|---|---|---|
| `color-neutral-100` | `#F8FAFC` | Lightest backgrounds |
| `color-neutral-500` | `#64748B` | Secondary text, disabled states |
| `color-neutral-900` | `#0F172A` | Primary text, dark backgrounds |

---

## Typography

### Font Families

- **Primary Font:** `Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif`
- **Monospace Font:** `"JetBrains Mono", "Fira Code", monospace`

### Font Sizes

| Token Name | Size (px) | Line Height | Usage |
|---|---|---|---|
| `font-size-xs` | `12px` | `16px` | Caption, help text |
| `font-size-sm` | `14px` | `20px` | Body small, labels |
| `font-size-base` | `16px` | `24px` | Body text, default |
| `font-size-lg` | `18px` | `28px` | Subheadings |
| `font-size-xl` | `20px` | `28px` | Section headings |
| `font-size-2xl` | `24px` | `32px` | Page titles |

### Font Weights

| Token Name | Weight | Usage |
|---|---|---|
| `font-weight-regular` | `400` | Body text |
| `font-weight-medium` | `500` | Labels, emphasis |
| `font-weight-semibold` | `600` | Subheadings |
| `font-weight-bold` | `700` | Headings, strong emphasis |

---

## Spacing

All spacing values follow an 8-point base unit system (with 4px for fine-tuning).

| Token Name | Value (px) | Value (rem) | Usage |
|---|---|---|---|
| `spacing-1` | `4px` | `0.25rem` | Minimal spacing |
| `spacing-2` | `8px` | `0.5rem` | Tight spacing, padding |
| `spacing-3` | `12px` | `0.75rem` | Small gaps |
| `spacing-4` | `16px` | `1rem` | Standard padding, margins |
| `spacing-6` | `24px` | `1.5rem` | Medium gaps |
| `spacing-8` | `32px` | `2rem` | Large margins |
| `spacing-12` | `48px` | `3rem` | Section spacing |

---

## Border Radius

| Token Name | Value | Usage |
|---|---|---|
| `border-radius-sm` | `4px` | Subtle rounding |
| `border-radius-md` | `8px` | Standard components (buttons, cards) |
| `border-radius-lg` | `16px` | Large containers, modals |
| `border-radius-full` | `9999px` | Circular elements, avatars |

---

## Shadows

| Token Name | CSS Value | Usage |
|---|---|---|
| `shadow-sm` | `0 1px 2px 0 rgb(0 0 0 / 0.05)` | Subtle elevation |
| `shadow-md` | `0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1)` | Standard cards, dropdowns |
| `shadow-lg` | `0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1)` | Elevated modals, popovers |
| `shadow-xl` | `0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1)` | Maximum elevation |

---

## Usage Guidelines

### Implementation

Use these tokens in your stylesheets via CSS variables or your framework's theming system. For app-specific primary colors, use the appropriate color tokens based on your application.

**CSS Variables (Archeology App):**
```css
:root {
  --color-primary: #C85A32;
  --color-primary-light: #FBECE5;
  --color-primary-dark: #8C3717;
  --spacing-4: 1rem;
}

.button {
  background-color: var(--color-primary);
  padding: var(--spacing-4);
}
```

**CSS Variables (Biology App):**
```css
:root {
  --color-primary: #1B8755;
  --color-primary-light: #E8F6EF;
  --color-primary-dark: #0E5233;
  --spacing-4: 1rem;
}

.button {
  background-color: var(--color-primary);
  padding: var(--spacing-4);
}
```

**CSS Variables (Geology App):**
```css
:root {
  --color-primary: #4F6B7E;
  --color-primary-light: #EEF3F6;
  --color-primary-dark: #2D3E4A;
  --spacing-4: 1rem;
}

.button {
  background-color: var(--color-primary);
  padding: var(--spacing-4);
}
```

### Dark Mode

For dark mode support, override color tokens as needed:

| Token Name | Light Mode | Dark Mode |
|---|---|---|
| `color-neutral-900` | `#0F172A` | `#F8FAFC` |
| `color-neutral-100` | `#F8FAFC` | `#0F172A` |

---

## Updates and Maintenance

- **Last Updated:** August 2026

To propose changes, open an issue or pull request in the central repository.
