# MASTER PRD PROMPT
## Website for Greeja Organic Solar Energy Pvt. Ltd. (Dr. Rajesh Kumar — UTL Solar Partner, Muzaffarpur)

> **How to use this document:** This is a complete Product Requirements Document written *as a prompt*. Paste the entire thing into an AI website builder (or hand it to a developer/designer) to generate the site in one go. It covers business context, goals, sitemap, page-by-page content, features, the solar calculator logic, design direction, SEO, and technical requirements.

---

## 1. ROLE & OBJECTIVE (for the AI/Developer)

You are a senior web designer and conversion copywriter. Build a **multi-page, mobile-first, fast-loading website** for a solar EPC (Engineering, Procurement, Installation) business. The website's core job is to:

1. **Educate** homeowners and businesses in Muzaffarpur (Bihar) and nearby towns on why solar is better than grid electricity — lower bills, energy independence, environmental benefit.
2. **Build trust** in Dr. Rajesh Kumar and Greeja Organic Solar Energy Pvt. Ltd. as the authorized UTL Solar dealer/installer.
3. **Convert visitors into leads** via an interactive electricity-bill/solar-savings calculator, WhatsApp, callback requests, and consultation bookings.
4. **Rank locally** on Google for solar-related searches in Muzaffarpur and surrounding districts.

---

## 2. BUSINESS CONTEXT

| Field | Detail |
|---|---|
| **Business Name** | Greeja Organic Solar Energy Pvt. Ltd. |
| **Founder/Owner** | Dr. Rajesh Kumar |
| **Brand Partner** | UTL Solar (authorized dealer/installer) |
| **Primary Location** | Muzaffarpur, Bihar |
| **Service Area** | Muzaffarpur city + nearby towns/districts (e.g., Hajipur, Vaishali, Motihari, Sitamarhi, Darbhanga, Samastipur — confirm exact list with client) |
| **Core Services** | Solar panel sales, rooftop installation (residential/commercial/industrial), solar water heaters, solar pumps, AMC (annual maintenance contracts), subsidy/documentation assistance, net-metering support |
| **Core Message** | Solar = lower electricity bills + clean/green energy + energy independence |

---

## 3. WEBSITE GOALS (in priority order)

1. Generate qualified leads (site visits, calculator submissions, WhatsApp chats, calls).
2. Educate visitors on solar economics — payback period, savings, subsidies.
3. Establish authority/trust (certifications, UTL partnership, completed projects, testimonials).
4. Rank on local search ("solar company in Muzaffarpur", "UTL solar dealer Muzaffarpur", etc.).
5. Make it dead simple for a non-technical visitor to understand their potential savings in under 60 seconds.

---

## 4. TARGET AUDIENCE

- Homeowners with high monthly electricity bills (₹2,000+) wanting to cut costs.
- Small business/shop owners (frequent power cuts, diesel generator costs).
- Farmers interested in solar water pumps.
- Environmentally conscious families.
- Housing societies / commercial building owners looking at larger installations.
- Mostly Hindi/Hinglish-speaking local audience — content should be simple, non-jargon-heavy, available in **English + Hindi** (bilingual toggle recommended).

---

## 5. SITEMAP (Multi-Page Structure)

