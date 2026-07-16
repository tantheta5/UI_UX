---
name: Blueprint UX
colors:
  surface: '#f9f9fa'
  surface-dim: '#dadadb'
  surface-bright: '#f9f9fa'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f4'
  surface-container: '#eeeeef'
  surface-container-high: '#e8e8e9'
  surface-container-highest: '#e2e2e3'
  on-surface: '#1a1c1d'
  on-surface-variant: '#4c4546'
  inverse-surface: '#2f3132'
  inverse-on-surface: '#f0f1f2'
  outline: '#7e7576'
  outline-variant: '#cfc4c5'
  surface-tint: '#5e5e5e'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#1b1b1b'
  on-primary-container: '#848484'
  inverse-primary: '#c6c6c6'
  secondary: '#5d5e66'
  on-secondary: '#ffffff'
  secondary-container: '#e3e1ec'
  on-secondary-container: '#63646c'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#1b1b1b'
  on-tertiary-container: '#848484'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e2e2e2'
  primary-fixed-dim: '#c6c6c6'
  on-primary-fixed: '#1b1b1b'
  on-primary-fixed-variant: '#474747'
  secondary-fixed: '#e3e1ec'
  secondary-fixed-dim: '#c6c5cf'
  on-secondary-fixed: '#1a1b22'
  on-secondary-fixed-variant: '#46464e'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c6'
  on-tertiary-fixed: '#1b1b1b'
  on-tertiary-fixed-variant: '#474747'
  background: '#f9f9fa'
  on-background: '#1a1c1d'
  surface-variant: '#e2e2e3'
typography:
  headline-xl:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-xl-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
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
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '500'
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
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  2xl: 48px
  3xl: 64px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 32px
---

## Brand & Style
The design system is a functional, medium-fidelity framework designed for structural clarity and user-flow validation. The objective is to eliminate visual noise—such as brand colors, decorative shadows, or complex gradients—to focus entirely on information architecture, hierarchy, and interaction logic.

The aesthetic follows a **Functional Minimalist** approach. It utilizes a strict grayscale palette and systematic spacing to create a professional environment suitable for high-level UX reviews and stakeholder alignment. The emotional response should be one of clarity, neutrality, and precision.

## Colors
The palette is strictly achromatic. By using only shades of black, white, and gray, the design system ensures that all emphasis remains on the content structure and functional affordances.

- **Primary:** Black (#000000) for primary actions, heavy text, and essential icons.
- **Secondary:** Mid-gray (#71717A) for secondary information, borders, and disabled states.
- **Surface/Neutral:** A range of light grays (#F4F4F5, #E4E4E7) to define container boundaries and background differentiation.
- **Background:** Pure White (#FFFFFF) for the primary workspace to maintain maximum contrast.

## Typography
This design system uses **Inter** for all roles. Inter is chosen for its systematic, utilitarian nature and exceptional legibility at small sizes. 

Hierarchy is established through weight and scale rather than color. Headlines use tighter tracking and heavier weights to anchor sections, while body text maintains generous line heights to ensure readability in data-heavy wireframes. For mobile views, large headlines scale down to prevent excessive wrapping.

## Layout & Spacing
The layout relies on a **strict 8px grid system** to ensure consistency across all components and views. 

- **Grid:** 12-column fluid grid for desktop; 4-column fluid grid for mobile.
- **Touch Targets:** All interactive elements maintain a minimum hit area of 44x44px.
- **Margins:** 16px safe areas for mobile devices; 32px or centered max-width (1200px) for desktop.
- **Rhythm:** Vertical rhythm is controlled via 8px increments. Components use `md` (16px) for internal padding and `lg` (24px) for section separation.

## Elevation & Depth
In the absence of shadows, depth is communicated through **Tonal Layers** and **Low-Contrast Outlines**.

- **Level 0 (Background):** White (#FFFFFF).
- **Level 1 (Cards/Containers):** Defined by a 1px solid border (#E4E4E7). No shadow.
- **Level 2 (Modals/Overlays):** Defined by a slightly thicker 2px border or a light gray background fill (#F4F4F5) to distinguish from the base layer.
- **Scrim:** A 40% opacity black overlay is used behind modals and bottom sheets to focus user attention and indicate modal behavior.

## Shapes
The design system uses a "Soft" corner radius. This provides a professional, modern feel that is less clinical than sharp corners but more formal than pill shapes.

- **Standard (4px):** Used for buttons, input fields, and checkboxes.
- **Large (8px):** Used for cards, modals, and larger container elements.
- **Extra Large (12px):** Reserved for bottom sheets and top-level containers.
- **Full (999px):** Used exclusively for avatars and progress bar caps.

## Components

### Buttons
- **Primary:** Solid Black fill with White text.
- **Secondary:** White fill with 1px Black border.
- **Ghost:** No fill or border; Black text. Used for less prominent actions or navigation.

### Input Fields
- **Text Fields:** 1px gray border (#D4D4D8). Focused state increases border to 2px Black. Labels sit above the field in `label-sm`.
- **Checkboxes/Radios:** 2px gray border. Selected state is solid Black.

### Cards & Lists
- **Cards:** 1px border (#E4E4E7) with 16px internal padding. 
- **Lists:** Separated by 1px horizontal dividers (#F4F4F5). 12px vertical padding for list items to ensure touch-friendly targets.

### Modals & Bottom Sheets
- **Modals:** Centered on desktop, 8px corner radius, centered header with a "Close" icon.
- **Bottom Sheets:** Mobile-only, slides from the bottom with a 12px top-corner radius and a horizontal drag handle indicator.

### Progress & Feedback
- **Progress Bars:** 8px height, light gray track with a solid Black indicator.
- **Avatars:** Circular frames with a light gray fill (#E4E4E7) and a centered user icon or initials.
- **Chips:** Small, 4px rounded containers with light gray fill, used for status or filtering.