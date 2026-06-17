---
name: SignalPad Canary
colors:
  surface: '#f8f9fb'
  surface-dim: '#d9dadc'
  surface-bright: '#f8f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f4f6'
  surface-container: '#edeef0'
  surface-container-high: '#e7e8ea'
  surface-container-highest: '#e1e2e4'
  on-surface: '#191c1e'
  on-surface-variant: '#434654'
  inverse-surface: '#2e3132'
  inverse-on-surface: '#f0f1f3'
  outline: '#737685'
  outline-variant: '#c3c6d6'
  surface-tint: '#0c56d0'
  primary: '#003d9b'
  on-primary: '#ffffff'
  primary-container: '#0052cc'
  on-primary-container: '#c4d2ff'
  inverse-primary: '#b2c5ff'
  secondary: '#535f73'
  on-secondary: '#ffffff'
  secondary-container: '#d4e0f8'
  on-secondary-container: '#576377'
  tertiary: '#7b2600'
  on-tertiary: '#ffffff'
  tertiary-container: '#a33500'
  on-tertiary-container: '#ffc6b2'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2ff'
  primary-fixed-dim: '#b2c5ff'
  on-primary-fixed: '#001848'
  on-primary-fixed-variant: '#0040a2'
  secondary-fixed: '#d7e3fb'
  secondary-fixed-dim: '#bbc7de'
  on-secondary-fixed: '#101c2d'
  on-secondary-fixed-variant: '#3b475b'
  tertiary-fixed: '#ffdbcf'
  tertiary-fixed-dim: '#ffb59b'
  on-tertiary-fixed: '#380d00'
  on-tertiary-fixed-variant: '#812800'
  background: '#f8f9fb'
  on-background: '#191c1e'
  surface-variant: '#e1e2e4'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '500'
    lineHeight: 14px
  mono-data:
    fontFamily: monospace
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 20px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 24px
---

## Brand & Style
The design system is engineered for high-stakes operational environments where clarity and data density are paramount. The brand personality is **deterministic, reliable, and utilitarian**, mirroring the precision of industrial monitoring tools. 

The aesthetic follows a **Modern Corporate/Industrial** approach:
- **Minimalist Complexity:** Large amounts of data are organized through rigorous alignment and subtle tonal shifts rather than heavy decorative elements.
- **Functional Density:** The UI prioritizes information per square inch while maintaining optical balance to prevent cognitive overload.
- **Deterministic UI:** Every interaction and state change is explicit, using a consistent logic that minimizes ambiguity for professional users.

## Colors
The palette is built on a foundation of professional blues and cool grays to foster a calm, focused working environment.

- **Primary Blue (#0052CC):** Used strictly for primary actions, active navigation states, and progress indicators.
- **Neutral Grays:** `#F4F5F7` provides a soft canvas for surfaces, while `#DFE1E6` defines boundaries and structural grids.
- **Semantic Colors:** Status indicators use high-saturation tones for immediate recognition:
  - **Success (#36B37E):** Positive operations and "healthy" status.
  - **Warning (#FFAB00):** Cautionary states and pending actions.
  - **Error (#FF5630):** Critical failures or required interventions.

## Typography
Inter is used across the system for its exceptional legibility at small sizes and its neutral, systematic character.

- **Hierarchy:** Established through weight shifts rather than dramatic size changes to maintain density.
- **Monospace:** Technical data, IDs, and timestamps should utilize a system monospace font to ensure character alignment in tabular views.
- **Labels:** Small, uppercase labels are used for metadata and table headers to distinguish them from actionable or editable content.

## Layout & Spacing
The system utilizes a **4px baseline grid** for internal component spacing and a **12-column fluid grid** for page layout.

- **Data Density:** Gutters are kept at a tight 16px to maximize horizontal space for data tables and dashboards.
- **Fixed Sidebar:** Primary navigation resides in a fixed 240px left-hand sidebar to provide a consistent frame for operational workflows.
- **Responsive Reflow:** At 768px (Tablet), the sidebar collapses to icons. Below 480px, data tables should transition to card-based layouts or horizontal scrolling with frozen columns.

## Elevation & Depth
Depth is conveyed through **Tonal Layering** and **Low-Contrast Outlines** rather than shadows. This minimizes visual clutter in dense interfaces.

- **Surface Levels:** 
  - Level 0 (Background): `#F4F5F7`
  - Level 1 (Cards/Work Areas): `#FFFFFF`
  - Level 2 (Popovers/Modals): `#FFFFFF` with a 1px border of `#DFE1E6` and a subtle 4px blur shadow.
- **Borders:** Every container must have a 1px solid border (`#DFE1E6`) to clearly define its boundaries against the light gray background.

## Shapes
This design system uses **Soft (0.25rem)** roundedness to balance the industrial aesthetic with modern software expectations.

- **Standard Elements:** Buttons, inputs, and tags use a 4px radius.
- **Large Containers:** Cards and panels may use up to 8px (`rounded-lg`) to create clear containment.
- **Selection Indicators:** Active states in sidebars or tabs use a sharp 0px radius on the leading edge to suggest "connection" to the active content pane.

## Components
- **Buttons:**
  - **Primary:** Solid `#0052CC` with white text. High contrast for critical actions.
  - **Secondary:** White background with `#DFE1E6` border and `#42526E` text.
  - **Tertiary/Ghost:** No border or background until hover.
- **Form Fields:** Must include a persistent 1px border. Validation states (Error/Success) must change the border color and include a supporting icon for accessibility.
- **Data Tables:** High-density rows (32px-40px height). Zebra striping is discouraged; use subtle 1px horizontal dividers instead.
- **Status Badges:** Small, "lo-fi" tags with light background tints and dark text (e.g., Success: Background 10% opacity of `#36B37E`, Text solid `#36B37E`).
- **Input Groups:** Use "Prepend" or "Append" blocks for units (e.g., "ms", "kb") to keep data entries unambiguous.