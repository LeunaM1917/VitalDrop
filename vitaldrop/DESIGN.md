---
name: VitalDrop
colors:
  surface: '#fff8f7'
  surface-dim: '#f1d3d0'
  surface-bright: '#fff8f7'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#fff0ef'
  surface-container: '#ffe9e7'
  surface-container-high: '#ffe2de'
  surface-container-highest: '#f9dcd9'
  on-surface: '#271816'
  on-surface-variant: '#5b403d'
  inverse-surface: '#3e2c2a'
  inverse-on-surface: '#ffedeb'
  outline: '#8f6f6c'
  outline-variant: '#e4beba'
  surface-tint: '#ba1a20'
  primary: '#af101a'
  on-primary: '#ffffff'
  primary-container: '#d32f2f'
  on-primary-container: '#fff2f0'
  inverse-primary: '#ffb3ac'
  secondary: '#29695b'
  on-secondary: '#ffffff'
  secondary-container: '#acedda'
  on-secondary-container: '#2e6d5f'
  tertiary: '#005f7b'
  on-tertiary: '#ffffff'
  tertiary-container: '#00799c'
  on-tertiary-container: '#e9f7ff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdad6'
  primary-fixed-dim: '#ffb3ac'
  on-primary-fixed: '#410003'
  on-primary-fixed-variant: '#930010'
  secondary-fixed: '#afefdd'
  secondary-fixed-dim: '#94d3c1'
  on-secondary-fixed: '#00201a'
  on-secondary-fixed-variant: '#065043'
  tertiary-fixed: '#bee9ff'
  tertiary-fixed-dim: '#7bd1f8'
  on-tertiary-fixed: '#001f2a'
  on-tertiary-fixed-variant: '#004d65'
  background: '#fff8f7'
  on-background: '#271816'
  surface-variant: '#f9dcd9'
typography:
  h1:
    fontFamily: manrope
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  h2:
    fontFamily: manrope
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.3'
    letterSpacing: -0.01em
  h3:
    fontFamily: manrope
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: '0'
  body-lg:
    fontFamily: inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  body-md:
    fontFamily: inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: '0'
  label-caps:
    fontFamily: inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  container-max: 1200px
  gutter: 24px
---

## Brand & Style

The design system is centered on the intersection of biological urgency and technological precision. It evokes a sense of calm authority, clinical reliability, and immediate action. The target audience includes individual donors seeking a frictionless experience and healthcare professionals requiring data accuracy.

The visual style is **Corporate / Modern** with a focus on high-contrast accessibility. It prioritizes clarity and functional efficiency, utilizing significant whitespace to reduce cognitive load during the donation process. The aesthetic is "MedTech"—blending the sterility of healthcare with the sleekness of modern software through crisp edges, deliberate color application, and a focus on data visualization.

## Colors

The palette is anchored by "Life Crimson" (#D32F2F), used strategically for primary actions and urgency-related notifications. This is balanced by "Trust Teal" (#004D40), which provides a stable, tech-forward foundation for navigation and secondary branding. 

Backgrounds utilize an off-white tint (#FAFAFA) to prevent screen glare and eye strain, while body text is set in Charcoal (#333333) to ensure a high WCAG-compliant contrast ratio. Use the secondary teal for data-heavy sections to distinguish "system" information from "human" actions (red).

## Typography

The design system employs a dual-font strategy. **Manrope** is used for headings to provide a refined, modern geometric feel that suggests intelligence and innovation. **Inter** is used for all body and UI text for its exceptional legibility in data-dense environments.

To maintain readability in long-form content, such as donation guidelines or health articles, the line length is strictly capped at approximately 65 characters (~650px). Type hierarchy is enforced through substantial size stepping and weight changes to ensure users can scan critical health data quickly.

## Layout & Spacing

This design system utilizes a **Fixed Grid** model for desktop experiences to maintain the 65ch readability standard, transitioning to a fluid model for mobile devices. The layout is structured on a 12-column grid with 24px gutters.

The spacing rhythm follows an 8px linear scale. Large vertical gaps (48px+) should be used to separate distinct stages of the user journey, such as "Eligibility Check" and "Appointment Scheduling." All internal component padding must align with the 8px base unit to maintain visual rigor.

## Elevation & Depth

To maintain a clean, professional healthcare aesthetic, the design system avoids heavy shadows. Depth is primarily conveyed through **Tonal Layers** and **Low-contrast Outlines**.

1.  **Level 0 (Base):** Off-white background (#FAFAFA).
2.  **Level 1 (Cards/Surface):** Pure White (#FFFFFF) with a 1px solid border (#ECEFF1).
3.  **Level 2 (Interactive):** Surfaces gain a very subtle, diffused ambient shadow (0px 4px 12px rgba(0,0,0,0.05)) only when being hovered or dragged.

This flat-first approach ensures the UI feels lightweight and fast, mimicking a high-end medical dashboard.

## Shapes

The shape language is **Rounded**, using a 0.5rem (8px) base radius. This softens the clinical nature of the platform, making it feel more approachable and "human." Large components like hero sections or dashboard containers use `rounded-xl` (1.5rem/24px) to create a modern, contained look. Small interactive elements like checkboxes or utility tags should maintain the base 8px radius to ensure a cohesive visual identity.

## Components

### Buttons
- **Primary:** Life Crimson background, White text. High-contrast, no gradient.
- **Secondary:** Trust Teal border (2px) and text, transparent background.
- **Tertiary:** Charcoal text, no background, for low-priority actions like "Cancel."

### Input Fields
Inputs should use Level 1 surfaces with a 1px #CFD8DC border. On focus, the border transitions to a 2px Trust Teal stroke. Error states must use Life Crimson for both the border and the helper text.

### Cards & Lists
Cards are the primary container for donor stats (e.g., "Last Donation"). They utilize White backgrounds and the 8px base radius. Lists for donation history should use alternating tonal rows (Level 0 and Level 1) for better scannability.

### Chips & Status Indicators
Status markers (e.g., "Eligible," "Urgent Need") use high-saturation background tints with dark text. For example, "Urgent" uses a light red tint with Crimson text to signal importance without overwhelming the layout.

### Specialized Components
- **The "Droplet" Progress Bar:** A custom progress indicator for blood supply levels using the droplet motif.
- **Appointment Timeline:** A vertical stepper with Teal connector lines to guide donors through the preparation, donation, and recovery phases.