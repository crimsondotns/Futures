# Apple Design System Analysis

> Source: https://www.apple.com/  
> Measured: May 17, 2026  
> Analysis by DesignMD

---

---
name: Apple
url: https://www.apple.com/
colors:
  primary: '#0071e3'
  text-accent: '#2997ff'
  text-accent-hover: '#0066cc'
  background: '#f5f5f7'
  background-alt: '#ffffff'
  surface: '#fafafc'
  text-primary: '#1d1d1f'
  text-muted: '#6e6e73'
  text-inverse: '#f5f5f7'
  dark-surface: '#000000'
  border: '#d2d2d7'
typography:
  display:
    family: SF Pro Display
    size: 56px
    weight: 600
    line-height: 1.1
  heading:
    family: SF Pro Text
    size: 44px
    weight: 600
    line-height: 1.2
  body:
    family: SF Pro Text
    size: 17px
    weight: 400
    line-height: 1.4
spacing:
  base: 4px
  scale: [4, 8, 12, 16, 20, 24, 32, 48, 128]
radius:
  sm: 8px
  md: 11px
  full: 9999px
elevation:
  hero: 'rgba(0, 0, 0, 0.22) 3px 5px 30px 0px'
components:
  button-primary:
    bg: '{colors.primary}'
    text: '{colors.background-alt}'
    radius: '{radius.full}'
    padding: '8px 15px'
  card:
    bg: '{colors.background-alt}'
    radius: '{radius.md}'
    shadow: 'none'
motion:
  duration-base: '320ms'
  easing-standard: 'cubic-bezier(0.4, 0, 0.6, 1)'
---

## 1. Visual Theme & Atmosphere
Apple's digital presence is an exercise in focused minimalism, where the product is the undisputed hero. The design system achieves this through a highly constrained palette, primarily using `#1d1d1f` (near-black) text on `#f5f5f7` (light gray) or `#ffffff` (white) backgrounds. A single, vibrant blue (`#0071e3`) is reserved for primary calls-to-action, creating clear pathways for users. Typography is paramount, with `SF Pro Display` used for large, impactful headlines (56px) and `SF Pro Text` providing exceptional legibility for all other content, typically at a comfortable 17px base size.

The layout is defined by generous whitespace and a centered, flexible grid that gives product photography ample room to breathe. UI elements are flat, unobtrusive, and precisely aligned, eschewing shadows and gradients in favor of subtle rounding (`8px` or `11px`) and layering. Motion is purposeful and refined, with UI transitions governed by a distinct `cubic-bezier(0.4, 0, 0.6, 1)` curve for a responsive but gentle feel. The signature visual element is not a UI component but the product imagery itself—flawlessly rendered and presented with minimal distraction.

**Key Characteristics:**
*   **Typography-led hierarchy:** `SF Pro Display` at 56px/600 and `SF Pro Text` at 17px/400.
*   **Monochromatic base:** A strict palette of `#f5f5f7`, `#ffffff`, and `#1d1d1f`.
*   **Singular accent color:** Primary actions are exclusively `#0071e3`.
*   **Product-as-hero:** Full-bleed imagery and vast negative space.
*   **Flat UI:** Depth is implied through typography and layout, not shadows.
*   **Precise rounding:** A tight radius scale of `8px` and `11px` for containers.
*   **Refined motion:** UI transitions use a `320ms` duration with `cubic-bezier(0.4, 0, 0.6, 1)`.

## 2. Color Palette & Roles
The palette is intentionally sparse, creating a calm, focused environment where content and product visuals are the primary focus.

### Primary & Accent
*   **Primary (`#0071e3`)**: The core interactive blue. Used exclusively for primary buttons and critical interactive elements like focus rings.
*   **Text Accent (`#2997ff`)**: A slightly lighter, more vibrant blue for inline text links and secondary actions.
*   **Text Accent Hover (`#0066cc`)**: The hover and active state for text links, providing clear feedback.

