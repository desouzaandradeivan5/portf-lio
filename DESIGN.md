---
name: Neon System Portfolio
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
  on-surface-variant: '#bcc8d0'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#86939a'
  outline-variant: '#3c484f'
  surface-tint: '#68d3ff'
  primary: '#99deff'
  on-primary: '#003546'
  primary-container: '#00c8ff'
  on-primary-container: '#005068'
  inverse-primary: '#006684'
  secondary: '#cfbdff'
  on-secondary: '#3a0093'
  secondary-container: '#5e00e4'
  on-secondary-container: '#cbb8ff'
  tertiary: '#cad3ff'
  on-tertiary: '#1c2c64'
  tertiary-container: '#a7b6f6'
  on-tertiary-container: '#37467e'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#bee9ff'
  primary-fixed-dim: '#68d3ff'
  on-primary-fixed: '#001f2a'
  on-primary-fixed-variant: '#004d64'
  secondary-fixed: '#e9ddff'
  secondary-fixed-dim: '#cfbdff'
  on-secondary-fixed: '#22005d'
  on-secondary-fixed-variant: '#5400cc'
  tertiary-fixed: '#dce1ff'
  tertiary-fixed-dim: '#b7c4ff'
  on-tertiary-fixed: '#02164e'
  on-tertiary-fixed-variant: '#34437c'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: '700'
    lineHeight: '1.2'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.0'
    letterSpacing: 0.1em
  code:
    fontFamily: monospace
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max-width: 1200px
  gutter: 24px
  section-padding: 80px
  stack-sm: 12px
  stack-md: 24px
  stack-lg: 48px
---

## Brand & Style
The design system is engineered for a student of Systems Development, bridging the gap between academic rigor and cutting-edge technical innovation. The brand personality is **highly technical, professional, and forward-looking**, evoking the feeling of a sophisticated command center or a premium IDE.

The design style is a hybrid of **Glassmorphism** and **High-Contrast Dark Mode**. It utilizes deep obsidian surfaces layered with translucent panels to create a sense of architectural depth. This is complemented by "cyber-lume" accents—vibrant neon glows that guide the user's eye to interactive elements and key achievements.

## Colors
The palette is rooted in a deep-space black (`#090909`) to ensure maximum contrast for the neon accents. 

- **Primary (Electric Cyan):** Used for primary actions, focus states, and active status indicators. It represents the "energy" of the system.
- **Secondary (Vivid Violet):** Used for decorative gradients, secondary accents, and highlighting specialized skills.
- **Surface (Deep Navy):** A semi-transparent `#071A52` forms the base for glassmorphic cards and containers.
- **Gradients:** Linear transitions from Violet to Cyan should be used sparingly for "Hero" sections and high-impact call-to-actions.

## Typography
This design system utilizes **Inter** exclusively to maintain a clean, Swiss-inspired functional aesthetic that feels systematic and legible.

- **Display & Headlines:** Use tight letter-spacing and heavy weights to create a strong visual anchor.
- **Body Text:** Maintains a generous line height for readability against dark backgrounds. 
- **Labels:** Uppercase labels with increased letter-spacing are used for categorization (e.g., "PROJECT TYPE", "SKILL CATEGORY").
- **Monospaced Accents:** For snippets of code or technical metadata, use a standard system monospace font to reinforce the "Systems Development" identity.

## Layout & Spacing
The layout follows a **fluid grid system** that prioritizes white space (or "dark space") to prevent the UI from feeling cluttered.

- **The Grid:** A 12-column desktop grid that collapses to 1 column on mobile. 
- **Margins:** Desktop margins are set at 64px, scaling down to 24px on mobile devices.
- **Rhythm:** All spacing is based on an 8px base unit. Section vertical padding should be significant (`80px` to `120px`) to create the "Story" template feel of distinct, immersive chapters.

## Elevation & Depth
Depth is achieved through **optical layering** rather than traditional heavy shadows.

1.  **Base Layer:** The solid `#090909` background.
2.  **Glass Layer:** Surfaces use `#071A52` with an opacity of 40-60% and a `backdrop-filter: blur(12px)`.
3.  **Stroke Layer:** A subtle 1px border using a semi-transparent white (10%) or a faint primary-to-secondary gradient defines the edges of containers.
4.  **Glow Layer:** High-priority elements use `box-shadow` with a large blur radius (20px+) and low opacity, using the primary Cyan color to simulate a neon light cast.

## Shapes
The design system uses **Rounded (0.5rem)** corners as the standard. This strikes a balance between the precision of "Sharp" geometric shapes and the approachability of "Pill" shapes.

- **Cards & Modals:** 1rem (`rounded-lg`) for a softer, premium feel.
- **Buttons & Inputs:** 0.5rem to maintain a crisp, professional look.
- **Decorative Elements:** Use perfectly circular shapes for background "blobs" that provide the blurred color accents.

## Components

### Buttons
- **Primary:** Background is the Cyan-to-Purple gradient. Text is white. On hover, increase the glow effect (box-shadow).
- **Ghost:** Transparent background with a 1px Cyan border. On hover, the background fills with a 10% opacity Cyan tint.

### Cards (Project/Skill)
- **Visuals:** Glassmorphic background. 1px top-left border highlight.
- **Interaction:** On hover, the card should scale slightly (1.02x) and the border brightness should increase.

### Chips (Tech Stack)
- Small, dark navy capsules with Cyan text and a 5% Cyan background. Used to list languages like "Java", "Python", or "React".

### Input Fields
- Dark backgrounds with a subtle bottom-border. Upon focus, the border animates to a full Cyan stroke with a faint outer glow.

### Navigation
- A "floating" glassmorphic header that stays pinned to the top. Use a blur effect so the portfolio content is visible as it scrolls underneath.