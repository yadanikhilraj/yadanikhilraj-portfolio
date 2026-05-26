---
name: Obsidian Prism
colors:
  surface: '#12131a'
  surface-dim: '#12131a'
  surface-bright: '#383940'
  surface-container-lowest: '#0c0e14'
  surface-container-low: '#1a1b22'
  surface-container: '#1e1f26'
  surface-container-high: '#282a31'
  surface-container-highest: '#33343c'
  on-surface: '#e2e1eb'
  on-surface-variant: '#c2c6d6'
  inverse-surface: '#e2e1eb'
  inverse-on-surface: '#2f3037'
  outline: '#8c909f'
  outline-variant: '#424754'
  surface-tint: '#adc6ff'
  primary: '#adc6ff'
  on-primary: '#002e6a'
  primary-container: '#4d8eff'
  on-primary-container: '#00285d'
  inverse-primary: '#005ac2'
  secondary: '#d0bcff'
  on-secondary: '#3c0091'
  secondary-container: '#571bc1'
  on-secondary-container: '#c4abff'
  tertiary: '#c8c6c7'
  on-tertiary: '#313031'
  tertiary-container: '#929091'
  on-tertiary-container: '#2a292b'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#adc6ff'
  on-primary-fixed: '#001a42'
  on-primary-fixed-variant: '#004395'
  secondary-fixed: '#e9ddff'
  secondary-fixed-dim: '#d0bcff'
  on-secondary-fixed: '#23005c'
  on-secondary-fixed-variant: '#5516be'
  tertiary-fixed: '#e5e2e3'
  tertiary-fixed-dim: '#c8c6c7'
  on-tertiary-fixed: '#1c1b1c'
  on-tertiary-fixed-variant: '#474647'
  background: '#12131a'
  on-background: '#e2e1eb'
  surface-variant: '#33343c'
typography:
  display-lg:
    fontFamily: Geist
    fontSize: 64px
    fontWeight: '700'
    lineHeight: 72px
    letterSpacing: -0.04em
  display-lg-mobile:
    fontFamily: Geist
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
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
  label-md:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.02em
  code:
    fontFamily: jetbrainsMono
    fontSize: 14px
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
  unit: 4px
  container-max: 1200px
  gutter: 24px
  margin-mobile: 20px
  section-gap: 120px
---

## Brand & Style

The design system is engineered for high-performance developer portfolios, evoking a sense of technical mastery and enterprise-grade reliability. The brand personality is "Sophisticated Futurist"—combining the precision of high-end developer tools with the aesthetic polish of modern SaaS leaders.

The visual style utilizes a refined **Glassmorphism** approach set against a deep, monochromatic void. This is not a "noisy" interface; it is a "focused" one. We prioritize legibility and performance, using translucent layers and vibrant gradients only to highlight key focal points and calls to action. The emotional response should be one of calm confidence, precision, and technical depth.

## Colors

The palette is anchored in a dark-mode-first philosophy. The background is a "True Charcoal" (#0A0A0B) to ensure maximum contrast for text and vibrant accents.

- **Primary & Secondary:** A high-vibrancy duo of Neon Blue and Vibrant Purple. These are used primarily for interactive states, progress indicators, and decorative gradients.
- **Surface Colors:** Derived from the primary neutral, utilizing low-opacity whites (e.g., `rgba(255, 255, 255, 0.03)`) to create the glass effect.
- **Accents:** Use gradients sparingly. A linear gradient from `primary` to `secondary` at 135 degrees is the standard for high-impact elements like primary buttons or hero headings.

## Typography

This design system leverages **Geist** for its technical, precise character in headings and UI labels, paired with **Inter** for optimized body readability. 

- **Display Text:** Should use tight letter spacing and heavy weights to command attention.
- **Contrast:** Maintain high contrast between headings (White/Near-White) and body text (Neutral Gray) to establish clear hierarchy.
- **Monospace:** Use **JetBrains Mono** exclusively for code snippets, terminal outputs, or technical metadata to reinforce the developer-centric theme.

## Layout & Spacing

The layout follows a **Fixed Grid** model for desktop to maintain the "professional tool" feel, while transitioning to a fluid model for mobile.

- **Grid System:** Use a 12-column grid for desktop (1200px max-width) with 24px gutters.
- **Spacing Rhythm:** Based on a 4px scale. Components should primarily use 16px (4 units) or 24px (6 units) for internal padding.
- **Sectioning:** Large vertical gaps (120px+) are encouraged between major sections to allow the glassmorphic elements "room to breathe" and to emphasize the minimalist aesthetic.
- **Background Patterns:** Implement a subtle 32px square grid pattern using a 1px stroke of `rgba(255, 255, 255, 0.03)` to add technical texture to the background.

## Elevation & Depth

Depth is achieved through **Glassmorphism** and light-based hierarchy rather than traditional shadows.

- **Surface Layers:** The primary container layer uses a background of `rgba(255, 255, 255, 0.03)` with a `backdrop-filter: blur(12px)`.
- **Borders:** Surfaces must have a 1px solid border. Use a top-down light source logic: the top and left borders are slightly brighter (`rgba(255, 255, 255, 0.1)`) than the bottom and right.
- **Glowing States:** Interactive elements or featured cards should utilize a subtle outer glow (box-shadow) that matches the primary or secondary accent color, with a high blur radius (32px+) and low opacity (0.15).

## Shapes

The shape language is "Soft-Technical." We avoid fully organic circles in favor of controlled, geometric radii that suggest precision.

- **Base Radius:** 0.25rem (4px) for small UI elements like checkboxes and tags.
- **Component Radius:** 0.5rem (8px) for buttons and input fields.
- **Container Radius:** 0.75rem (12px) for cards and modals.
- **Consistency:** All glass layers must share the same corner radius as their background masks to maintain the "milled glass" appearance.

## Components

### Buttons
- **Primary:** Gradient background (Blue to Purple), white text, 8px radius. On hover, increase the glow intensity.
- **Secondary:** Glass background, 1px white border (0.1 opacity), Geist SemiBold text.
- **Tertiary/Ghost:** No background, primary color text, subtle underline on hover.

### Glassy Cards
Cards are the core layout building block. They feature a `0.03` white opacity fill, a `12px` backdrop blur, and a `1px` border. For "featured" cards, apply a 2px gradient border.

### Input Fields
Dark backgrounds (#000000), 1px border, and Geist-font labels. Focus state should trigger a primary-color glow and border.

### Chips & Tags
Small, 4px radius, using a subtle primary color tint (e.g., `rgba(59, 130, 246, 0.1)`) with primary color text. Used for "Tech Stack" or "Language" labels.

### Code Blocks
Custom-styled containers with a darker-than-background fill (#050505), JetBrains Mono text, and a header bar showing a simulated "file name" and copy button.

### Animated Borders
For top-tier sections (e.g., "Hire Me" or "Featured Project"), use a continuous gradient border animation that slowly rotates around the card perimeter.