### Neutral Scale
*   **Text Primary (`#1d1d1f`)**: The default text color for all headings and body copy on light backgrounds. It's a softer alternative to pure black.
*   **Text Muted (`#6e6e73`)**: Used for secondary text, footer links, and legal disclaimers where a lower contrast is desired.
*   **Background (`#f5f5f7`)**: The primary off-white background color for the main page body, providing a soft, non-glaring canvas.
*   **Background Alt (`#ffffff`)**: Pure white, used for distinct content sections and cards to create separation from the main background.
*   **Surface (`#fafafc`)**: A very subtle off-white, often used for navigation flyouts and modal backgrounds.

### Dark Theme
*   **Dark Surface (`#000000`)**: Pure black used as the background for immersive, product-focused sections, particularly for devices with OLED screens.
*   **Text Inverse (`#f5f5f7`)**: The primary text color on dark backgrounds, ensuring high readability.

### Borders
*   **Border (`#d2d2d7`)**: A light gray used for subtle separators, footer rules, and the default state of some form inputs.

## 3. Typography Rules
Typography is the backbone of the user interface, built around Apple's proprietary and highly legible `SF Pro` family. `SF Pro Display` is used for marketing headlines, while `SF Pro Text` is optimized for UI legibility at all other sizes.

*   **Font Family**:
    *   **Primary**: `SF Pro Text`, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol"
    *   **Display**: `SF Pro Display`, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol"
    *   **Monospace**: `SF Mono`, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace

*   **Hierarchy**:

| Role | Font | Size | Weight | Line Height | Letter Spacing | Notes |
| :--- | :--- | :--- | :--- | :--- | :--- |:---|
| Display | SF Pro Display | 56px | 600 | 1.1 | -0.02em | For hero headlines. |
| H1 | SF Pro Text | 44px | 600 | 1.2 | -0.01em | Main section titles. |
| H2 | SF Pro Text | 28px | 600 | 1.2 | normal | Sub-section titles. |
| H3 | SF Pro Text | 21px | 600 | 1.3 | normal | Card titles and tertiary headings. |
| Body | SF Pro Text | 17px | 400 | 1.4 | normal | Primary paragraph text. |
| Sub-body | SF Pro Text | 14px | 400 | 1.5 | normal | Secondary text, descriptions. |
| Caption | SF Pro Text | 12px | 400 | 1.5 | 0.01em | Legal footnotes, metadata, nav links. |

*   **Principles**:
    *   **Clarity First**: The system prioritizes legibility above all else. Type is set with generous line height and tracking.
    *   **Strict Hierarchy**: A clear and limited set of type styles ensures users can scan and understand content structure instantly.
    *   **Weight for Emphasis**: `600` weight is reserved for headings to create a clear distinction from `400` weight body copy.

## 4. Component Stylings

### Buttons
Buttons are used for key actions. They are clearly delineated by color and shape.

**Primary Button**
The primary CTA, using the brand's vibrant blue. It has a friendly, pill-shaped radius.

```css
.button-primary {
  display: inline-block;
  background-color: var(--color-primary, #0071e3);
  color: var(--color-text-inverse, #ffffff);
  font-family: "SF Pro Text", sans-serif;
  font-size: 17px;
  font-weight: 400;
  line-height: 1;
  text-align: center;
  padding: 12px 24px;
  border: 1px solid transparent;
  border-radius: var(--radius-full, 9999px);
  cursor: pointer;
  transition: background-color 0.2s ease-out;
}

.button-primary:hover {
  background-color: #0077ed; /* inferred from screenshot */
}

.button-primary:active {
  background-color: #0066cc; /* inferred from screenshot */
}

.button-primary:disabled {
  background-color: var(--color-primary, #0071e3);
  opacity: 0.42;
  cursor: not-allowed;
}
```

**Secondary Button**
Used for less critical actions, often appearing alongside a primary button. It inverts the primary style for a lighter feel.

