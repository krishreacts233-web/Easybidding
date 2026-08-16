---
name: Industrial Authority
colors:
  surface: '#0f131f'
  surface-dim: '#0f131f'
  surface-bright: '#353946'
  surface-container-lowest: '#0a0e1a'
  surface-container-low: '#171b28'
  surface-container: '#1b1f2c'
  surface-container-high: '#262a37'
  surface-container-highest: '#313442'
  on-surface: '#dfe2f3'
  on-surface-variant: '#d0c5af'
  inverse-surface: '#dfe2f3'
  inverse-on-surface: '#2c303d'
  outline: '#99907c'
  outline-variant: '#4d4635'
  surface-tint: '#eac249'
  primary: '#eac249'
  on-primary: '#3d2f00'
  primary-container: '#c5a028'
  on-primary-container: '#493800'
  inverse-primary: '#745b00'
  secondary: '#c1c5dd'
  on-secondary: '#2b3042'
  secondary-container: '#414659'
  on-secondary-container: '#b0b4cb'
  tertiary: '#c0c5e2'
  on-tertiary: '#292f46'
  tertiary-container: '#9da3bf'
  on-tertiary-container: '#333950'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffe08b'
  primary-fixed-dim: '#eac249'
  on-primary-fixed: '#241a00'
  on-primary-fixed-variant: '#584400'
  secondary-fixed: '#dde1f9'
  secondary-fixed-dim: '#c1c5dd'
  on-secondary-fixed: '#161b2c'
  on-secondary-fixed-variant: '#414659'
  tertiary-fixed: '#dce1ff'
  tertiary-fixed-dim: '#c0c5e2'
  on-tertiary-fixed: '#141a30'
  on-tertiary-fixed-variant: '#40465e'
  background: '#0f131f'
  on-background: '#dfe2f3'
  surface-variant: '#313442'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-md:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  container-margin: 24px
  gutter: 16px
  sidebar-width: 280px
  card-padding: 20px
---

## Brand & Style

This design system is engineered for high-stakes industrial procurement. The personality is authoritative, precise, and secure, reflecting the significant capital managed within the portal. 

The design style utilizes a **Modern Corporate** approach with **Glassmorphic** accents. It prioritizes data density and legibility through a "Dark Mode First" philosophy. Surface hierarchy is established through subtle tonal shifts rather than aggressive shadows, creating a high-end, command-center aesthetic. The visual language conveys reliability and technical sophistication, ensuring procurement professionals feel in control of complex workflows.

## Colors

The palette is anchored by deep, obsidian-inspired tones to reduce eye strain during prolonged technical review. 

- **Primary Background (#0a0e1a):** The bedrock of the UI. All main content areas sit on this deep navy-black.
- **Surface Secondary (#161b2c):** Used for persistent navigation elements like sidebars and secondary containers.
- **Accent Gold (#c5a028):** Reserved strictly for primary actions, success states, and key financial KPIs. It provides high contrast against the dark background to drive user focus.
- **Border/Divider (#2d334a):** Defines structure without creating visual noise. Use for table row separators and component outlines.

## Typography

The system utilizes **Inter** for its exceptional legibility in dense data environments. To lean into the industrial/technical nature of procurement, **JetBrains Mono** is introduced for labels, status tags, and numerical data (IDs, SKU numbers, currency), providing a precise, "ledger-like" feel.

For mobile devices, `display-lg` should scale down to 32px, and `headline-lg` should scale to 24px. All body text remains constant to ensure readability. High-contrast white (`#f8f9fa`) is used for headings, while light gray (`#e9ecef`) is used for secondary body copy to manage information hierarchy.

## Layout & Spacing

This design system uses a **12-column fluid grid** for the main content area with a fixed-width sidebar at 280px. The spacing rhythm is based on a **4px baseline grid**.

- **Desktop:** 24px margins with 16px gutters. KPI cards typically span 3 columns (4 per row).
- **Tablet:** 16px margins. Sidebar collapses into an icon-only rail or drawer.
- **Mobile:** 16px margins. Content stacks vertically. Data tables should transition to a card-based list view or horizontal scroll.

Information density is "Medium-High." Use consistent 20px padding for cards and containers to maintain a structured, professional balance.

## Elevation & Depth

Hierarchy is achieved through **Tonal Layering** and **Glassmorphic** overlays.

1.  **Level 0 (Base):** `#0a0e1a` - The background.
2.  **Level 1 (Cards/Sidebar):** `#161b2c` - Primary containers.
3.  **Level 2 (Modals/Popovers):** `#2d334a` with a 20px backdrop blur and 40% opacity. 

Shadows are used sparingly. When required, use a large, diffused black shadow (`0px 8px 24px rgba(0,0,0,0.5)`) to lift interactive elements like modals or active dropdowns. Avoid inner shadows or heavy glows to keep the interface feeling grounded and professional.

## Shapes

The shape language balances modern aesthetics with industrial rigor. 

- **Containers (Cards, Modals):** Use `rounded-lg` (16px) to soften the dark interface and make the portal feel accessible despite its complexity.
- **Interactive Elements (Buttons, Inputs):** Use `rounded-md` (8px) for a sharper, more precise appearance.
- **Status Badges:** Use full pills (999px) to clearly differentiate "Status" from "Action" elements.

## Components

### Buttons
- **Primary:** Solid Gold (`#c5a028`) with Black text. Bold weight.
- **Secondary:** Outlined with Gold border or Ghost style with White text.
- **Destructive:** Deep Red (`#991b1b`) with White text.

### Inputs & Selects
- Background should be one shade darker than the parent container.
- Borders use the `#2d334a` token, turning Gold on focus.
- Monospaced font (JetBrains Mono) for numerical inputs.

### KPI Cards
- Feature a large `headline-lg` value in Gold or White.
- Include a small sparkline or percentage change indicator in the bottom right.
- 1px border using `#2d334a`.

### Data Tables
- Header background: `#161b2c`.
- Row dividers: 1px solid `#2d334a`.
- Row hover state: Subtle highlight using `#1e2538`.
- Use "Compact" vertical padding (12px) to maximize data visibility.

### Sidebar Navigation
- Icons: 24px, light gray. Active state: Gold.
- Background: `#161b2c`.
- Include a "Secured Connection" indicator at the bottom to reinforce the trust narrative.