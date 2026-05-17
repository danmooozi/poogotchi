---
name: Digital Pet Retro-Modernism
colors:
  surface: "#fff9eb"
  surface-dim: "#e0dac7"
  surface-bright: "#fff9eb"
  surface-container-lowest: "#ffffff"
  surface-container-low: "#faf3e0"
  surface-container: "#f4eedb"
  surface-container-high: "#efe8d5"
  surface-container-highest: "#e9e2d0"
  on-surface: "#1e1c10"
  on-surface-variant: "#52443a"
  inverse-surface: "#333024"
  inverse-on-surface: "#f7f0de"
  outline: "#847469"
  outline-variant: "#d7c3b6"
  surface-tint: "#885120"
  primary: "#703e0e"
  on-primary: "#ffffff"
  primary-container: "#8d5524"
  on-primary-container: "#ffd7bb"
  inverse-primary: "#ffb77f"
  secondary: "#735c00"
  on-secondary: "#ffffff"
  secondary-container: "#fdcc00"
  on-secondary-container: "#6e5700"
  tertiary: "#245500"
  on-tertiary: "#ffffff"
  tertiary-container: "#317000"
  on-tertiary-container: "#a2f46e"
  error: "#ba1a1a"
  on-error: "#ffffff"
  error-container: "#ffdad6"
  on-error-container: "#93000a"
  primary-fixed: "#ffdcc3"
  primary-fixed-dim: "#ffb77f"
  on-primary-fixed: "#2f1500"
  on-primary-fixed-variant: "#6c3a0a"
  secondary-fixed: "#ffe086"
  secondary-fixed-dim: "#efc100"
  on-secondary-fixed: "#231a00"
  on-secondary-fixed-variant: "#574500"
  tertiary-fixed: "#a6f872"
  tertiary-fixed-dim: "#8bdb59"
  on-tertiary-fixed: "#092100"
  on-tertiary-fixed-variant: "#225100"
  background: "#fff9eb"
  on-background: "#1e1c10"
  surface-variant: "#e9e2d0"
typography:
  headline-lg:
    fontFamily: Space Mono
    fontSize: 32px
    fontWeight: "700"
    lineHeight: "1.2"
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Space Mono
    fontSize: 24px
    fontWeight: "700"
    lineHeight: "1.2"
  body-lg:
    fontFamily: Work Sans
    fontSize: 18px
    fontWeight: "500"
    lineHeight: "1.5"
  body-md:
    fontFamily: Work Sans
    fontSize: 16px
    fontWeight: "400"
    lineHeight: "1.5"
  status-number:
    fontFamily: Space Mono
    fontSize: 20px
    fontWeight: "700"
    lineHeight: "1"
  label-sm:
    fontFamily: Space Mono
    fontSize: 12px
    fontWeight: "700"
    lineHeight: "1"
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  container-padding: 24px
  gutter: 16px
  button-depth: 4px
  border-width: 3px
---

## Brand & Style

This design system captures the whimsical, nostalgic essence of 90s handheld gaming while applying a "Modern Retro" polish. The aesthetic is defined by a high-fidelity interpretation of 8-bit limitations: vibrant colors, chunky physical-feeling interfaces, and a playful "PooGotchi" character-driven narrative.

The target audience spans nostalgic adults and younger casual gamers seeking a tactile, low-stress engagement. The UI should feel like a physical object—a "toy" in the user's hand—evoking feelings of care, humor, and tactile satisfaction. We blend **Brutalism** (thick borders, high contrast) with **Skeuomorphism** (3D button depths) to create a UI that feels interactive and "squishy."

Key principles:

- **Toy-like Tactility:** Every interaction should feel like pressing a physical plastic button.
- **Lo-fi Clarity:** Use pixel-inspired geometry but rendered with modern anti-aliasing and smooth transitions.
- **Expressive Feedback:** Visual "bounces" and frame-by-frame animations for all state changes.

## Colors

