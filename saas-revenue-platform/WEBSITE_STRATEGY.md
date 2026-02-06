# Website Strategy & Architecture

## Website Goals

1. **Educate** visitor about the problem and solution in <2 minutes
2. **Capture** email/phone for demo booking or free trial signup
3. **Convert** visitor to trial user or paying customer
4. **Segment** for follow-up (which tier are they interested in?)

---

## Site Architecture

```
www.revenueplatform.com/
├── / (Home/Landing Page)
├── /how-it-works
├── /pricing
├── /for-[segment] (HVAC, Real Estate, Clinics)
├── /case-studies
├── /blog
├── /demo (Interactive dashboard)
├── /contact
├── /app/signup (Free trial)
└── /app/login
```

---

## Page-by-Page Strategy

### 1. HOME (Landing Page)

**Goal:** Get visitor to "schedule demo" or "start free trial" within 2 minutes

**Sections:**

#### Hero (First scroll)
**Headline:** "Stop Losing Money on Phone Calls You Don't Understand"
**Subheading:** "The only platform service businesses need to track call revenue, automate follow-up, and prove ROI in real-time."
**Visual:** Screenshot of dashboard with red circle around key metric ($12,450 in revenue today)
**CTA Button:** "See Your Revenue Dashboard" → /demo or /app/signup

---

#### Segment Quick Select (Just below hero)
**Headline:** "Are you...?"
**Buttons:** 
- HVAC/Plumbing
- Real Estate
- Clinic/Medical
- Other Service Business

→ Each goes to /for-[segment] for custom messaging

---

#### Problem Section
**Headline:** "You're Already Getting Calls. You Just Don't Know Their Value."
**3 Cards:**
1. **Icon: Phone + ?** "Where did that call come from?" → No visibility into ROI
2. **Icon: Missed call** "Why did they disappear?" → Missed callbacks, lost deals
3. **Icon: Dollar + ?** "Is marketing actually working?" → Can't prove impact

**Social proof below:** "Trusted by 150+ service businesses in HVAC, plumbing, real estate, and medical"

---

#### Solution Section
**Headline:** "See Every Call. Track Every Deal. Prove Every Dollar."
**3 Key Features (with visuals):**

1. **Call Tracking & Attribution**
   - Visual: Screenshot of call log with source, duration, outcome
   - Copy: "Every inbound call automatically recorded, transcribed, and attributed to source"
   - CTA: "See how tracking works" → /how-it-works

2. **Automated Follow-Up & Booking**
   - Visual: SMS/email templates, calendar booking
   - Copy: "Missed calls auto-texted. Appointments auto-booked. No manual work."
   - CTA: "See automation in action" → /demo

3. **Revenue Dashboard**
   - Visual: Key metrics (calls today, revenue, conversion rate, lost opportunities)
   - Copy: "Real-time visibility into revenue impact. Know what's working."
   - CTA: "Explore the dashboard" → /demo

---

#### Social Proof / Case Study Carousel
**Headline:** "Service Businesses Are Already Saving Time & Money"

**3 Case Studies (carousel):**
1. **HVAC Company, Chicago**
   - "We were losing $4K/month in missed callbacks."
   - "Now we recover 90% of leads automatically."
   - "ROI: Paid for itself in 2 weeks."

2. **Real Estate Team, Austin**
   - "We close 20% more deals since automating follow-up."
   - "Saves our team 10+ hours per week on admin."
   - "Already upsold to Tier 3 for AI optimization."

3. **Medical Clinic, Denver**
   - "Missed calls were costing us $8K/month in lost appointments."
   - "Now we auto-confirm and catch rescheduling."
   - "Worth every penny."

---

#### Pricing Preview
**Headline:** "Simple Pricing. No Surprises."

**3 Pricing Cards (simple overview):**
- **Tier 1:** $1,500/mo — Dashboard + call tracking
- **Tier 2:** $2,000/mo — + Automation + booking
- **Tier 3:** $3,000/mo — + AI + optimization + support

**Button:** "See Full Pricing" → /pricing

---

#### Bottom CTA Section
**Headline:** "Ready to See Your Real Revenue?"
**Subheading:** "14-day free trial. No credit card. See your first insights in 48 hours."

**2 Buttons (side-by-side):**
- "Start Free Trial" → /app/signup
- "Schedule Demo" → Calendly embed

---

### 2. /HOW-IT-WORKS

**Goal:** Show the workflow and how the platform fits into their day

**Sections:**

