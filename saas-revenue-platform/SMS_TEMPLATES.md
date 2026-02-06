# SMS Automation Templates

## Implementation: Twilio API + Zapier or backend webhook

All SMS should include opt-out: "Reply STOP to unsubscribe"

---

## Template 1: Missed Call Alert (Immediate)

**Trigger:** Call comes in, customer misses it

**Recipient:** Customer's personal phone (configured in dashboard)

```
Hi [Name], you missed a call from [Caller Name] at [Time]. Tap to listen: [Recording Link] — RevenueLock
```

**Timing:** Immediate (send within 30 seconds of missed call)

**Conversion Goal:** Alert customer, preserve memory, prevent loss

---

## Template 2: Lead Follow-Up - First Attempt (5 min after missed call)

**Trigger:** Customer opts in + missed call

**Recipient:** Caller's phone number (if captured) OR Customer's team members

```
Hi [Caller Name], thanks for calling [Company]. I'm following up on your inquiry. Can you confirm interest in learning more about our services? Y/N
```

**Timing:** 5 minutes after call ends (if enabled)

**Conversion Goal:** Re-engage cold lead, get response, qualify

---

## Template 3: Lead Follow-Up - Reminder (1 hour later)

**Trigger:** No response to first SMS

**Recipient:** Caller's phone number

```
[Caller Name], just checking back in. Are you still interested in [Service Type]? Let me know or I'll try back tomorrow. Reply or call [Phone].
```

**Timing:** 1 hour after first message

**Conversion Goal:** Second touch, increase response rate

---

## Template 4: Booking Confirmation (Auto-triggered)

**Trigger:** Caller books appointment via SMS or web link

**Recipient:** Caller's phone number

```
Perfect! Your appointment is confirmed:
📅 [Date]
🕐 [Time]
📍 [Location or Zoom Link]
Confirm: [Yes/No Buttons or Reply "C"]
```

**Timing:** Immediately after booking

**Conversion Goal:** Confirmation, reduce no-shows

---

## Template 5: Booking Reminder (24 hours before)

**Trigger:** 24 hours before appointment

**Recipient:** Caller's phone number

```
Reminder: Your appointment is tomorrow at [Time]. See you at [Location]! Need to reschedule? [Reschedule Link] — [Company Name]
```

**Timing:** 24 hours before appointment

**Conversion Goal:** Reduce no-shows, increase attendance

---

## Template 6: Post-Booking Follow-Up (After appointment)

**Trigger:** Appointment marked complete in dashboard

**Recipient:** Caller's phone number

```
Thanks for coming in, [Name]! Have any questions? Reply here or call [Phone]. We'd love to help! — [Company]
```

**Timing:** 1-2 hours after appointment end time

**Conversion Goal:** Nurture relationship, answer questions, next steps

---

## Template 7: Win Message (After deal close)

**Trigger:** Deal marked won in dashboard

**Recipient:** Caller's phone number

```
Awesome! Your order is confirmed. Here's your ref #[Order ID]. You'll hear from us on [Next Step Date] with updates. Thanks, [Company]!
```

**Timing:** Within 2 hours of deal close

**Conversion Goal:** Celebrate, set expectations, confirmation

---

## Template 8: Survey / Feedback Request (Post-service)

**Trigger:** Service/appointment completed

**Recipient:** Caller's phone number

```
Quick question: How was your experience? Rate us 1-5: 1⭐ 2⭐ 3⭐ 4⭐ 5⭐ Your feedback matters! Reply with number.
```

**Timing:** 24-48 hours after service

**Conversion Goal:** Get NPS score, identify issues, improve

---

## Template 9: Referral Request (Happy customer)

**Trigger:** 5⭐ rating received OR 30 days after win

**Recipient:** Caller's phone number (happy customer)

```
[Name], you've been awesome! Know anyone who could use our services? Share this link & we'll both save 20%: [Referral Link] 🎁
```

**Timing:** 30 days after service completion

**Conversion Goal:** Generate referrals, grow customer base

---

## Template 10: Re-Engagement (Old lead, no response)

**Trigger:** Missed call + no response after 3 SMS attempts

**Recipient:** Caller's phone number

```
Last try: I know we've reached out a few times. Still interested in [Service]? If not, no problem. But let me know so I can stop pestering 😊 Y/N?
```

**Timing:** 5-7 days after original missed call

**Conversion Goal:** Qualify or disqualify lead

---

## Template 11: Industry-Specific: HVAC