```css
.button-secondary {
  display: inline-block;
  background-color: transparent;
  color: var(--color-text-accent, #2997ff);
  font-family: "SF Pro Text", sans-serif;
  font-size: 17px;
  font-weight: 400;
  line-height: 1;
  text-align: center;
  padding: 12px 24px;
  border: 1px solid var(--color-text-accent, #2997ff);
  border-radius: var(--radius-full, 9999px);
  cursor: pointer;
  transition: background-color 0.2s ease-out, color 0.2s ease-out;
}

.button-secondary:hover {
  background-color: var(--color-text-accent, #2997ff);
  color: var(--color-background-alt, #ffffff);
}

.button-secondary:active {
  background-color: var(--color-text-accent-hover, #0066cc);
  border-color: var(--color-text-accent-hover, #0066cc);
  color: var(--color-background-alt, #ffffff);
}

.button-secondary:disabled {
  color: var(--color-text-accent, #2997ff);
  border-color: var(--color-text-accent, #2997ff);
  opacity: 0.42;
  cursor: not-allowed;
}
```

**Ghost Button (Text Link)**
Used for tertiary actions, rendered as a simple text link to minimize visual weight.

```css
.button-ghost {
  background-color: transparent;
  color: var(--color-text-accent, #2997ff);
  font-family: "SF Pro Text", sans-serif;
  font-size: 17px;
  font-weight: 400;
  padding: 0;
  border: none;
  border-radius: 0;
  cursor: pointer;
  text-decoration: none;
  transition: color 0.2s ease-out;
}

.button-ghost:hover {
  color: var(--color-text-accent-hover, #0066cc);
  text-decoration: underline;
}

.button-ghost:disabled {
  opacity: 0.42;
  cursor: not-allowed;
  text-decoration: none;
}
```

### Cards & Containers
Cards are large, simple containers for content, relying on whitespace and background color changes rather than borders or shadows.

```css
.card {
  background-color: var(--color-background-alt, #ffffff);
  border-radius: var(--radius-md, 11px);
  padding: 48px;
  text-align: center;
  overflow: hidden;
  transition: transform 0.3s cubic-bezier(0.4, 0, 0.6, 1);
}

/* Hover effect is typically on a link within the card, not the card itself */
.card a.tile-link:hover {
  text-decoration: underline;
  text-decoration-color: var(--color-text-accent, #2997ff);
}
```

### Inputs & Forms
Form elements are minimal and clean, with clear focus states.

```css
.form-label {
  display: block;
  font-family: "SF Pro Text", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: var(--color-text-muted, #6e6e73);
  margin-bottom: 8px;
}

.text-input {
  width: 100%;
  padding: 12px 16px;
  font-family: "SF Pro Text", sans-serif;
  font-size: 17px;
  color: var(--color-text-primary, #1d1d1f);
  background-color: var(--color-background-alt, #ffffff);
  border: 1px solid var(--color-border, #d2d2d7);
  border-radius: var(--radius-sm, 8px);
  transition: border-color 0.2s ease-out, box-shadow 0.2s ease-out;
}

.text-input:focus,
.text-input:focus-visible {
  border-color: var(--color-primary, #0071e3);
  outline: 2px solid var(--color-primary, #0071e3);
  outline-offset: 3px;
}

.text-input:disabled {
  background-color: var(--color-background, #f5f5f7);
  opacity: 0.5;
  cursor: not-allowed;
}
```

### Navigation
The global navigation is a thin, semi-transparent bar that sits atop the content.

