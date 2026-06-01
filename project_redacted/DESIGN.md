---
name: 'Project: REDACTED'
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#20201f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353535'
  on-surface: '#e5e2e1'
  on-surface-variant: '#e3beb8'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#aa8984'
  outline-variant: '#5a403c'
  surface-tint: '#ffb4a8'
  primary: '#ffb4a8'
  on-primary: '#690000'
  primary-container: '#8b0000'
  on-primary-container: '#ff907f'
  inverse-primary: '#b52619'
  secondary: '#ffb4a8'
  on-secondary: '#621109'
  secondary-container: '#842a1f'
  on-secondary-container: '#ff9f90'
  tertiary: '#c6c6c6'
  on-tertiary: '#303030'
  tertiary-container: '#424242'
  on-tertiary-container: '#afafaf'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdad4'
  primary-fixed-dim: '#ffb4a8'
  on-primary-fixed: '#410000'
  on-primary-fixed-variant: '#920703'
  secondary-fixed: '#ffdad4'
  secondary-fixed-dim: '#ffb4a8'
  on-secondary-fixed: '#410000'
  on-secondary-fixed-variant: '#81281d'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c6'
  on-tertiary-fixed: '#1b1b1b'
  on-tertiary-fixed-variant: '#474747'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353535'
typography:
  display:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.05em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.2'
  body-lg:
    fontFamily: Space Grotesk
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-sm:
    fontFamily: Space Grotesk
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  code:
    fontFamily: Space Grotesk
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.4'
    letterSpacing: 0.1em
  label:
    fontFamily: Space Grotesk
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1'
spacing:
  unit: 8px
  gutter: 24px
  margin: 40px
  container-max: 1200px
---

## Brand & Style

This design system is built to evoke a sense of dread, claustrophobia, and clinical detachment. The brand personality is cold, industrial, and inherently unstable—mirroring a corrupted government terminal or a leaked classified dossier. It targets an audience that appreciates psychological horror, environmental storytelling, and the "analog horror" aesthetic.

The visual style is a hybrid of **Digital Brutalism** and **High-Contrast Terminal UI**. It rejects soft aesthetics in favor of sharp edges, heavy borders, and intentional visual "errors." The UI should feel like a physical object that has been damaged or censored. Key stylistic hallmarks include high-contrast shadows that obscure information, scanline overlays, and "redacted" blocks that hide sensitive data.

## Colors

The palette is restricted to a suffocating range of deep charcoals and visceral reds. 

- **Primary (#8B0000):** Used for critical alerts, interactive states, and headers. It represents both authority and biological horror.
- **Background (#1A1A1A):** A deep, non-pure black that provides enough range for pure black (#000000) shadows and redaction marks to remain visible.
- **Accent/Secondary:** Deeper crimsons are used for hover states and low-priority warnings.
- **Functional:** Off-white/Grey is used for legibility, ensuring the text feels like it is emanating from a low-quality CRT monitor rather than a modern screen.

Transparency is rarely used; when data is hidden, it is blocked out with solid black rather than faded.

## Typography

Typography in this design system utilizes **Space Grotesk** to achieve a technical, industrial appearance. The font's geometric quirks provide a "synthetic" feel that complements the terminal theme.

- **Headlines:** Use heavy weights with tight letter-spacing to feel oppressive and dominant.
- **Body Text:** Maintain generous line height for legibility against dark backgrounds, but keep the font size slightly smaller than standard to mimic document densities.
- **Labels:** Always uppercase with increased tracking (letter-spacing) to simulate stamped serial numbers or file classifications.
- **Stylistic Note:** Occasionally apply a slight horizontal skew (italics) or a "glitch" offset (duplicate text layer shifted by 2px) to headers to indicate system corruption.

## Layout & Spacing

The layout philosophy follows a **Rigid Fixed Grid**. Content is housed within visible or implied containers that follow a strict 12-column structure. 

- **Grid:** Use 24px gutters. Elements should align strictly to the grid to maintain an "official document" feel.
- **Asymmetry:** Occasionally break the grid with "corrupted" elements—images or text blocks that are offset by 8px or 16px to create visual tension.
- **Margins:** Large outer margins (40px+) create a sense of isolation for the central content.
- **Redaction:** Use black blocks to fill empty grid cells, suggesting that information has been removed from those spaces.

## Elevation & Depth

This design system eschews modern soft shadows in favor of **Hard-Edge Shadows** and **Tonal Layering**.

- **Depth:** Conveyed through "stacked" containers. A card sits "above" the background not through a blur, but by having a 1px border of #8B0000 and a 4px offset solid black shadow (#000000).
- **Redaction Layers:** Use solid black overlays to hide content. These should have 100% opacity. 
- **Atmospheric Overlays:** A persistent, low-opacity "scanline" or "noise" texture should be fixed to the viewport to give the impression of a physical screen.
- **Visual Glitches:** Interactive elements should "flicker" or shift their shadow position on hover, creating an unstable depth effect.

## Shapes

The shape language is strictly **Sharp (0px)**. There are no rounded corners in this design system. 

All buttons, inputs, cards, and images must have 90-degree angles. This reinforces the industrial, brutalist nature of the site and the "unfeeling" personality of a government machine. Borders should be used frequently to define these shapes, typically 1px or 2px thick.

## Components

### Buttons
- **Default:** Solid #1A1A1A background with a 1px #8B0000 border and red text.
- **Hover:** The border thickness increases, and text undergoes a "glitch" animation (briefly changing characters or shifting color).
- **Active:** Background becomes #8B0000 with black text.

### Inputs & Text Fields
- Styled as command-line prompts. Use a "greater-than" symbol (>) as a prefix for all text inputs.
- The cursor should be a blinking solid block.

### Cards & Dossiers
- Cards feature a "Classified" header bar in solid red with black uppercase text.
- Content is separated by 1px horizontal dividers that look like scratched metal or scanned lines.

### Chips & Tags
- Rectangular blocks with high-contrast backgrounds. Used for status indicators like "TERMINATED," "CONTAINED," or "MISSING."

### Redacted Text
- A specific component for "spoiler" content. It appears as a solid black box over text. On hover, the box flickers or dissolves into a "blood spatter" texture to reveal the text underneath.

### Media Containers
- Images should have a high-contrast, slightly desaturated filter applied. 
- Apply a "glitch" border—a 1px frame that is slightly offset from the image itself.