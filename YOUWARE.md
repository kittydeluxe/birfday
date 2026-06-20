# Birthday Card — Dark & Moody

## Overview

- **Stack**: React 18 + TypeScript + Vite 7 + Tailwind CSS 3 + Framer Motion
- **Core Command**: `npm run build`
- **Entry**: `src/main.tsx` → `src/App.tsx` → `src/components/BirthdayCard.tsx`

## Design Theme

- **Background**: Pure black (#000000)
- **Accent**: Deep dark red (#8B0000)
- **Highlight**: Dusty pink (#D8A7B1)
- **Text**: Soft blush (#e8d5d5)
- **Fonts**: Cormorant Garamond (serif headings), Inter (sans-serif UI)

## Architecture

Single-component interactive birthday card with 3 phases:

1. **Cover**: Dramatic entrance with animated heart, gradient text, and "tap to open" prompt
2. **Letter Envelope**: Redesigned letter-style envelope with V-flap, wax seal with heartbeat, and letter peeking inside. Tap seal → red & white petals fall
3. **Card Content**: Full scrollable experience with:
   - Hero section with birthday wish
   - **Dancing Cat** with pulsing hearts (above the letter)
   - Love letter in dark glass card with user's personal text
   - "5 Things I Adore" interactive reveal cards
   - Night sky with star particles
   - **Melting Candle** — tap to "light" it, reveals typewriter final quote
   - Music toggle button (top-right, fixed)
   - Footer

## Interactions & Animations

- Framer Motion for scroll-reveal, entrance, and hover animations
- CSS keyframes for floating particles, heartbeat, breathing glow, and falling petals
- Envelope open/close with CSS 3D transforms
- Red & white falling petals on envelope open
- Melting candle SVG with flickering flame animation
- Typewriter effect for the final love quote
- Glass-morphism cards with border glow on hover
- Noise texture overlay for cinematic feel
- Background music with toggle button

## Assets

- `public/dancing-cat.gif` — animated dancing cat GIF
- Google Fonts loaded via `index.html` link tags
- Particle and petal systems are pure CSS animations
- Melting candle is an inline SVG component

## Build Verification

Production bundle validated with `npm run build`; output confirmed in `dist/`.