```css
.global-nav {
  position: sticky;
  top: 0;
  width: 100%;
  height: 44px;
  background-color: rgba(250, 250, 252, 0.7); /* --sk-fill-secondary with blur */
  backdrop-filter: saturate(180%) blur(20px);
  z-index: 9999;
}

.nav-link {
  font-family: "SF Pro Text", sans-serif;
  font-size: 12px;
  font-weight: 400;
  color: var(--color-text-primary, #1d1d1f);
  text-decoration: none;
  padding: 0 8px;
  transition: opacity 0.2s ease-out;
}

.nav-link:hover {
  opacity: 0.7;
}

.nav-link.active {
  opacity: 1;
  /* Active state is often contextual, not a simple class */
}
```

### Links

```css
a {
  color: var(--color-text-accent, #2997ff);
  text-decoration: none;
  transition: color 0.2s ease-out;
}

a:hover {
  color: var(--color-text-accent-hover, #0066cc);
  text-decoration: underline;
}

a:visited {
  color: var(--color-text-accent, #2997ff);
}
```

### Badges
(none observed in source)

## 5. Layout Principles

*   **Spacing System**: The system uses a multiple of a 4px base unit. The scale is `[4, 8, 12, 16, 20, 24, 32, 48, 128]`.
    *   **Usage Context**:
        *   `4px`, `8px`: Micro-spacing within components (e.g., icon to text).
        *   `12px`, `16px`: Component padding.
        *   `24px`: Gutter between grid items.
        *   `32px`, `48px`: Margin between components and content blocks.
        *   `128px`: Vertical padding for major page sections.

*   **Grid & Container**: The primary content grid is centered with a max-width around `980px` for dense content and `1068px` for marketing layouts. The grid is typically 12 columns but often used as 2, 3, or 4-column layouts for product tiles.

*   **Whitespace Philosophy**: Whitespace is a primary design tool. It is used generously to create focus, improve readability, and impart a sense of calm and quality. Large, empty spaces around product imagery are a hallmark of the design.

*   **Border Radius Scale**:
    *   `8px`: Used for smaller components like inputs and embedded media.
    *   `11px`: The standard radius for content cards and containers.
    *   `9999px`: Used to create pill-shaped buttons.

## 6. Depth & Elevation
The design system is fundamentally flat. Depth is created through typographic hierarchy and content layering, not shadows. A single, diffuse shadow is reserved for specific hero imagery to give it a subtle lift from the page.

| Level | Treatment | Use | Z-Index |
| :--- | :--- | :--- | :--- |
| z-0: Flat | `box-shadow: none;` | Default state for all page content, cards, and text. | 0 |
| z-1: Content | `box-shadow: none;` | Active content links and interactive elements. | 1-4 |
| z-2: Hero | `rgba(0, 0, 0, 0.22) 3px 5px 30px 0px` | Applied to hero product imagery to create a subtle float. | 3 |
| z-3: Navigation | `backdrop-filter: blur(20px);` | The main global navigation bar. | 9999 |
| z-4: Modal/Overlay | `background: rgba(250, 250, 252, 0.7);` | Full-screen overlays like the locale switcher or menu flyouts. | 10000 |

**Shadow Philosophy**: Shadows are avoided in UI components. The system prefers a clean, graphic aesthetic. The single defined shadow is a content-level effect for hero photography, not a state indicator for buttons or cards.

## 7. Do's and Don'ts

### Do
*   **Do** use `#1d1d1f` for primary body text on `#f5f5f7` backgrounds.
*   **Do** use `SF Pro Display` at `56px` for major hero titles only.
*   **Do** reserve the `#0071e3` blue for primary calls-to-action.
*   **Do** use the `48px` or `128px` spacing tokens for vertical separation between sections.
*   **Do** use a `9999px` border-radius for all pill-shaped buttons.
*   **Do** use a `11px` radius for all primary content cards.
*   **Do** ensure all interactive elements have a focus state with a `3px` outline offset.
*   **Do** use pure black (`#000000`) backgrounds only for immersive product sections.
*   **Do** pair `#f5f5f7` text on `#000000` backgrounds for dark mode content.
*   **Do** use `17px` `SF Pro Text` as the default for all paragraph copy.

