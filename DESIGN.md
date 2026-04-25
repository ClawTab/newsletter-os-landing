---
version: alpha
name: Newsletter OS Landing
colors:
  bg: "#0a0a0f"
  bg-elevated: "#12121a"
  bg-card: "#1a1a24"
  border: "rgba(255,255,255,0.08)"
  text: "#e8e6e3"
  text-muted: "#8a8780"
  accent: "#7c6efa"
  accent-light: "#a299ff"
  accent-glow: "rgba(124,110,250,0.15)"
  success: "#4ade80"
  warning: "#fbbf24"
typography:
  hero:
    fontFamily: "DM Sans"
    fontSize: "clamp(2.5rem, 6vw, 4.5rem)"
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: "-0.03em"
  headline:
    fontFamily: "DM Sans"
    fontSize: "clamp(1.8rem, 4vw, 2.5rem)"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "-0.02em"
  body:
    fontFamily: "DM Sans"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Space Mono"
    fontSize: "0.75rem"
    fontWeight: 400
    lineHeight: 1
    letterSpacing: "0.1em"
  mono:
    fontFamily: "Space Mono"
    fontSize: "0.85rem"
    fontWeight: 700
    lineHeight: 1.5
rounded:
  sm: "6px"
  md: "8px"
  lg: "12px"
  xl: "16px"
  full: "9999px"
spacing:
  unit: "8px"
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "32px"
  xl: "64px"
  gutter: "24px"
  section-y: "6rem"
  section-x: "2rem"
  container-max: "1100px"
components:
  nav:
    backgroundColor: "rgba(10,10,15,0.8)"
    textColor: "{colors.text}"
    typography: "{typography.mono}"
    padding: "1.25rem 2rem"
  nav-link:
    textColor: "{colors.text-muted}"
    typography: "{typography.body}"
    padding: "0"
  nav-cta:
    backgroundColor: "{colors.accent}"
    textColor: "#ffffff"
    typography: "{typography.mono}"
    rounded: "{rounded.sm}"
    padding: "0.5rem 1rem"
  button-primary:
    backgroundColor: "{colors.accent}"
    textColor: "#ffffff"
    typography: "{typography.mono}"
    rounded: "{rounded.md}"
    padding: "0.875rem 1.75rem"
  button-primary-hover:
    backgroundColor: "{colors.accent-light}"
    transform: "translateY(-2px)"
  button-secondary:
    backgroundColor: "transparent"
    textColor: "{colors.text}"
    typography: "{typography.mono}"
    rounded: "{rounded.md}"
    padding: "0.875rem 1.75rem"
  button-secondary-hover:
    backgroundColor: "{colors.bg-card}"
    borderColor: "rgba(255,255,255,0.2)"
  card:
    backgroundColor: "{colors.bg-card}"
    borderColor: "{colors.border}"
    rounded: "{rounded.lg}"
    padding: "2rem"
  card-hover:
    borderColor: "rgba(124,110,250,0.3)"
    transform: "translateY(-4px)"
  input:
    backgroundColor: "{colors.bg-card}"
    textColor: "{colors.text}"
    borderColor: "{colors.border}"
    rounded: "{rounded.md}"
    padding: "0.875rem 1.25rem"
  input-focus:
    borderColor: "{colors.accent}"
  feature-icon:
    backgroundColor: "{colors.accent-glow}"
    borderColor: "{colors.accent}"
    rounded: "{rounded.md}"
    size: "40px"
  demo-bar:
    backgroundColor: "{colors.bg-card}"
    borderBottom: "1px solid {colors.border}"
    padding: "0.75rem 1rem"
  badge:
    backgroundColor: "{colors.bg-card}"
    borderColor: "{colors.border}"
    textColor: "{colors.accent-light}"
    rounded: "{rounded.full}"
    padding: "0.4rem 1rem"
---

## Brand & Style

Newsletter OS is a technical, agent-powered newsletter automation stack. The brand personality is precise and futuristic yet approachable — "tools for builders, by builders." The aesthetic draws from developer tooling and SaaS dashboards: dark surfaces, monospace accents, and a single vibrant purple that signals intelligence and automation.

