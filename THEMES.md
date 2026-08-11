# Design Tokens

## Overview

This document defines the shared design tokens (colors, typography, spacing, and other design properties) used across all applications in our organization. All teams should reference these tokens to maintain visual and functional consistency.

---

## Color Palette

### Primary Colors by App

Each application has its own primary color while maintaining consistent secondary, semantic, and neutral colors across the organization.

#### Archeology App

| Token Name | Hex Value | RGB | Usage |
|---|---|---|---|
| `color-primary` | TBD | TBD | Primary buttons, links, active states |
| `color-primary-light` | TBD | TBD | Light backgrounds, hover states |
| `color-primary-dark` | TBD | TBD | Pressed states, dark mode primary |

#### Biology App

| Token Name | Hex Value | RGB | Usage |
|---|---|---|---|
| `color-primary` | TBD | TBD | Primary buttons, links, active states |
| `color-primary-light` | TBD | TBD | Light backgrounds, hover states |
| `color-primary-dark` | TBD | TBD | Pressed states, dark mode primary |

#### Geology App

| Token Name | Hex Value | RGB | Usage |
|---|---|---|---|
| `color-primary` | TBD | TBD | Primary buttons, links, active states |
| `color-primary-light` | TBD | TBD | Light backgrounds, hover states |
| `color-primary-dark` | TBD | TBD | Pressed states, dark mode primary |

### Secondary Colors

| Token Name | Hex Value | RGB | Usage |
|---|---|---|---|
| `color-secondary` | TBD | TBD | Secondary actions, accents |
| `color-secondary-light` | TBD | TBD | Secondary backgrounds |

### Semantic Colors

| Token Name | Hex Value | Usage |
|---|---|---|
| `color-success` | TBD | Success messages, positive states |
| `color-warning` | TBD | Warning messages, caution states |
| `color-error` | TBD | Error messages, destructive actions |
| `color-info` | TBD | Informational messages |

### Neutral Colors

| Token Name | Hex Value | Usage |
|---|---|---|
| `color-neutral-100` | TBD | Lightest backgrounds |
| `color-neutral-500` | TBD | Secondary text, disabled states |
| `color-neutral-900` | TBD | Primary text, dark backgrounds |

---

## Typography

### Font Families

- **Primary Font:** TBD
- **Monospace Font:** TBD

### Font Sizes

| Token Name | Size (px) | Line Height | Usage |
|---|---|---|---|
| `font-size-xs` | TBD | TBD | Caption, help text |
| `font-size-sm` | TBD | TBD | Body small, labels |
| `font-size-base` | TBD | TBD | Body text, default |
| `font-size-lg` | TBD | TBD | Subheadings |
| `font-size-xl` | TBD | TBD | Section headings |
| `font-size-2xl` | TBD | TBD | Page titles |

### Font Weights

| Token Name | Weight | Usage |
|---|---|---|
| `font-weight-regular` | TBD | Body text |
| `font-weight-medium` | TBD | Labels, emphasis |
| `font-weight-semibold` | TBD | Subheadings |
| `font-weight-bold` | TBD | Headings, strong emphasis |

---

## Spacing

All spacing values follow a base unit system.

| Token Name | Value (px) | Value (rem) | Usage |
|---|---|---|---|
| `spacing-1` | TBD | TBD | Minimal spacing |
| `spacing-2` | TBD | TBD | Tight spacing, padding |
| `spacing-3` | TBD | TBD | Small gaps |
| `spacing-4` | TBD | TBD | Standard padding, margins |
| `spacing-6` | TBD | TBD | Medium gaps |
| `spacing-8` | TBD | TBD | Large margins |
| `spacing-12` | TBD | TBD | Section spacing |

---

## Border Radius

| Token Name | Value | Usage |
|---|---|---|
| `border-radius-sm` | TBD | Subtle rounding |
| `border-radius-md` | TBD | Standard components (buttons, cards) |
| `border-radius-lg` | TBD | Large containers, modals |
| `border-radius-full` | TBD | Circular elements, avatars |

---

## Shadows

| Token Name | CSS Value | Usage |
|---|---|---|
| `shadow-sm` | TBD | Subtle elevation |
| `shadow-md` | TBD | Standard cards, dropdowns |
| `shadow-lg` | TBD | Elevated modals, popovers |
| `shadow-xl` | TBD | Maximum elevation |

---

## Usage Guidelines

### Implementation

Use these tokens in your stylesheets via CSS variables or your framework's theming system. For app-specific primary colors, use the appropriate color tokens based on your application.

**CSS Variables (Archeology App):**
```css
:root {
  --color-primary: TBD;
  --color-primary-light: TBD;
  --color-primary-dark: TBD;
  --spacing-4: TBD;
}

.button {
  background-color: var(--color-primary);
  padding: var(--spacing-4);
}
```

**CSS Variables (Biology App):**
```css
:root {
  --color-primary: TBD;
  --color-primary-light: TBD;
  --color-primary-dark: TBD;
  --spacing-4: TBD;
}

.button {
  background-color: var(--color-primary);
  padding: var(--spacing-4);
}
```

**CSS Variables (Geology App):**
```css
:root {
  --color-primary: TBD;
  --color-primary-light: TBD;
  --color-primary-dark: TBD;
  --spacing-4: TBD;
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
| `color-neutral-900` | TBD | TBD |
| `color-neutral-100` | TBD | TBD |

---

## Updates and Maintenance

- **Last Updated:** August 2026

To propose changes, open an issue or pull request in the central repository.