**Trigger:** Customer calls HVAC company in winter

**Recipient:** Caller's phone number

```
Hi [Name]! Thanks for calling [HVAC Company]. We can get a technician to you [Same Day/Tomorrow] for emergency repair. Confirm? Y/N
```

---

## Template 12: Industry-Specific: Real Estate

**Trigger:** Lead inquires about property

**Recipient:** Caller's phone number

```
Perfect! I have 2 other showings lined up for that property this week. When works for you?
→ Today after 3pm
→ Tomorrow morning
→ This weekend
Reply with the time that works.
```

---

## Template 13: Industry-Specific: Medical Clinic

**Trigger:** Appointment booked

**Recipient:** Caller's phone number

```
Your appointment confirmed:
📅 [Date] at [Time]
📋 Dr. [Name]
📍 [Address]
Please arrive 10 min early. Insurance? [Link]
Questions? Call [Phone]
```

---

## Template 14: Time-Sensitive: Limited Offer

**Trigger:** High-value lead + no response to calls

**Recipient:** Caller's phone number

```
Last minute: We have an opening [Tomorrow at 2pm] for [Service]. Book now and get 20% off: [Link]. Expires in 2 hours.
```

**Timing:** When opening becomes available

**Conversion Goal:** Urgency, fill capacity, drive booking

---

## Template 15: Abandonment Recovery

**Trigger:** Lead started booking, didn't complete

**Recipient:** Caller's phone number

```
We noticed you started booking an appointment but didn't finish. Need help? [Reschedule Link] or call [Phone]. We're here! 😊
```

**Timing:** 30 minutes after abandonment

**Conversion Goal:** Recover lost bookings

---

## SMS Best Practices

### Timing
- **Missed call alert:** Immediate (<1 min)
- **Follow-up attempt:** 5 min
- **Reminder follow-up:** 1 hour
- **Second day follow-up:** Next day
- **Re-engagement:** 5-7 days later

### Length
- **Max 160 characters** = 1 SMS (international standard)
- **160-307 chars** = 2 SMS (charged as 2 messages)
- **Keep to <160 chars** when possible

### Tone
- **Friendly, conversational** (not corporate)
- **Use [Name]** when possible (personalization)
- **Include CTA** (Y/N, click link, reply)
- **Optional:** Emojis (📅 📞 ✅) for visual breaks

### Legal
- **STOP clause:** Always include opt-out option
- **Company name:** Include sender ID
- **Timing:** Avoid 9pm-8am unless urgent
- **Compliance:** Follow TCPA regulations (USA)

### Metrics to Track
- **Delivery rate** (target: >95%)
- **Read rate** (opening/view)
- **Response rate** (target: 10-30% for follow-up)
- **Conversion rate** (SMS → booking)
- **Opt-out rate** (should be <2%)

---

## Integration Instructions

### Option 1: Zapier + Twilio
1. Zapier Trigger: "New Call to Number"
2. Action: "Send SMS via Twilio"
3. Template: Use text from above
4. Delays: Use "Delay" action for timed sends

### Option 2: Make.com
Similar to Zapier, more visual workflow builder.

### Option 3: Custom Backend (Node.js + Twilio)
```javascript
const twilio = require('twilio');
const client = twilio(accountSid, authToken);

// Send SMS on missed call
async function sendMissedCallSMS(callerPhone, callerName) {
  await client.messages.create({
    body: `Hi ${callerName}, you missed a call. Call back: ${companyPhone}`,
    from: '+1-your-twilio-number',
    to: callerPhone
  });
}
```

---

## Example: Full Automation Flow

**Trigger:** Call comes in, customer doesn't answer

**Sequence:**
1. **0 min:** SMS Alert — "You missed a call from [Name]"
2. **5 min:** Follow-Up 1 — "Are you interested? Y/N"
3. **60 min:** Follow-Up 2 — "Just checking back in"
4. **24 hrs:** Final Touch — "Still interested? Let me know"

**Result:** Customer sees 4 SMS, has multiple ways to respond, high re-engagement.

---

## Cost Estimate (per customer per month)

- **SMS sent per missed call:** ~4 messages
- **Missed calls per month:** ~20
- **Total SMS:** 80-100/month
- **Cost per SMS:** $0.01-0.02 (Twilio)
- **Monthly SMS cost:** $1-2 per customer
- **Per company (50 customers):** $50-100/month for SMS

ROI: 1 recovered deal ($1K+) pays for months of SMS.
