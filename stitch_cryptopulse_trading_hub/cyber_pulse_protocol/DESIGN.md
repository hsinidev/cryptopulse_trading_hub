---
name: Cyber-Pulse Protocol
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#baccb0'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#85967c'
  outline-variant: '#3c4b35'
  surface-tint: '#2ae500'
  primary: '#efffe3'
  on-primary: '#053900'
  primary-container: '#39ff14'
  on-primary-container: '#107100'
  inverse-primary: '#106e00'
  secondary: '#c8c6c5'
  on-secondary: '#303030'
  secondary-container: '#474747'
  on-secondary-container: '#b6b5b4'
  tertiary: '#fff8f7'
  on-tertiary: '#690006'
  tertiary-container: '#ffd3ce'
  on-tertiary-container: '#c50015'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#79ff5b'
  primary-fixed-dim: '#2ae500'
  on-primary-fixed: '#022100'
  on-primary-fixed-variant: '#095300'
  secondary-fixed: '#e4e2e1'
  secondary-fixed-dim: '#c8c6c5'
  on-secondary-fixed: '#1b1c1c'
  on-secondary-fixed-variant: '#474747'
  tertiary-fixed: '#ffdad6'
  tertiary-fixed-dim: '#ffb4ab'
  on-tertiary-fixed: '#410002'
  on-tertiary-fixed-variant: '#93000c'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-lg:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  data-mono:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '500'
    lineHeight: '1.4'
    letterSpacing: 0.05em
  body-reg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: '0'
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.1em
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  container-margin: 16px
  gutter: 12px
---

## Brand & Style

The design system is engineered for high-frequency crypto trading, evoking a sense of precision, speed, and technical sovereignty. The brand personality is "Elite Technical," catering to users who view trading as a high-stakes, data-driven operation. 

The visual style merges **Minimalism** with **Cyber-Tech** elements. It utilizes a deep, matte foundation to minimize eye strain during extended sessions while employing high-intensity neon accents to signal critical system states. The aesthetic incorporates subtle **Glassmorphism** for layered data overlays and **High-Contrast** interactive zones to ensure zero-latency cognitive processing of market movements.

## Colors

This design system utilizes a strict dark-mode-only palette to maintain high contrast and "glowing" visual hierarchy. 

- **Matte Black (#0D0D0D):** The absolute foundation. All background surfaces use this to eliminate light bleed.
- **Neon Green (#39FF14):** Reserved for primary branding, successful trade executions, and positive price action ("Bullish"). It carries a 0 0 8px glow effect in high-priority states.
- **Alert Red (#FF3131):** Used exclusively for sell actions, negative price action ("Bearish"), and critical system errors.
- **Graphite (#2C2C2C):** Used for secondary containers, input backgrounds, and dividers to provide subtle structural depth without breaking the dark aesthetic.

## Typography

The typography strategy prioritizes legibility of numerical data and a "technical" atmosphere. 

- **Space Grotesk** is used for headings and branding elements to provide a futuristic, geometric edge. 
- **Inter** is the workhorse for body copy and UI labels, chosen for its exceptional clarity on small mobile screens. 
- All price data and ticker symbols should utilize a tabular-nums configuration to prevent horizontal "jitter" during rapid price updates.
- **Label-caps** are used for secondary data metadata (e.g., "24H VOL", "MARKET CAP") to create a clear visual distinction from live price data.

## Layout & Spacing

The design system employs a **Fluid Grid** optimized for mobile-first trading. 

- **Grid:** A 4-column grid for mobile, expanding to a 12-column grid for desktop views.
- **Rhythm:** A strict 4px baseline grid ensures all elements align to technical increments.
- **Safe Areas:** On mobile, a 16px horizontal margin is mandatory. 
- **Density:** High density is preferred for data tables (order books, recent trades), while interaction zones (trade execution buttons) require larger hit targets of at least 56px height.

## Elevation & Depth

In a pure matte black environment, depth is achieved through **Tonal Layering** and **Glassmorphism** rather than traditional shadows.

1.  **Level 0 (Floor):** Matte Black (#0D0D0D) for the main application background.
2.  **Level 1 (Cards/Containers):** Graphite (#2C2C2C) with a subtle 1px border (#333333).
3.  **Level 2 (Overlays/Modals):** Glassmorphic surfaces with a 15% opacity white tint and a 20px backdrop blur.
4.  **Accents:** Interactive elements use "Neon Glows"—a drop shadow with 0 spread and 10px blur using the primary neon green or alert red color to indicate active states or focus.

## Shapes

The shape language of this design system is **Sharp (0)**. 

To reinforce the high-performance, "technical instrument" aesthetic, all corners are kept at 0px radius. This creates a precision-milled look and maximizes screen real estate for data. In rare cases where a container needs to be differentiated (such as a primary action button), a 45-degree "clipped corner" (chamfer) can be used on the top-right corner to suggest a tactical, military-grade interface.

## Components

- **Trade Buttons:** Massive, full-width blocks at the bottom of the viewport. "BUY" uses Neon Green with black text; "SELL" uses Alert Red with white text. 
- **Inputs:** Dark Graphite background with a Sharp (0px) 1px border that turns Neon Green on focus. Labels sit inside the top border in a small, uppercase mono font.
- **Chips/Status:** Outline-only indicators using 1px stroke of the status color (Green/Red/Grey). No fills.
- **Data Visualization:** Line charts should be 1.5px stroke width. Bullish trends use a Neon Green gradient fill with 10% opacity; Bearish trends use Alert Red.
- **The "Pulse" Indicator:** A small, 8px glowing dot in the header that pulses with Neon Green whenever a WebSocket connection is receiving live price updates.
- **Segmented Controls:** Rectangular blocks with no gap between segments, using Graphite for inactive and Neon Green for active states.