### Don't
*   **Don't** use shadows on buttons, inputs, or standard cards.
*   **Don't** introduce new colors; stick to the primary blue and neutral gray scale.
*   **Don't** use text smaller than `12px`, even for legal footnotes.
*   **Don't** use borders to separate most content sections; use whitespace instead.
*   **Don't** use any font other than `SF Pro` or the specified system fallbacks.
*   **Don't** use a radius other than `8px`, `11px`, or `9999px`.
*   **Don't** place text over complex product imagery without a protective scrim.
*   **Don't** use `#6e6e73` on `#fafafc` for body text; its 4.86:1 ratio is for secondary text only.
*   **Don't** underline links by default; only apply underlines on `:hover`.
*   **Don't** create buttons that are not pill-shaped.

## 8. Responsive Behavior
The site uses a fluid-responsive approach with specific breakpoints for reflowing content. The values below are measured from the site's CSS.

*   **Breakpoints**:

| Breakpoint Name | Width | Key Changes |
| :--- | :--- | :--- |
| Desktop Large | `1441px+` | Increased whitespace and padding. Grid remains at max-width. |
| Desktop | `1069px - 1440px` | Standard desktop view. Content at `1068px` max-width. |
| Tablet | `735px - 1068px` | Content reflows. 2-3 column grids stack to 2 columns. Type sizes remain large. |
| Mobile | `max-width: 734px` | Single-column layout. Navigation collapses to a hamburger menu. Touch targets are enlarged. |

*   **Touch Targets**:
    *   Buttons maintain a minimum height of `44px`.
    *   Links in footers and dense areas have ample line-height to ensure they can be tapped easily.
    *   Minimum spacing between interactive elements is `16px`.

*   **Collapsing Strategy**:
    *   **Navigation**: The primary navigation bar collapses into a single "menu" icon, which opens a full-screen overlay.
    *   **Cards**: Multi-column card layouts (e.g., 3-up) stack vertically into a single column on mobile.
    *   **Typography**: Hero headline sizes (56px, 44px) are reduced significantly on mobile to prevent overflow.
    *   **Padding**: Section padding is reduced from `128px` to `48px` or less on mobile.
    *   **Buttons**: Buttons may span the full width of the screen on mobile for emphasis.

## 9. Agent Prompt Guide

*   **Quick Color Reference**:
    *   Primary Action BG: `#0071e3`
    *   Text Link: `#2997ff`
    *   Text Link Hover: `#0066cc`
    *   Main Background: `#f5f5f7`
    *   Card/Section Background: `#ffffff`
    *   Dark Background: `#000000`
    *   Primary Text (on light): `#1d1d1f`
    *   Inverse Text (on dark): `#f5f5f7`

*   **Iteration Guide**:
    1.  **CTAs**: All primary buttons use background `#0071e3`, text `#ffffff`, and `border-radius: 9999px`.
    2.  **Typography**: Body text is `17px` `SF Pro Text` in `#1d1d1f`. Headings are `600` weight.
    3.  **Spacing**: Use the scale: `[4, 8, 12, 16, 20, 24, 32, 48, 128]`. Default margin between elements is `24px` or `32px`.
    4.  **Radius**: Use `11px` for cards, `8px` for inputs, `9999px` for buttons. No other values.
    5.  **Cards**: Default card is background `#ffffff` with `11px` radius and no border or shadow.
    6.  **Inputs**: Default input has a `1px` border of `#d2d2d7` and an `8px` radius.
    7.  **Focus State**: All focusable elements must have a `2px` solid outline of `#0071e3` with a `3px` offset.
    8.  **Navigation**: The main nav bar is `44px` tall with a blurred background effect.
    9.  **Shadows**: Do not apply `box-shadow` to any UI component.
    10. **Contrast**: Ensure body text (`#1d1d1f` on `#f5f5f7`) passes AAA. Muted text (`#6e6e73`) is only for non-essential copy.