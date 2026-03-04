# Presentation Brief: Termene.ro UX Assessment for Leadership

## File: presentation.html

Build a beautiful, click-through HTML presentation (like a slide deck) for Termene.ro leadership.
Use Reveal.js from CDN (https://cdn.jsdelivr.net/npm/reveal.js@5/dist/reveal.esm.js) OR build a clean custom slide deck with CSS transitions. Whichever looks more polished.

## Slides to Build

### Slide 1 — Title
- Title: "Termene.ro: Growth Unlocked"
- Subtitle: "A ProductLed Assessment & UX Redesign"
- Presented by: ProductLed Implementation Program
- Date: March 2026
- Dark background, premium feel

### Slide 2 — The Opportunity
- Headline: "A 7/10 product with a 4/10 go-to-market"
- 3 big stats in cards:
  - 100,000+ companies as customers
  - €16M RON revenue, +19% YoY
  - Strong enterprise logos (OMV Petrom, CEC Bank, EY)
- Bottom: "The infrastructure is there. The growth motion needs work."

### Slide 3 — What We Did
- Headline: "We went through the full experience"
- 4 steps with icons:
  1. 🔍 Explored the website and pricing
  2. 📝 Created a real account (no special access)
  3. 🏢 Searched and explored company profiles
  4. 📊 Mapped every friction point in the journey

### Slide 4 — Current Signup Experience (PROBLEM)
- Headline: "Problem 1: The signup sends the wrong signal"
- Show screenshot: screenshots/02-signup-form-email.png
- Annotation overlaid: Red arrow pointing to "În maximum 12 ore ești contactat de un consultant" → "Sales signal on a self-service page"
- Annotation: Red arrow to URL "/book-a-meeting-contact" → "URL screams 'talk to sales'"

### Slide 5 — The AI Gate (PROBLEM)
- Headline: "Problem 2: An AI terms gate blocks the product"  
- Show screenshot: screenshots/05-post-signup-ai-tc-gate.jpg
- Annotation: "User's first experience after signup: a legal disclaimer"
- Key text: "Users didn't sign up for AI. They came to check a company."

### Slide 6 — Wrong First Screen (PROBLEM)
- Headline: "Problem 3: Wrong first experience"
- Show screenshot: screenshots/07-post-signup-ai-chat-first-screen.jpg  
- Annotation: "An AI chatbot is shown instead of the company search — the core product"
- Score badge: "Onboarding: 3/10"

### Slide 7 — The Good News: The Product is Excellent
- Headline: "The product itself? Genuinely impressive."
- Show screenshot: screenshots/09-company-search-results.png
- 4 bullets of what works:
  - ✅ Deep financial data (10+ years of history)
  - ✅ Risk scoring (insolvency, credit, legal)
  - ✅ Real-time data from ANAF, ONRC, courts
  - ✅ AI Agents with real business context

### Slide 8 — The PLG Scorecard
- Headline: "ProductLed Readiness Score"
- 8 dimensions shown as a horizontal bar chart (use inline SVG or simple CSS bars):
  - Free Model: 5/10
  - Time to Value: 3/10
  - Viral Loops: 2/10
  - Self-Service: 3/10
  - Product Qualified Leads: 4/10
  - Pricing Transparency: 7/10
  - User Experience: 6/10
  - Network Effects: 7/10
- Overall: 4.6/10
- Color code: red for <4, amber for 4-6, green for >6

### Slide 9 — The Core Problem (visual summary)
- Headline: "The gap between sign up and value is too wide"
- Visual: A funnel or journey showing steps with friction scores
  - Landing → CTA: ⚠️ Mixed signals (sales vs. self-service)
  - Signup: OK ✅ (email only, fast OTP)
  - Post-signup: ❌ AI T&C gate
  - First screen: ❌ AI chatbot (not search)
  - Company search: ✅ Clean
  - Company profile: ✅ Excellent
  - Upgrade: ❌ Routes to consultant
- Key callout: "4+ friction points before first value"

### Slide 10 — The Fix: Show the prototype
- Headline: "What the ideal experience looks like"
- 4 preview screenshots (use placeholder/description boxes if no screenshots of prototype yet)
  - "New Landing: Value-first hero, product preview"
  - "New Signup: Google SSO, 3 clean steps, no consultant"
  - "New Dashboard: Search is the hero"
  - "New Profile: Free sections open, locked sections tastefully blurred"
- CTA: "→ View live prototype" (link to index.html)

### Slide 11 — Top 3 Quick Wins
- Headline: "3 changes that unlock growth immediately"
- Three big cards:
  1. 🎯 Fix the first experience
     "After signup → company search, pre-loaded with their own company. Goal: value in <60 seconds."
  2. 💳 Add self-service checkout for Esențial (€17/mo)
     "Remove consultant requirement. Credit card purchase. Keep consultants for Avansat+ only."
  3. 🔄 Make Redbill the viral hook
     "Free invoice reporting = data network effect. More reporters → more valuable data → more signups."

### Slide 12 — Roadmap
- Headline: "90-day roadmap"
- Three columns:
  - Quick Wins (<30 days): Fix landing, Google SSO, remove AI gate, OTP as text, progress bar during signup
  - Medium Term (30-90 days): Product tour, self-service checkout, 14-day Esențial trial, PQL tracking
  - Long Term (90+ days): Embeddable widgets, API-first PLG, team workspaces, referral program

### Slide 13 — Expected Impact
- Headline: "What moving the needle looks like"
- Metrics table:
  | Metric | Today (Est.) | Target |
  | Signup → First Search | ~30% | 80%+ |
  | Free → Paid Conversion | ~2% | 5-8% |
  | Time to First Value | 5+ min | <60 sec |
  | Self-Service Revenue | ~0% | 30%+ |

### Slide 14 — Thank You / Next Steps
- "Ready to build your PLG flywheel?"
- 3 next steps:
  1. Review the prototype (index.html)
  2. Prioritize the quick wins
  3. Schedule implementation kickoff
- ProductLed logo area + contact

## Design Requirements

- Dark theme: #0A0E1F background, white text
- Accent: #3D7FFF (blue), #10B981 (green), #F59E0B (amber), #EF4444 (red)  
- Font: Inter from Google Fonts
- Slide navigation: left/right arrow keys OR prev/next buttons
- Slide counter: "3 / 14" in bottom right
- Smooth transitions between slides
- Screenshots should display with a browser chrome frame around them (looks professional in presentations)
- Red annotation arrows/boxes can be done with CSS overlays
- Make it BEAUTIFUL. This is going to leadership.

## Implementation Notes
- If using Reveal.js: load from CDN, minimal config
- If building custom: CSS grid/flex for layout, JS for slide transitions
- All in ONE file: presentation.html
- Screenshots are in: screenshots/ folder (relative paths)
- Link to prototype files: index.html, signup.html, dashboard.html, company.html
