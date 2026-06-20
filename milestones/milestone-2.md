# Milestone 2 — CSS Foundation: Dual-Theme Variables + Font Swap

**Status:** ✅ Complete

## What this milestone does

Replaces the old teal/navy color scheme and Playfair/Poppins/Raleway fonts with the new design system. No layout changes — only the color and typography layer.

## Design System

### Fonts
- **Headings:** Sora (700, 800) — imported from Google Fonts
- **Body/UI:** Inter (400, 500, 600) — imported from Google Fonts

### Dark Theme (`:root` default)
```css
--bg-primary:     #0F0F0F
--bg-secondary:   #1A1A2E
--card-bg:        #141414
--text-primary:   #FFFFFF
--text-secondary: #A0AEC0
--accent:         #4F9CF9
--accent-light:   #60A5FA
--border:         rgba(255, 255, 255, 0.08)
```

### Light Theme (`html[data-theme="light"]`)
```css
--bg-primary:     #F8FAFC
--bg-secondary:   #F1F5F9
--card-bg:        #FFFFFF
--text-primary:   #0F172A
--text-secondary: #475569
--accent:         #2563EB
--accent-light:   #3B82F6
--border:         rgba(0, 0, 0, 0.08)
```

## Tasks

- [x] Replace Google Fonts import (remove Playfair Display, Poppins, Raleway → add Sora, Inter)
- [x] Rewrite `:root` CSS variables with dark theme values
- [x] Add `html[data-theme="light"]` block with light theme values
- [x] Replace all hardcoded hex colors with CSS variable references
- [x] Update `font-family` on body, headings, nav to use Inter/Sora
- [x] Add `transition: background-color 0.3s ease, color 0.3s ease` to body for smooth theme switch

## Verification

Open in browser — dark theme should look identical in structure but with electric blue accents and new fonts. No broken layout.
