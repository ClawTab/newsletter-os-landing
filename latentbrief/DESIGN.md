---
version: alpha
name: LatentBrief Landing
colors:
  primary: "#1a1c1c"
  secondary: "#454747"
  accent: "#4caf93"
  accent-light: "#6dd5b8"
  accent-glow: "rgba(76,175,147,0.15)"
  surface: "#0a0a0f"
  surface-elevated: "#12121a"
  surface-card: "#1a1a24"
  on-surface: "#e8e6e3"
  on-surface-muted: "#8a8780"
  border: "rgba(255,255,255,0.08)"
  background: "#0a0a0f"
  on-background: "#e8e6e3"
  error: "#ff6b6b"
  outline: "rgba(255,255,255,0.08)"
  outline-variant: "rgba(255,255,255,0.05)"
  inverse-surface: "#e8e6e3"
  inverse-on-surface: "#1a1a24"
typography:
  display-lg:
    fontFamily: "DM Sans"
    fontSize: "clamp(2.5rem, 6vw, 4rem)"
    fontWeight: 700
    lineHeight: 1.15
    letterSpacing: "-0.03em"
  headline-lg:
    fontFamily: "DM Sans"
    fontSize: "clamp(1.6rem, 4vw, 2.2rem)"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "-0.02em"
  body-lg:
    fontFamily: "DM Sans"
    fontSize: "1.2rem"
    fontWeight: 400
    lineHeight: 1.5
  body-md:
    fontFamily: "DM Sans"
    fontSize: "0.95rem"
    fontWeight: 400
    lineHeight: 1.6
  body-sm:
    fontFamily: "DM Sans"
    fontSize: "0.9rem"
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: "Space Mono"
    fontSize: "0.7rem"
    fontWeight: 400
    lineHeight: 1
    letterSpacing: "0.08em"
  label-md:
    fontFamily: "Space Mono"
    fontSize: "0.75rem"
    fontWeight: 400
    lineHeight: 1
    letterSpacing: "0.1em"
  mono-sm:
    fontFamily: "Space Mono"
    fontSize: "0.8rem"
    fontWeight: 700
    lineHeight: 1.5
rounded:
  none: "0px"
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
  section-y: "5rem"
  section-x: "2rem"
  container-max: "1000px"
components:
  nav:
    backgroundColor: "rgba(10,10,15,0.8)"
    textColor: "{colors.on-surface}"
    borderColor: "{colors.border}"
    backdropFilter: "blur(20px)"
    padding: "1.25rem 2rem"
  nav-logo:
    fontFamily: "{typography.label-md.fontFamily}"
    textColor: "{colors.accent-light}"
  nav-link:
    textColor: "{colors.on-surface-muted}"
    fontSize: "0.9rem"
  nav-link-hover:
    textColor: "{colors.on-surface}"
  nav-cta:
    backgroundColor: "{colors.accent}"
    textColor: "#ffffff"
    typography: "{typography.mono-sm}"
    rounded: "{rounded.sm}"
    padding: "0.5rem 1rem"
  hero-headline:
    textColor: "{colors.on-surface}"
    typography: "{typography.display-lg}"
  hero-subheadline:
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.body-lg}"
  email-input:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.on-surface}"
    borderColor: "{colors.border}"
    rounded: "{rounded.md}"
    padding: "0.875rem 1.25rem"
  email-input-focus:
    borderColor: "{colors.accent}"
  submit-button:
    backgroundColor: "{colors.accent}"
    textColor: "#ffffff"
    typography: "{typography.mono-sm}"
    rounded: "{rounded.md}"
    padding: "0.875rem 1.5rem"
  submit-button-hover:
    backgroundColor: "{colors.accent-light}"
    transform: "translateY(-1px)"
  value-card:
    backgroundColor: "{colors.surface-card}"
    borderColor: "{colors.border}"
    rounded: "{rounded.lg}"
    padding: "2rem"
  value-card-hover:
    borderColor: "rgba(76,175,147,0.3)"
    transform: "translateY(-2px)"
  sample-card:
    backgroundColor: "{colors.surface-card}"
    borderColor: "{colors.border}"
    rounded: "{rounded.lg}"
    padding: "1.75rem"
  sample-card-hover:
    borderColor: "rgba(76,175,147,0.3)"
  footer:
    borderColor: "{colors.border}"
    textColor: "{colors.on-surface-muted}"
