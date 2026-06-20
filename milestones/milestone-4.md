# Milestone 4 — Hero Section Redesign

**Status:** ✅ Complete

## What this milestone does

Redesigns only the `#home` hero section with a clean two-column layout, circle profile picture, and CTA buttons.

## Design

### Layout
- Two-column flex row: text on left (55%), image on right (45%)
- Full viewport height (`min-height: 100vh`)
- Vertically centered with `align-items: center`

### Profile Picture
- Shape: Circle, 280px × 280px
- Border: 3px gradient ring using `accent` → `accent-light`
- Effect: Subtle box-shadow glow in accent color
- No float animation (static, sharp)

### Typography
- Name: Sora 800, ~3.5rem, name span in `var(--accent-light)`
- Subtitle: Inter 400, ~1.15rem, `var(--text-secondary)`

### CTA Buttons (two side by side)
- **Primary** ("View Projects"): solid `var(--accent)` background, white text, rounded pill
- **Secondary** ("Contact Me"): transparent with `1px solid var(--accent)`, accent text, rounded pill
- Both link to `#projects` and `#contact` respectively

### Removed
- Float keyframe animation on image
- `fadeInUp` opacity animation on title/subtitle (replaced with static layout)

## Tasks

- [x] Rewrite `.hero-section` CSS to two-column flex layout
- [x] Replace `.hero-image` styles with circle crop + gradient ring
- [x] Update hero HTML: wrap image in a container div for the ring effect
- [x] Add two CTA anchor buttons below the subtitle
- [x] Update responsive breakpoints (stack to single column on mobile)

## Verification

1. Desktop (1280px+): text left, circle pic right, both vertically centered
2. Mobile (375px): text stacked above image, image centered, buttons stacked
3. Both themes: image ring color matches accent