The palette is anchored by "Poop Brown" (#8D5524), a warm, cocoa-toned primary that avoids being muddy by pairing with high-saturation action colors.

- **Primary (Cocoa):** Used for branding, character outlines, and primary containers.
- **Secondary (Golden):** Reserved for rewards, coins, and "happy" state highlights.
- **Success/Nature (Grass):** Used for health bars and environment-related UI.
- **System/Sky (Blue):** Used for informational modals and background depth.
- **Background (Pastel Cream):** A soft, warm neutral (#FDF6E3) that acts as the "plastic shell" of the device, reducing eye strain compared to pure white.

Contrast is maintained through heavy 4px dark brown (#3E2723) borders rather than traditional grey scales.

## Typography

Typography follows a dual-path strategy to balance character with legibility:

1.  **Headlines & Labels (Space Mono):** Used for all game-critical "retro" text. The monospaced nature of **Space Mono** mimics early LCD character displays. Use it for titles, button labels, and all uppercase micro-copy.
2.  **Status & Data (Work Sans):** Used for numerical values and longer descriptions. **Work Sans** provides a grounded, professional contrast that ensures players can quickly read stats like "Hunger" or "Happiness" levels at a glance.

**Formatting Rules:**

- All headlines should use a tight letter-spacing to feel "chunky."
- Avoid italics; emphasize via color shifts or bold weights only.
- Use uppercase for labels to reinforce the 8-bit aesthetic.

## Layout & Spacing

The layout philosophy mimics a **fixed-width handheld console**. The main "Game Screen" is a 1:1 or 4:3 ratio container centered on the device.

- **Grid:** Built on an 8px baseline. All dimensions and margins must be multiples of 8 to maintain "pixel alignment."
- **Safe Zones:** Use a generous 24px margin around the main device frame to simulate the bezel of a physical toy.
- **Desktop:** The game screen is contained within a "Virtual Device" graphic, centered on the screen.
- **Mobile:** The game screen expands to fill width, with physical-style buttons pinned to the bottom 30% of the viewport (simulating a D-pad and action buttons).

## Elevation & Depth

This design system rejects ambient shadows and blurs in favor of **Bold Borders and Hard Offsets**:

- **Layer 0 (Background):** Solid pastel fills.
- **Layer 1 (Containers):** 3px solid dark brown border with a 4px hard "drop shadow" (solid color, 100% opacity, shifted 4px right and 4px down).
- **Layer 2 (Buttons/Interactives):** Uses a "Skeuomorphic Press" effect. In the default state, a bottom-border of 4px creates a 3D "raised" look. On `:active` or `:press`, the element translates 2px down and the bottom border shrinks, simulating a physical mechanical click.
- **Backdrop:** No blurs. Use a 50% opacity solid brown overlay for modals to maintain the retro-tech feel.

## Shapes

The shape language is "Friendly-Chunky." We use **Rounded Level 2** (0.5rem / 8px) as the base for all containers and buttons to mimic molded plastic.

- **Primary Containers:** 8px corner radius.
- **Game Screen:** 16px corner radius (Large) to differentiate the "glass" from the "plastic shell."
- **Buttons:** 8px corner radius.
- **Icons:** Must be strictly pixel-art style, framed in circles with 2px solid borders.

## Components

### Buttons

Buttons are the core interaction point. They must feature a 3px dark brown border and a 4px "bottom-lip" of a darker shade of the button's background color to create a 3D effect. Labels are always centered, bold, and uppercase.

### Status Chips

Small pills used to show stats (e.g., "Full," "Sleepy"). These use a lighter version of the primary color, 2px borders, and no 3D depth to distinguish them from clickable buttons.

### Handheld Containers (Cards)

Cards feature a "Bezel" effect—an inner inset shadow (solid color) that makes the content look like it's recessed behind a screen.

### Input Fields

Inputs are styled as "inset boxes." Use a dark background (e.g., a very dark green or brown) with light-colored Space Mono text to simulate a retro terminal input.

### Progress Bars

"Health" or "Hunger" bars should be segmented. Instead of a smooth fill, use 10 discrete blocks to represent 0-100%, reinforcing the 8-bit grid logic.

### Pixel Icons

All icons must be created on a 24x24 pixel grid. Lines should be 1-2 pixels thick. Do not use gradients or transparency within the icon glyph itself.