---

## Brand & Style

LatentBrief is a tech newsletter brand focused on signal extraction — finding the stories that matter beneath the noise of AI hype. The brand personality is editorially rigorous yet accessible: like a sharp analyst who explains complex trends in plain English.

The aesthetic is "editorial tech" — mixing the gravitas of a quality publication with the precision of developer tooling. The dark background creates focus. The teal accent evokes clarity and signal (like a waveform on an oscilloscope). The design should feel like you're entering a quiet reading room, not a flashy marketing page.

## Colors

The palette is extremely restrained. A near-black foundation with a single teal accent.

- **Surface (#0a0a0f):** Deep dark background. Slightly blue-shifted black for a technical feel.
- **Surface Elevated (#12121a):** For section separators and sample backgrounds.
- **Surface Card (#1a1a24):** Card and container backgrounds.
- **On-Surface (#e8e6e3):** Primary text — warm off-white.
- **On-Surface Muted (#8a8780):** Secondary text, captions, placeholders.
- **Accent (#4caf93):** Teal green — the signature color. Used for CTAs, links, labels, hover states, and the gradient text effect in headlines.
- **Accent Light (#6dd5b8):** Lighter teal for hover states and gradient endpoints.

## Typography

Same dual-font strategy as Newsletter OS, adapted for editorial reading.

- **DM Sans** for all prose and headlines. The geometric sans feels contemporary and clean.
- **Space Mono** for labels, CTAs, and metadata. Creates rhythm and hierarchy.

The hero headline uses a gradient text effect (accent-light to purple) via background-clip — the only decorative text treatment on the page. All other text is solid color.

## Layout & Spacing

Centered, contained layout with max-width 1000px.

- **Base unit:** 8px grid.
- **Sections:** 5rem vertical padding (tighter than Newsletter OS — this is a simpler page).
- **Value cards:** 3-column auto-fit grid with 1.5rem gaps.
- **Sample cards:** Stacked single column with 1.5rem gaps.
- **Footer:** Centered with border-top separator.
- **Responsive:** Stacks to single column below 768px, adjusts padding.

## Elevation & Depth

Flat design with tonal layers.

- **Level 0:** #0a0a0f background.
- **Level 1 (Samples section):** #12121a with top/bottom borders.
- **Level 2 (Cards):** #1a1a24 with 1px border at 8% white opacity.
- **Hero glow:** Radial gradient overlay using accent-glow (teal at 15% opacity).
- **CTA glow:** Linear gradient from transparent to accent-glow and back.
- **Card hover:** Border shifts to teal at 30% opacity, subtle translateY(-2px).

No shadows used anywhere — depth is purely tonal.

## Shapes

Soft-technical, matching Newsletter OS family.

- **Buttons:** 8px radius.
- **Cards:** 12px radius.
- **Inputs:** 8px radius.
- **Navigation:** No radius (full-width bar).

## Components

### Navigation
Fixed top bar matching Newsletter OS structure but with teal accent. Logo reads "Latent" (accent) + "Brief" (muted). Links: "Sample Issue", "Subscribe", "Newsletter OS" (external).

### Hero
Centered layout with gradient headline. Subheadline explains the value proposition. Email capture form with inline button. Trust note below.

### Value Cards (3-up)
Three feature cards explaining what you get, what you don't get, and who it's for. Each has a mono number label, headline, and body text.

### Sample Issues
Stacked cards showing example newsletter content. Each card has a headline, summary paragraph, and "Read more →" link in accent color. Section has elevated background.

### CTA
Simple centered section with glow background. Headline + subtext + email form.

### Footer
Minimal footer with link row (GitHub, Newsletter OS) and copyright line.

## Do's and Don'ts

- Do use the teal accent sparingly — it's the only color besides neutrals
- Don't use purple — that's reserved for Newsletter OS branding
- Do keep text warm off-white, never pure white
- Don't use more than two font weights on a single screen
- Do maintain 4.5:1 contrast ratio
- Do limit decorative elements — the design is intentionally minimal
- Don't add shadows to cards
- Do use gradient text effect only on the hero headline
