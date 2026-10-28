# China Trip 2026 — Eduard & Eloise

## Project
Single-page website presenting 3 itinerary options for a first trip to China (May 2-10, 2026, Paris roundtrip with Air France).

## Structure
- `index.html` — Single self-contained file (HTML + CSS + JS, no build tools or dependencies)
- Fonts: Google Fonts (Playfair Display + Inter)
- Images: Unsplash URLs + some custom URLs provided by Eduard

## The 3 Options
1. **Beijing + Shanghai** — Badge: "Recommended". The classic first-trip choice. Open jaw flights (CDG→PEK, PVG→CDG), bullet train between cities.
2. **Beijing + Chongqing** — Badge: "Desired". Imperial + cyberpunk city. SkyTeam domestic flights.
3. **Chongqing + Zhangjiajie** — Badge: "Next Time". Avatar mountains + cyberpunk. Quick Beijing stopover.

## Key UI Components
- **Hero**: Full-screen landing with animated lantern
- **Nav tabs**: Sticky tabs with coloured badges (Recommended/Desired/Next Time)
- **Why boxes**: Togglable cards (click to expand/collapse) explaining each option
- **Day cards**: Accordion-style day-by-day timeline (click header to toggle)
- **Activity galleries**: Horizontal scroll with snap, 3 photos per attraction. CSS: `.activity-gallery`
- **Highlight cards**: Grid of 4 cards per option with cover photos
- **Vote section**: Bottom section where Eloise can pick her favourite

## Photo Conventions
- Activity galleries use `<div class="activity-gallery">` with 3 `<img>` tags
- Unsplash URLs format: `https://images.unsplash.com/photo-XXXXX?w=600&h=400&fit=crop`
- Some photos are custom URLs (Reddit, external sites) provided by Eduard
- Highlight card images use class `highlight-img`
- Gallery is responsive: 92% width on mobile, 75% on desktop, with `aspect-ratio: 16/10`

## Content Guidelines
- Language: English
- Do NOT recommend specific restaurants — suggest typical dishes instead
- When mentioning place names, clarify if it's a neighbourhood/street/square (not a restaurant)
- Lunch entries should suggest local dishes to try, not specific venues
- All day cards start collapsed (no auto-open)

## Design Tokens
- Red: `#C41E3A` (primary accent, nav active, badges)
- Gold: `#D4A84B` (secondary accent, why-box border)
- Dark: `#1A1A2E` (headings, hero background)
- Cream: `#FFF9F0` (page background)