#### Step 1: Call Comes In
- Visual: Phone ringing, incoming call
- Text: "Your customer calls. We capture it. Automatically."
- Details:
  - Virtual phone number you forward to us
  - Or we integrate with existing PBX
  - Call recorded, transcribed, stored

#### Step 2: Dashboard Shows It
- Visual: Dashboard updates in real-time
- Text: "You see every call. Source. Duration. Outcome."
- Details:
  - Call source (Google, Facebook, Direct, Referral, etc.)
  - Caller info (name, number, history)
  - Call recording/transcript

#### Step 3: Automation Kicks In
- Visual: SMS/email being sent automatically
- Text: "Missed call? Auto-text. Not responsive? Auto-email. Lead gets booked? Calendar updates."
- Details:
  - SMS follow-up templates (customizable)
  - Email templates (with booking link)
  - Appointment auto-confirmation
  - Leads without callbacks auto-scored

#### Step 4: Revenue Attribution
- Visual: Deal closed, checkmark, revenue added to dashboard
- Text: "Deal closes. Revenue linked to call. Dashboard updates."
- Details:
  - You log deal in dashboard (or CRM integrates)
  - Revenue tied to original call
  - Channel ROI becomes visible

#### Step 5: You Optimize
- Visual: Reports, trends, recommendations
- Text: "See what's working. Double down on high-ROI channels."
- Details:
  - Channel ROI analysis (Google vs Facebook vs referral)
  - Best times to call (AI recommendations)
  - Team performance (who closes fastest)

---

### 3. /FOR-[SEGMENT] (e.g., /for-hvac)

**Goal:** Show segment-specific value and use cases

**Structure:** Same as home, but:
- Headline tailored: "HVAC Companies: Stop Guessing on Marketing ROI"
- Problem section uses HVAC pain points ("Google ads working?" "Roofer calling back leads?")
- Case study from HVAC company
- CTAs mention HVAC: "Schedule HVAC demo"

**Repeat for:** /for-realtor, /for-clinic, /for-lawyer, /for-other

---

### 4. /PRICING

**Goal:** Make it easy to compare tiers and choose

**Layout:**

#### Pricing Cards (3-column, desktop; stacked mobile)

| Tier 1 | Tier 2 | Tier 3 |
|--------|--------|--------|
| **Dashboard + Tracking** | **Full Automation** | **AI + Optimization** |
| $1,500/month | $2,000/month | $3,000/month |
| ✓ Call tracking | ✓ All of Tier 1 | ✓ All of Tier 2 |
| ✓ Dashboard | ✓ SMS/email follow-up | ✓ AI call analysis |
| ✓ Call recording | ✓ Booking system | ✓ Predictive scoring |
| ✓ Basic reporting | ✓ Lead scoring | ✓ Smart routing |
| | ✓ Appointment confirmation | ✓ Advanced attribution |
| | | ✓ Optimization recommendations |
| | | ✓ Priority support |
| [Start Free Trial] | [Start Free Trial] | [Schedule Demo] |

#### FAQ Below
- "Can I change tiers?"
- "What if I need custom features?"
- "Do you offer annual pricing discounts?"
- "What's included in setup?"
- "Can I integrate with my existing CRM?"

---

### 5. /CASE-STUDIES

**Goal:** Build credibility with social proof

**Layout:** 3-4 detailed case studies (one per row)

**Each case study includes:**
- Company name, location, industry
- Challenge (what they were losing)
- Solution (how they used our platform)
- Result (specific metrics: revenue recovered, time saved, deals closed)
- Quote from owner
- Photo/video testimonial (if possible)
- "Ready to get similar results?" CTA

**Example:**
> **HVAC Company, Chicago**
> 
> **Challenge:** Getting 50+ calls/month but couldn't track where they came from or which ones turned into revenue. Marketing spend felt like gambling.
> 
> **Solution:** Deployed call tracking + automated follow-up. Set up 3 SMS templates for missed calls.
> 
> **Result:**
> - Recovered $4,000/month in missed callback revenue
> - Reduced admin time by 8 hours/week
> - Improved marketing ROI visibility by 40%
> - Upsold to Tier 3 after 90 days
> 
> **Quote:** "We were losing money we didn't even know about. This platform made it impossible to ignore."

---

### 6. /BLOG

**Goal:** SEO + thought leadership + nurture leads

**Content Calendar (launch + ongoing):**

