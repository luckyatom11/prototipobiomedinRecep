---
name: Clinical Precision System
colors:
  surface: '#f8f9fa'
  surface-dim: '#d9dadb'
  surface-bright: '#f8f9fa'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f4f5'
  surface-container: '#edeeef'
  surface-container-high: '#e7e8e9'
  surface-container-highest: '#e1e3e4'
  on-surface: '#191c1d'
  on-surface-variant: '#424752'
  inverse-surface: '#2e3132'
  inverse-on-surface: '#f0f1f2'
  outline: '#727784'
  outline-variant: '#c2c6d4'
  surface-tint: '#115cb9'
  primary: '#003f87'
  on-primary: '#ffffff'
  primary-container: '#0056b3'
  on-primary-container: '#bbd0ff'
  inverse-primary: '#acc7ff'
  secondary: '#555f6b'
  on-secondary: '#ffffff'
  secondary-container: '#d9e3f1'
  on-secondary-container: '#5b6571'
  tertiary: '#3a434a'
  on-tertiary: '#ffffff'
  tertiary-container: '#515a62'
  on-tertiary-container: '#c8d1da'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d7e2ff'
  primary-fixed-dim: '#acc7ff'
  on-primary-fixed: '#001a40'
  on-primary-fixed-variant: '#004491'
  secondary-fixed: '#d9e3f1'
  secondary-fixed-dim: '#bdc7d5'
  on-secondary-fixed: '#131c26'
  on-secondary-fixed-variant: '#3e4853'
  tertiary-fixed: '#dbe4ed'
  tertiary-fixed-dim: '#bfc8d0'
  on-tertiary-fixed: '#141d23'
  on-tertiary-fixed-variant: '#3f484f'
  background: '#f8f9fa'
  on-background: '#191c1d'
  surface-variant: '#e1e3e4'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  title-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
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
  label-bold:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
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
  sidebar_width: 240px
  header_height: 64px
  container_max_width: 1280px
---

## Brand & Style
The design system is rooted in the principles of **Modern Corporate** and **Minimalist** aesthetics, specifically tailored for the high-stakes environment of a clinical analysis laboratory. The visual narrative centers on "Precision, Trust, and Hygiene." 

The brand personality is authoritative yet accessible, using a "sterile white" foundation to evoke cleanliness and professional rigor. By eliminating unnecessary decorative elements, the system ensures that medical data remains the primary focus. The emotional response should be one of calm reliability—reassuring both lab technicians and patients that their data is handled with meticulous care and systematic accuracy.

## Colors
This design system utilizes a high-clarity palette to differentiate functional zones and status types. 

- **Primary Blue (#0056b3):** Used for primary actions, navigation selection, and branding to establish a professional medical identity.
- **Secondary Light Blue (#e7f1ff):** Employed for subtle background fills in tables, active states in sidebars, and highlighting specific data rows without overwhelming the eye.
- **Sterile Backgrounds:** The main canvas is pure white (#ffffff), while off-white neutrals (#f8f9fa) are used to separate the sidebar and header from the main workspace.
- **Semantic States:** Success (Green) and Error (Red) are used exclusively for status indicators, validation messages, and critical alerts to ensure instant cognitive recognition of test result status.

## Typography
**Inter** is selected for its exceptional legibility in data-dense interfaces. Its tall x-height and clear letterforms prevent fatigue during long shifts of data entry and analysis.

For technical data or reference numbers, a secondary monospaced font (JetBrains Mono) may be used within table cells to ensure character alignment. Use `label-bold` for table headers and form labels to provide a clear structural hierarchy. Mobile typography scales down display sizes by 20% to maintain screen real estate while preserving legibility.

## Layout & Spacing
The system follows a **Fixed-Fluid Hybrid** model. The sidebar remains fixed at 240px to provide a consistent anchor for navigation, while the main content area utilizes a 12-column fluid grid that adapts to the browser width.

A strict 4px baseline grid ensures vertical rhythm. Tables use a "Compact" density (8px vertical padding) to maximize the amount of information visible on screen without sacrificing scanability. Margins of 24px (lg) are maintained between major logical sections (e.g., Personal Information vs. Clinical Analysis) as seen in the patient registration sketches.

## Elevation & Depth
In line with the clinical theme, depth is primarily conveyed through **Tonal Layers** and **Low-contrast Outlines** rather than heavy shadows.

- **Level 0 (Base):** The main background #ffffff.
- **Level 1 (Surface):** Neutral #f8f9fa used for the sidebar and header to create a structural frame.
- **Level 2 (Interactive):** Form inputs and table rows use a 1px border (#dee2e6). On hover, borders transition to the Primary Blue.
- **Overlays:** Only modals and dropdowns utilize a subtle, highly-diffused shadow (0px 4px 12px rgba(0,0,0,0.05)) to separate them from the work surface without appearing "heavy."

## Shapes
The system uses a **Soft** shape language (4px radius). This slight rounding softens the "clinical" edge just enough to feel modern and user-friendly while maintaining the geometric precision required for a professional tool.

- **Small (4px):** Buttons, input fields, and checkboxes.
- **Large (8px):** Main content containers and cards.
- **Full (Pill):** Used exclusively for status chips (e.g., "Pending", "Completed") to distinguish them from interactive buttons.

## Components

### Navigation Sidebar
A vertical persistent bar on the left. Active items use a Primary Blue left-accent bar (4px width) and a Secondary Blue background tint. Icons should be stroke-based and 20px in size.

### Tables & Data
Table headers use `label-bold` with a light gray background. Rows must alternate colors (Zebra striping) or use a clear 1px bottom border. Status indicators are displayed as "Chips" with high-contrast text against a light-tinted version of the semantic color (e.g., Light Green background with Dark Green text).

### Form Inputs
Inputs are stacked vertically with labels positioned above. Focus states are marked by a 2px Primary Blue border. Error states utilize a Red border and include a small icon and helper text below the field.

### Buttons
- **Primary:** Solid Primary Blue with white text.
- **Secondary:** Transparent with Primary Blue border and text.
- **Action/Ghost:** Used for table actions (Edit, Delete) to reduce visual noise; these only appear fully opaque on row hover.

### Progress Indicators
For long-running laboratory reports, use a linear progress bar at the top of the table or section, utilizing the Primary Blue color.