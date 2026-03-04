# Termene Presentation — ProductLed Rebrand Brief

## Task
Rebrand `presentation.html` to use the official ProductLed visual identity.
Do NOT change any content, copy, slide structure, or logic — only visual design.

## ProductLed Brand Specs

### Colors
- **Background (primary):** `#030302` (near-black — replaces current navy `#0A0E1F`)
- **Background (card/elevated):** `#0e0d0c` or `#1a1a18` (replaces `#131835`, `#1a2040`)
- **Accent / Primary:** `#f3ca07` (yellow — replaces current `#3D7FFF` blue)
- **Accent hover/glow:** `rgba(243, 202, 7, 0.15)` (yellow glow — replaces blue glow)
- **White:** `#ffffff` (keep)
- **Muted text:** `#c0bdb8` (replaces gray-400/500 where used for secondary text)

### Typography
- **Primary font:** Montserrat (for headings and labels)
- **Body font:** Inter (already loaded — keep for body text)
- Add Google Font import: `https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700;800;900&family=Inter:wght@400;500;600;700;800;900&display=swap`
- Update all heading font-family to 'Montserrat', sans-serif
- Keep body text as 'Inter', sans-serif

### Logo
Replace any existing "ProductLed" text branding with the official logo SVG:
  <img src="https://productled.com/cdn-images/6357526c0b897b08f455b7db/672273abe4013f1c98da5670_Logo-no-institute-white.svg" alt="ProductLed" height="28" style="display:block;">

### Accent Elements
- Progress dots, active slide indicators → `#f3ca07`
- Highlighted stat numbers, callout boxes → `#f3ca07` instead of blue
- Score bars (green/amber/red) → keep those semantic colors, just update accent
- Borders and glow effects → use yellow tones
- CTA buttons → background: #f3ca07; color: #030302; font-weight: 700;
- Tag/badge backgrounds → background: rgba(243,202,7,0.15); color: #f3ca07; border: 1px solid rgba(243,202,7,0.3);

## What to Change

### In the :root CSS variables block:
--navy: #030302;
--navy-light: #0e0d0c;
--navy-mid: #1a1a18;
--blue: #f3ca07;
--blue-hover: #d4ae06;
--blue-glow: rgba(243, 202, 7, 0.12);

### Fonts:
- Add Montserrat to the Google Fonts import URL
- Add font-family: 'Montserrat', sans-serif; to all h1, h2, h3, h4 CSS rules
- Keep Inter for body/paragraph text

### Slide 1 (Title slide):
- Replace any "ProductLed" text logo with the img tag above
- Subtitle should reflect: "Presented by Rodrigo Fernandez · ProductLed Implementation"
- Make the background slightly more visually interesting (subtle radial gradient from #1a1a18 at center to #030302 at edges)

### Navigation / Progress bar:
- Active dot → #f3ca07
- Progress line → #f3ca07

### Score/rating elements:
- Score number highlights → #f3ca07
- "Verdict" callout banner → yellow accent border

### Footer on every slide:
- Add small ProductLed logo (bottom-right corner of each slide)
- Add subtle text: "Confidential · ProductLed Implementation Program"

## What NOT to Change
- All text content, copy, numbers, recommendations
- Slide structure and order
- JavaScript slide navigation logic
- Screenshot references
- Semantic colors (green for good scores, red for bad scores) — only change the primary accent blue → yellow

## Output
Overwrite `presentation.html` in place. No new files.

## Verify
After completing, check that:
1. All #3D7FFF and #0A0E1F references are replaced
2. ProductLed logo SVG loads correctly (it's on their CDN, no auth needed)
3. Font import includes Montserrat
4. The presentation still navigates correctly (slide count, keyboard nav, etc.)
