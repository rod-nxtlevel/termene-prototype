# Termene.ro — Ideal UX Prototype Brief

## What We're Building
A **pure HTML/CSS/JS prototype** of the ideal product-led onboarding for Termene.ro — a Romanian B2B business intelligence platform. No backend. Open with index.html in any browser.

## What Termene.ro Does
Aggregates financial, legal, and fiscal data on Romanian companies. Users can look up any company by name or CUI (tax ID) and see: financial performance, risk scores (insolvency, credit), legal cases, shareholder networks, ANAF tax status, sector comparisons.

## Problems to Fix (from assessment)
1. "Create Account" routes to /book-a-meeting-contact — screams sales-led
2. AI T&C gate blocks the product right after signup
3. First post-signup screen is an AI chatbot (wrong first experience)
4. Zero onboarding — no tour, no guidance, no "aha moment" engineering
5. "Profil incomplet" warning badge immediately after signup
6. OTP code sent as image (can't copy-paste on mobile)
7. No Google/LinkedIn SSO
8. No self-service upgrade (always routes to consultant)

## Pages to Build

### 1. Landing Page (index.html)
- Hero: "Make data-driven decisions about Romanian companies"
- Social proof: "100,000+ companies trust Termene" + 3 logos
- CTA: "Try free — no credit card" → goes to signup
- Show blurred company profile preview to tease value
- Secondary CTA: "See pricing"

### 2. Signup Flow (modal or separate page)
- Google SSO button (primary)
- Email alternative below
- If email: show OTP step with TEXT code input (not image)
- Then password step
- Progress indicator: Step 1 of 3
- NO mention of consultants. NO "we'll contact you in 12 hours."

### 3. Post-Signup First Experience (MOST IMPORTANT PAGE)
- Welcome message: "Find your first company"
- Large centered search bar is the HERO
- Subtitle: "Search by company name, CUI (tax ID), email, or phone"
- Pre-filled suggested example: "Try: Termene Just SRL"
- What you get FREE: 4 icons (unlimited company lookups, fiscal status, basic profile, invoice reporting)
- NO AI chat. NO token limit warnings. NO profile completion nags.

### 4. Company Profile Page (the "aha moment")
Header:
- Company name, green "Active" badge, city
- Quick stats row: Revenue (16M RON +19%), Profit (2.1M RON), Employees (48 +50%), Founded (2014)

Risk summary cards:
- Commercial Risk: Low (score 9.3/10) — green
- Payment Capacity: 595,541 RON — blue
- Insolvency Rating: Class A (0.04%) — green
- Legal Risk: Low — green

FREE sections (fully visible):
- Company Details (CUI, registration number, CAEN code, status)
- Fiscal Information (VAT payer, ANAF status, no debts)
- Address
- Basic Contact (phone, email, website)

PAID sections (show blurred/locked with upgrade prompt):
- Financial Analysis (blurred chart) → "Unlock with Esențial"
- Court Cases (blurred list, "30 cases found") → "Unlock with Esențial"
- Shareholder Network (blurred graph) → "Unlock with Esențial"
- Sector Comparison (blurred chart) → "Unlock with Esențial"

### 5. Upgrade Modal
- Headline: "Get the full picture on any Romanian company"
- What you unlock: Financial deep-dives, Court records, Shareholder connections, Monitoring alerts, Sector benchmarks
- Pricing: €17/month (billed €204/year) OR €22/month (billed monthly)
- CTA: "Start Esențial — €17/month" → mock credit card form
- Small text below: "Questions? Talk to us" (NOT the primary path)

## Design Direction
- Colors: Dark navy (#0A0E1F) + white + electric blue (#3D7FFF) + emerald green (#10B981) for positives + amber for warnings
- Font: Inter from Google Fonts CDN
- Style: Stripe meets Crunchbase — professional, data-forward, trustworthy
- Romanian text where it adds authenticity, English OK for prototype
- Mobile responsive

## UX Principles
1. Speed to value — company data visible within 60 seconds
2. Show, don't gate — locked content shows blurred, not hidden
3. Self-service first — no consultant required for Esential tier
4. Data is the hero — let the depth speak for itself

## Deliverable
Multiple linked HTML files. All CSS in <style> tags or inline. Vanilla JS only. CDN links OK for: Chart.js (charts), Lucide (icons), Inter font. Should feel like a real product, not a wireframe. Make it beautiful.

File structure:
- index.html (landing)
- signup.html (signup flow with steps)
- dashboard.html (post-signup: search first company)
- company.html (company profile with free/locked sections)
