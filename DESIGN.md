---
name: Azure Architect Dark
colors:
  surface: '#0e1418'
  surface-dim: '#0e1418'
  surface-bright: '#343a3e'
  surface-container-lowest: '#090f13'
  surface-container-low: '#161c20'
  surface-container: '#1a2025'
  surface-container-high: '#252b2f'
  surface-container-highest: '#2f363a'
  on-surface: '#dde3e9'
  on-surface-variant: '#c0c7d4'
  inverse-surface: '#dde3e9'
  inverse-on-surface: '#2b3136'
  outline: '#8d919a'
  outline-variant: '#42474f'
  surface-tint: '#a3c9ff'
  primary: '#d3e4ff'
  on-primary: '#00315c'
  primary-container: '#0078d4'
  on-primary-container: '#2c5483'
  inverse-primary: '#396090'
  secondary: '#c2c7d0'
  on-secondary: '#2b3138'
  secondary-container: '#42474f'
  on-secondary-container: '#b0b5be'
  tertiary: '#dee3ec'
  on-tertiary: '#2c3138'
  tertiary-container: '#c2c7d0'
  on-tertiary-container: '#4e535a'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d3e3ff'
  primary-fixed-dim: '#a3c9ff'
  on-primary-fixed: '#001c38'
  on-primary-fixed-variant: '#1e4876'
  secondary-fixed: '#dee3ec'
  secondary-fixed-dim: '#c2c7d0'
  on-secondary-fixed: '#171c23'
  on-secondary-fixed-variant: '#42474f'
  tertiary-fixed: '#dee3ec'
  tertiary-fixed-dim: '#c2c7cf'
  on-tertiary-fixed: '#171c22'
  on-tertiary-fixed-variant: '#42474e'
  background: '#0e1418'
  on-background: '#dde3e9'
  surface-variant: '#2f363a'
  linkedin-blue: '#0077b5'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-sm:
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
  label-md:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.02em
  code-sm:
    fontFamily: Geist
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  xs: 4px
  base: 8px
  sm: 12px
  md: 24px
  lg: 48px
  xl: 80px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
---

## Brand & Style
The brand identity is built for a senior infrastructure engineer, focusing on reliability, precision, and a high-tech "Operations Center" aesthetic. 

The design style is a sophisticated mix of **Glassmorphism** and **Technical Minimalism**. It utilizes deep obsidian surfaces, semi-transparent frosted layers, and precise geometric grid patterns to evoke the feeling of a terminal or a high-end cloud dashboard. The visual language conveys competence in the Microsoft ecosystem through a "system-active" atmosphere, utilizing glowing status indicators and high-quality typography.

## Colors
The palette is a high-fidelity dark mode optimized for reduced eye strain and professional clarity.

- **Primary**: A bright, electric "Azure Blue" used for highlights, calls to action, and active status indicators.
- **Surface**: A deep navy-charcoal base that provides high contrast for white and light-blue text.
- **Glass Accents**: Semi-transparent versions of the surface color are used for cards to allow background patterns to peek through.
- **Action Colors**: A specific high-contrast blue is reserved for LinkedIn integration to maintain brand recognition.

## Typography
The typography system uses a dual-font approach to balance readability with a technical feel.

- **Headlines & Body**: **Inter** is the primary workhorse, providing a neutral and utilitarian foundation that scales perfectly from small body text to massive hero headers.
- **Labels & UI Elements**: **Geist** (specifically Geist Mono where applicable) is used for technical labels, buttons, and navigation. This adds a "developer-centric" flavor to the interface, signaling precision and expertise in code-adjacent environments.

## Layout & Spacing
The layout follows a **Fixed Grid** philosophy for content, centered within a max-width of 1200px to maintain readability on ultra-wide monitors.

- **Grid**: A standard 12-column system is used on desktop, collapsing to a single column on mobile.
- **Vertical Rhythm**: Large vertical padding (`xl`) separates major sections, while `md` (24px) is the standard gap between internal card elements.
- **Technical Grid**: A background pattern of 40px x 40px lines is used to reinforce the "infrastructure/architect" theme.

## Elevation & Depth
Depth is achieved through **Glassmorphism** rather than traditional drop shadows.

- **Surface Tiers**: Base background is solid. Secondary containers use semi-transparent fills with 20px backdrop blurs.
- **Borders**: Depth is defined by subtle 1px white borders at 10% opacity, which act as "inner glows" on dark surfaces.
- **Interactive State**: Hovering over cards increases the border opacity and introduces a primary-colored glow (`0 0 20px rgba(0, 120, 212, 0.15)`) rather than a shadow, simulating an illuminated display.

## Shapes
The shape language is modern and approachable but retains structure. 

- **Standard Containers**: Use a base radius of 0.75rem (`rounded-xl`) for main cards and content blocks.
- **Pill Shapes**: Used for small status chips, badges, and top-level callouts to provide a friendlier contrast to the rigid technical grid.
- **Interactive Elements**: Buttons use a slightly more conservative 0.5rem (`rounded-lg`) to feel more "industrial" and button-like.

## Components
- **Buttons**:
    - **Primary**: Solid background using `primary-container`, white text, and a strong glow on hover.
    - **Secondary**: Outlined with primary color, with a subtle color fill on hover.
- **Glass Cards**: The signature component. Semi-transparent background, 20px blur, and an interactive border that reacts to pointer proximity.
- **Status Chips**: Pill-shaped containers with a pulsing 8px dot (animation: `pulse`) to indicate "live" system status.
- **Timeline**: A vertical line with `primary/20` gradient, using technical icons (Material Symbols) inside circles to denote milestones.
- **Inputs & Reveal Buttons**: Large, clickable areas that transform upon interaction (e.g., clicking to reveal email), providing tactile feedback through scale transforms (`active:scale-95`).