The emotional response is one of capability and control. Visitors should feel that running a newsletter can be systematic, not chaotic. The visual language uses technical motifs (terminal-style elements, code-like typography) without being intimidating.

## Colors

The palette is anchored in deep space darks with a single electric purple accent.

- **Background (#0a0a0f):** Near-black with a subtle blue shift. Creates a foundation that feels like a terminal or IDE.
- **Elevated (#12121a):** Slightly lighter for sections that need visual separation.
- **Card (#1a1a24):** Surface for interactive elements and feature cards.
- **Text (#e8e6e3):** Warm off-white for primary content. Softer than pure white for reduced eye strain.
- **Muted (#8a8780):** For secondary text, captions, and metadata.
- **Accent (#7c6efa):** Electric purple — the signature color. Used for CTAs, links, badges, and hover states.
- **Accent Light (#a299ff):** Lighter purple for hover states and highlights.
- **Success (#4ade80):** Green for positive states (live indicators, checkmarks).
- **Warning (#fbbf24):** Amber for attention states.

## Typography

The dual-font strategy balances technical credibility with readability.

- **DM Sans** is the workhorse: used for all body text, headlines, and UI labels. Its geometric construction feels modern and engineered.
- **Space Mono** provides the technical voice: navigation labels, timestamps, code snippets, badges, and CTAs. The monospace creates a rhythm that says "this is a tool built by developers."

Headlines use tight negative letter-spacing to feel compact and authoritative. Mono labels are uppercase with wide positive letter-spacing for a technical, telemetry-like aesthetic.

## Layout & Spacing

The layout follows a centered, contained model with max-width 1100px.

- **Base unit:** 8px grid.
- **Sections:** 6rem vertical padding, 2rem horizontal.
- **Cards:** 1.5rem gaps in auto-fit grids. Each card has generous 2rem internal padding.
- **Navigation:** Fixed top bar with glassmorphism (blur + semi-transparent background).
- **Responsive:** Breaks at 768px and 640px. Mobile stacks grids to single columns.

## Elevation & Depth

Depth is achieved through tonal layering rather than heavy shadows.

- **Level 0 (Base):** #0a0a0f background.
- **Level 1 (Elevated sections):** #12121a with top/bottom borders.
- **Level 2 (Cards):** #1a1a24 with 1px border at 8% white opacity.
- **Glow effects:** Radial gradient overlays using accent-glow (purple at 15% opacity) behind hero and CTA sections.
- **Card hover:** Subtle border color shift to accent at 30% opacity + translateY(-4px).

No drop shadows on cards — the border + background contrast provides definition.

## Shapes

Soft-technical shape language.

- **Buttons:** 6-8px radius — modern but not pill-shaped.
- **Cards:** 12px radius — provides clear containment without feeling bubbly.
- **Badges/pills:** Full radius (9999px) for status indicators.
- **Feature icons:** 10px radius, square containers.

The slight rounding prevents the UI from feeling too aggressive while maintaining a technical aesthetic.

## Components

### Navigation
Fixed top bar with glassmorphism. Logo uses mono font with accent-light color. Links are muted by default, white on hover. CTA button is solid accent purple.

### Hero
Centered layout with gradient text effect on the headline (accent-light to teal gradient clip). Includes a terminal-style demo window showing a cron run output. The demo window uses a "traffic light" dot bar.

### Workflow Steps
Horizontal step cards with arrow connectors (desktop only). Each step has a mono number label, headline, and description. Hover lifts the card with accent border.

### Feature Cards
Auto-fit grid with icon, headline, and description. Icons sit in 40px square containers with accent glow background and accent border.

### Demo Card
Two-column layout: content left, visual right. Visual side shows a newsletter preview mockup with scoring badges.

### CTA Section
Centered with glow background gradient. Simple headline + subtext + button pattern.

## Do's and Don'ts

- Do use accent purple sparingly — it's the single action color
- Don't use more than two font weights on a single screen
- Do maintain 4.5:1 contrast ratio for all text
- Don't use pure white (#ffffff) — always use the warm off-white text token
- Do keep cards at 12px radius or below
- Don't add drop shadows to cards — rely on tonal contrast and borders
- Do uppercase all monospace labels with letter-spacing
- Don't use emoji in place of icons
