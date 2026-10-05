# Automation logic

## A. Lead capture to pipeline

1. Form submission.
2. Create or update contact.
3. Create or update company from domain.
4. Map email, company domain, source, industry.
5. Assign owner by region or persona.
6. Create deal on Lead Generation at New Lead.
7. Internal notification.
8. Start outreach sequence.

Stop if Do Not Contact is true or consent is missing for the channel.

## B. Lead response

- Reply with interest: set Interested, move deal to Qualified, notify owner, create meeting task.
- No reply: phase-2 email on day 3, SMS on day 5, Nurture on day 7.

## C. Sales stage

- Discovery booked: deal at Discovery Call Booked, set next action.
- Solution accepted: Proposal Sent.
- Closed won: create retainer record, set MRR and contract dates.
- Closed lost: add to reactivation list, stamp last touched.

## D. Twilio

- No reply after 3 business days: SMS follow-up.
- Missed meeting: reminder SMS.
- Qualified lead: SMS or WhatsApp confirming the meeting.

Do not send if Do Not Contact is set. Do not include price, retainer, or commission in the message.

## E. Lemon Squeezy

- Payment success: client status Active, billing deal Retainer Active, write subscription id and MRR.
- Payment failed: billing alert, email, task to finance owner, service At Risk.

## F. Reporting

Once a month:
- Pull deal stage counts and amounts.
- Compare expected revenue to closed revenue.
- Refresh the dashboard in docs/05-dashboard.md.
- Draft the client report from docs/06-client-report.md. A human sends it.