**Month 1 (Pre-launch):**
- "How to Track Call Revenue (And Why You're Probably Losing $10K/Month)"
- "The Hidden Cost of Missed Callbacks"
- "3 Real Estate Teams That Doubled Their Closing Rate"

**Ongoing:**
- Service business best practices
- Marketing ROI tips
- Customer spotlights
- Product updates

**Each post has:** CTA to free trial or demo

---

### 7. /DEMO (Interactive)

**Goal:** Let them play with a sample dashboard

**What they see:**
- Demo company: "ABC HVAC, Chicago"
- Last 30 days of simulated data:
  - 87 inbound calls
  - $45,320 in attributed revenue
  - 62% answer rate
  - Top source: Google Ads
  - Revenue per call: $521
  - Lost opportunities: $8,400 (missed callbacks)

**Interactive elements:**
- Click on a call to see details (source, transcription, outcome)
- Hover over charts to see trends
- Filter by source, date range, outcome
- See sample SMS follow-up automation
- See booking calendar with auto-filled appointments

**CTA after demo:** "Ready to see YOUR data?" → /app/signup

---

### 8. /CONTACT

**Goal:** Capture for high-touch sales (phone, email, web)

**Simple form:**
- Name
- Company
- Email
- Phone
- Company size (5-10, 10-50, 50+)
- Which tier are you interested in? (radio buttons: Tier 1/2/3)
- Preferred contact method (phone, email, calendar)
- Message (optional)

**On submit:**
- Thank you message
- Offer: "Schedule 30-min demo" (Calendly embed)
- Alternative: "Grab a free trial link"
- Set up follow-up email sequence

---

### 9. /APP/SIGNUP (Free Trial)

**Goal:** Get them into the platform

**Flow:**
1. Name + email + company
2. Choose phone number (we provide, or forward existing)
3. Import first leads (CSV or manual entry)
4. Set up SMS templates (pick from defaults)
5. Onboarding call scheduled (optional but encouraged)
6. Dashboard opens with first insights in 24-48 hours

---

## Design System

**Colors:**
- Primary: Clean blue (#0066CC)
- Accent: Success green (#00AA00)
- Text: Dark gray (#333333)
- Background: White + light gray (#F8F9FA)

**Typography:**
- Headlines: Bold, sans-serif (Montserrat or Inter)
- Body: Clean sans-serif (Inter, Roboto)
- Monospace for code/metrics (Courier, Monaco)

**Components:**
- Large buttons (CTA focus)
- Subtle shadows (modern, not skeuomorphic)
- Lots of whitespace (SaaS aesthetic)
- Icons for visual breaks (Feather, HeroIcons)

**Mobile-first responsive design**

---

## Lead Capture Strategy

### Funnels

**Path 1: Free Trial**
- Visit home → Click "Start Free Trial" → Signup form → App access → $0, see for 14 days

**Path 2: Demo Booking**
- Visit home → Click "Schedule Demo" → Calendly → 30-min call + demo + proposal

**Path 3: Case Study/Blog**
- Read blog post → Click "See if this applies to you" → Lead form → Add to email sequence → Demo offer

### Email Sequences

**Segment 1: Free trial signups**
- Day 0: Welcome, "Your first dashboard is ready"
- Day 2: "Here's what we found in your calls"
- Day 5: "You're saving time. Here's what you're missing without Tier 2"
- Day 10: "One week left in trial. Ready to switch to paid?"
- Day 14: "Your trial ends tomorrow. Keep your data and 20% off first 3 months"

**Segment 2: Demo bookers**
- Day 0: Confirmation email
- Day +1: "Questions before your demo?"
- Day +3: Follow-up "Your ROI opportunity" + pricing
- Day +7: "Still interested?" (re-engagement)

---

## Conversion Targets

- **Landing page → Free trial:** 5% conversion
- **Landing page → Demo booking:** 2% conversion
- **Free trial → Paid:** 25% conversion
- **Demo → Paid:** 40% conversion
- **Blended trial + demo:** 30% conversion to paid

---

## Launch Sequence

**Week 1:** Home page + pricing + one segment page (/for-hvac)
**Week 2:** Add case studies + blog (3 posts)
**Week 3:** Add demo page + /how-it-works
**Week 4:** Full site live + paid ads start

---

## Success Metrics

Track:
- Homepage bounce rate (target: <50%)
- Free trial signups per month
- Demo booking rate
- Free trial → paid conversion (target: 25%)
- Demo → paid conversion (target: 40%)
- Blended CAC (customer acquisition cost)
- LTV (lifetime value)