1. **Home**
2. **About Us** (Dr. Rajesh Kumar's story, company mission, UTL partnership)
3. **Why Solar?** (education page — solar vs grid electricity vs other green energy)
4. **Services**
   - Residential Rooftop Solar
   - Commercial & Industrial Solar
   - Solar Water Pumps
   - Solar Water Heaters
   - AMC / Maintenance
   - Net Metering & Subsidy Assistance
5. **Solar Savings Calculator** (flagship interactive tool — see Section 7)
6. **Products** (UTL panels, inverters, batteries — specs & brochures)
7. **Projects / Gallery** (before-after photos, case studies by area)
8. **Government Subsidy Info** (PM Surya Ghar Muft Bijli Yojana details, how to apply)
9. **Testimonials / Reviews**
10. **Blog** (SEO content — see Section 10)
11. **FAQ**
12. **Contact Us** (form, map, WhatsApp, phone, service area list)

---

## 6. PAGE-BY-PAGE CONTENT BRIEF

### Home Page
- Hero section: strong headline (e.g., "Cut Your Electricity Bill by up to 90% — Go Solar with Muzaffarpur's Trusted UTL Partner") + subheadline + CTA button "Calculate My Savings"
- Trust bar: "Authorized UTL Solar Dealer," years of experience, number of installations, cities served
- Quick 3-step "How It Works" (Consultation → Installation → Start Saving)
- Embedded mini calculator widget (bill amount → instant estimated savings) linking to full calculator page
- Why Solar snapshot (3-4 icon benefits: Save Money, Government Subsidy, Clean Energy, 25-Year Lifespan)
- Featured services grid
- Testimonials carousel
- Recent projects strip
- Service area map/list (Muzaffarpur + nearby cities)
- Final CTA: WhatsApp / Book Free Site Visit

### About Us
- Dr. Rajesh Kumar's background, credentials, why he started Greeja Organic Solar Energy
- Company mission/vision (organic + solar = sustainability angle)
- UTL Solar partnership badge/explanation
- Team, certifications, licenses
- Milestones (installations completed, MW installed, years in business)

### Why Solar? (Education Hub — core persuasion page)
- Solar vs. grid electricity: cost comparison over 25 years
- Solar vs. diesel generators (for shopkeepers)
- Environmental benefits (CO₂ offset in simple terms, e.g., "equivalent to planting X trees")
- How net metering works (sell excess power back to grid)
- Government subsidy explainer
- Simple explainer video/infographic on how solar panels work
- Link to Calculator with CTA

### Services (each service = own subpage)
- What's included, ideal customer, price range/starting price (if shareable), process, warranty, CTA to calculator or contact

### Solar Savings Calculator (see Section 7 — detailed spec)

### Products
- UTL panel models, wattage options, inverter/battery options, spec sheets, downloadable brochure PDFs

### Projects/Gallery
- Filterable by location/type (residential/commercial/pump), before-after photos, capacity installed, customer quote

### Government Subsidy Info
- PM Surya Ghar Yojana breakdown, eligibility, subsidy amount by system size, application process, how Greeja Organic Solar helps with paperwork

### Testimonials
- Photo/video testimonials, city-wise, star ratings, Google review embed

### Blog
- SEO articles (see Section 10)

### FAQ
- "How much does solar cost in Bihar?", "How long does installation take?", "What's the subsidy amount?", "Does solar work during power cuts?", "What's the maintenance cost?", "How long do panels last?"

### Contact Us
- Form (Name, Phone, City, Monthly Bill, Roof Type — pre-qualifies leads)
- Click-to-WhatsApp button (floating on all pages)
- Click-to-call button
- Google Map embed (office location, Muzaffarpur)
- List of serviceable cities/pin codes

---

## 7. FLAGSHIP FEATURE: Solar Savings & Electricity Bill Calculator

This is the **most important feature** on the site. Build it as an interactive, multi-step calculator (React component or embedded JS widget).

### Step 1 — Input
- Current average monthly electricity bill (₹) **[required, simple slider or number input]**
- OR: Monthly units consumed (kWh) — toggle between "I know my bill" / "I know my units"
- City/location (dropdown: Muzaffarpur + nearby towns — affects sunlight-hour assumptions)
- Roof type/area available (optional, for system-size estimate): Rooftop (RCC) / Tin Shed / Open Land
- Property type: Home / Shop / Farm / Factory

### Step 2 — Calculation Logic (transparent formulas)
- Estimate recommended system size (kW) based on monthly units ÷ average sunlight hours/day (use Bihar average ~4.5–5 peak sun hours) ÷ days in month
- Estimated system cost (₹/kW installed — configurable rate, editable by client)
- Applicable government subsidy (per PM Surya Ghar Yojana slabs — up to 3kW residential subsidy tiers; make this a configurable variable since subsidy amounts change)
- Net cost after subsidy
- Estimated monthly savings (new reduced bill vs. old bill)
- Payback period (net cost ÷ monthly savings, converted to years)
- 25-year total savings projection (accounting for expected electricity tariff inflation, e.g., 3-5%/year — configurable)
- Approximate CO₂ offset per year (kg) and "equivalent trees planted" for the environmental hook

### Step 3 — Output (visual, shareable)
- Clear result card: "Your Estimated Monthly Savings: ₹X | Payback Period: Y years | 25-Year Savings: ₹Z"
- Simple bar/line chart: Old bill vs. New bill vs. Savings over time
- Recommended system size and estimated cost breakdown (before/after subsidy)
- CTA: "Get Exact Quote — Book Free Site Visit" (opens lead form pre-filled with calculator data) + WhatsApp share button

### Technical Notes
- All assumptions (sunlight hours, tariff rate, subsidy %, cost/kW) should live in a single config object so Dr. Kumar's team can update them as prices/subsidies change without touching code.
- Mobile-first, large touch-friendly sliders.
- No login required; capture lead info only at the final "Get Exact Quote" step (progressive profiling, not upfront friction).
- Store submitted calculator leads in a simple backend/Google Sheet/CRM integration.

---

## 8. ADDITIONAL FEATURE IDEAS (beyond the calculator)

- **Floating WhatsApp Chat Button** on every page (direct to business WhatsApp number)
- **"Book a Free Site Visit"** sticky CTA button
- **Live Google Reviews widget** embedded on homepage
- **Subsidy Eligibility Checker** (simple yes/no quiz: roof type, ownership, sanctioned load)
- **EMI/Financing Calculator** (if loans/EMI options offered) — monthly EMI vs. monthly savings comparison
- **Interactive System Size Recommender** (input appliances used → suggests kW system)
- **Service Area Map** — pin-drop map showing all cities covered, with "Check if we service your area" search
- **Downloadable Solar Guide PDF** (lead magnet — "Free Guide: How to Save on Electricity with Solar in Bihar" in exchange for phone number)
- **Before/After Case Study Cards** with real ₹ savings numbers per project
- **Live Chatbot** for FAQs (can be simple rule-based)
- **Referral Program page** ("Refer a friend, earn ₹X")
- **Seasonal/Festival Offer Banner** (configurable promo banner)
- **Trust badges**: UTL Authorized Dealer, MNRE-approved vendor status (if applicable), ISO certs if any
- **Video testimonials / installation timelapse videos**
- **Multi-language toggle** (English/Hindi)
- **Blog with local SEO content** (see below)
- **"Compare Solar Brands" page** if positioning UTL against generic competitors
- **Emergency/Power-cut angle content**: solar + battery backup messaging for Bihar's frequent outages

---

## 9. DESIGN DIRECTION

- **Palette**: Sunlight yellow/orange + deep green (organic/eco cue) + white/dark navy for contrast and trust; avoid generic "corporate blue" cliché.
- **Typography**: Clean, highly readable sans-serif; large numerals in the calculator for impact.
- **Imagery**: Real installation photos in Muzaffarpur (not generic stock solar panels in a US suburb) — authenticity matters for local trust.
- **Tone**: Simple, reassuring, non-jargon. Assume first-time solar buyers.
- **Mobile-first**: Majority of visitors will be on mobile; calculator and CTAs must work flawlessly on small screens.
- **Speed**: Optimize images, lazy-load galleries, target <3s load time.

---

## 10. SEO & CONTENT STRATEGY

- **Primary keywords**: "solar company in Muzaffarpur," "UTL solar dealer Muzaffarpur," "rooftop solar installation Bihar," "solar subsidy Bihar," "reduce electricity bill solar Muzaffarpur"
- **Local SEO**: Google Business Profile integration, city-specific landing pages/sections for each nearby town served, embedded map, NAP (Name/Address/Phone) consistency
- **Blog topics** (2-4 to start):
  1. "How Much Can You Save on Your Electricity Bill with Solar in Muzaffarpur?"
  2. "PM Surya Ghar Yojana: Complete Subsidy Guide for Bihar Homeowners"
  3. "Solar vs. Diesel Generator: What's Cheaper for Bihar Shopkeepers?"
  4. "5 Signs Your Home Roof Is Ready for Solar Panels"
- **Schema markup**: LocalBusiness, FAQ, Review/AggregateRating schema

---

## 11. TECHNICAL REQUIREMENTS

- Multi-page site (not single-page scroll) — separate URLs per page for SEO
- Framework suggestion: Next.js/React (or WordPress if client needs easy self-editing) — confirm with developer
- CMS-editable: services, pricing assumptions, testimonials, blog, gallery (client shouldn't need a developer to update text/images)
- Forms integrate with email/CRM/Google Sheets/WhatsApp Business API
- Fully responsive (mobile/tablet/desktop)
- Basic analytics (Google Analytics/GTM) + conversion tracking on calculator submissions and form fills
- SSL, fast hosting, image optimization
- Accessibility basics (alt text, readable contrast ratios)

---

## 12. OPEN QUESTIONS FOR CLIENT (Dr. Rajesh Kumar) BEFORE BUILD

- Exact list of serviceable cities/districts near Muzaffarpur
- Current subsidy rates and system cost per kW to hardcode into calculator config
- Preferred WhatsApp Business number and contact details
- Availability of real installation photos/testimonials/certifications
- Whether Hindi-language version is required at launch or phase 2
- Whether financing/EMI partnerships exist (for the EMI calculator feature)
- Logo, brand colors, and any existing brand guidelines

---

*End of PRD. This document can be pasted directly into an AI website builder or shared with a design/dev team as the single source of truth for scope.*
