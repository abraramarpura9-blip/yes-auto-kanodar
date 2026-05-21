---
name: High-Performance Luxury
colors:
  surface: '#121414'
  surface-dim: '#121414'
  surface-bright: '#37393a'
  surface-container-lowest: '#0c0f0f'
  surface-container-low: '#1a1c1c'
  surface-container: '#1e2020'
  surface-container-high: '#282a2b'
  surface-container-highest: '#333535'
  on-surface: '#e2e2e2'
  on-surface-variant: '#c4c7c7'
  inverse-surface: '#e2e2e2'
  inverse-on-surface: '#2f3131'
  outline: '#8e9192'
  outline-variant: '#444748'
  surface-tint: '#c9c6c5'
  primary: '#c9c6c5'
  on-primary: '#313030'
  primary-container: '#0a0a0a'
  on-primary-container: '#7b7979'
  inverse-primary: '#5f5e5e'
  secondary: '#ffb3b1'
  on-secondary: '#680011'
  secondary-container: '#d6042f'
  on-secondary-container: '#ffe7e5'
  tertiary: '#c6c6c6'
  on-tertiary: '#2f3131'
  tertiary-container: '#090a0b'
  on-tertiary-container: '#79797a'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e5e2e1'
  primary-fixed-dim: '#c9c6c5'
  on-primary-fixed: '#1c1b1b'
  on-primary-fixed-variant: '#474646'
  secondary-fixed: '#ffdad8'
  secondary-fixed-dim: '#ffb3b1'
  on-secondary-fixed: '#410007'
  on-secondary-fixed-variant: '#92001d'
  tertiary-fixed: '#e3e2e2'
  tertiary-fixed-dim: '#c6c6c6'
  on-tertiary-fixed: '#1a1c1c'
  on-tertiary-fixed-variant: '#464747'
  background: '#121414'
  on-background: '#e2e2e2'
  surface-variant: '#333535'
typography:
  display-lg:
    fontFamily: Montserrat
    fontSize: 64px
    fontWeight: '800'
    lineHeight: 72px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Montserrat
    fontSize: 40px
    fontWeight: '800'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Montserrat
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-md:
    fontFamily: Montserrat
    fontSize: 24px
    fontWeight: '700'
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
  label-bold:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 8px
  gutter: 24px
  margin-desktop: 64px
  margin-mobile: 20px
  container-max-width: 1440px
---

## Brand & Style
The design system is engineered to evoke the atmosphere of an elite, high-end automotive showroom. It prioritizes precision, speed, and uncompromising quality. The aesthetic is rooted in **Minimalism** with a **High-Contrast** edge, utilizing deep blacks and sharp accents to place the vehicles—the "hero" products—at the center of the experience.

Every interaction should feel mechanical and deliberate. The emotional response is one of security and prestige, reinforcing the "Driven By Trust" narrative through crystalline clarity and a disciplined visual hierarchy.

## Colors
The palette is dominated by **Deep Black (#0A0A0A)**, serving as a sophisticated canvas that absorbs light and allows vehicle photography to pop. **Performance Red (#E31837)** is used sparingly for critical actions and high-tension indicators, mimicking the adrenaline of a tachometer needle. 

**Metallic Silver (#C0C0C0)** is utilized for secondary information and hairline borders, providing a machined, industrial finish. **Pure White (#FFFFFF)** is reserved for high-readability typography and primary interface controls. Subtle linear gradients (from #1A1A1A to #0A0A0A) may be used to define surface depth without breaking the minimalist aesthetic.

## Typography
Typography follows a high-contrast logic. **Montserrat** provides a geometric, authoritative voice for headlines, echoing the bold branding seen in high-performance automotive marketing. All headlines should utilize tight letter-spacing to feel compact and "fast."

**Inter** is the functional workhorse for all technical data and body copy. It ensures that complex vehicle specifications remain legible even at small sizes. Labels and technical meta-data use an uppercase style with increased letter-spacing to create a "specification sheet" aesthetic.

## Layout & Spacing
The layout follows a **Fixed Grid** model on desktop to maintain the composed look of a luxury catalog. A 12-column system is used with generous 64px outer margins to create "breathable" whitespace, preventing the UI from feeling crowded.

Spacing is strictly mathematical, based on an 8px scale. Vehicle listings should utilize asymmetric layouts occasionally to create visual rhythm, while technical specs are aligned to a rigid, multi-column grid to emphasize precision engineering. On mobile, margins tighten to 20px, and content reflows into a single-column stack with priority given to high-resolution imagery.

## Elevation & Depth
Depth is achieved through **Tonal Layers** rather than traditional shadows. In this dark mode environment, higher elevation is signaled by lighter shades of grey (#161616 or #1A1A1A) rather than drop shadows. 

Where shadows are necessary for focus (e.g., modals), use a hard, high-opacity black shadow to maintain the "sharp" feel. Hairline outlines (1px) in Metallic Silver are used to define the boundaries of cards and input fields, creating a look reminiscent of machined metal parts. Backdrop blurs (Glassmorphism) are used exclusively for navigation bars to allow the vehicle photography to bleed through subtly as the user scrolls.

## Shapes
The shape language is "Soft-Precision" (Level 1). Elements use a consistent **4px (0.25rem)** corner radius. This is enough to prevent the UI from feeling aggressive or "brutalist," yet sharp enough to maintain a technical, engineered appearance. Large containers like vehicle hero cards may use up to 8px (0.5rem) to create a subtle distinction, but fully rounded or pill-shaped elements are strictly forbidden except for utility tags.

## Components

### Buttons
Primary buttons are solid Performance Red with white Montserrat Bold text. Secondary buttons use a Metallic Silver hairline border with no fill. Hover states should feature a subtle metallic glint effect (a diagonal linear gradient sweep).

### Vehicle Cards
Cards must prioritize the image aspect ratio (16:9). Specifications (KM, Fuel, Year) should be displayed in a horizontal grid at the bottom of the card using `label-bold` typography. Price is always highlighted in Performance Red.

### Premium Filters
Filters utilize a minimalist sidebar. Use custom-styled checkboxes that feature a sharp "tick" and a red border on active states. Sliders for price/year should be thin, silver lines with red circular handles.

### Inquiry Forms
Forms use "Ghost" style inputs: no background fill, only a bottom border of 1px Silver. On focus, the border turns Performance Red and the label floats upward. This minimizes visual clutter.

### Trust Badges
Badges should be monochromatic (Silver or White) to avoid competing with vehicle images. They feature thin-line iconography and small, precise `label-sm` text. They are often placed in the footer or directly below the primary "Book a Test Drive" action.