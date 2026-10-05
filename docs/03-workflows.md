# Workflows

Build these in HubSpot. Enrollment must be once per object unless noted.

## A. Lead intake

Trigger: form submission or list import.

Actions:
- Create or associate company
- Create contact if missing
- Assign owner by source or region
- Add lead to Lead Generation pipeline at New Lead
- Set lifecycle stage to Lead
- Create task: review lead within 1 business hour
- Send internal email notification
- Enroll in email nurture

## B. Lead qualification

Trigger: contact tracked as engaged or replied.

Actions:
- Set lead score
- If score is above the threshold set on the workflow: move deal to Qualified and create a scheduling task
- If no response after 3 days: send follow-up SMS via Twilio and enroll in re-engagement

## C. Discovery call

Trigger: meeting booked or discovery task marked complete.

Actions:
- Create deal from contact and company if none exists
- Set stage to Discovery Call Booked
- Send confirmation email
- Create sales-rep task
- Enroll follow-up sequence
- Attach call-notes task

## D. Proposal

Trigger: deal stage is Proposal Sent.

Actions:
- Create follow-up task in 3 days
- If no response: send follow-up SMS and add nurture email
- If positive response: move to Negotiation and create proposal-deck task

## E. Closed won

Trigger: deal closed won.

Actions:
- Create client retainer deal
- Create onboarding checklist task
- Create billing record (Lemon Squeezy subscription id on the billing deal)
- Notify the team by email
- Send welcome email
- Set MRR and retainer fields from the closed deal
- Start the monthly report cycle task

## F. Renewal

Trigger: renewal date is within 30 days.

Actions:
- Notify account owner
- Send client check-in email
- Set churn-risk task
- Schedule renewal call
- Create renewal quote task

## G. Payment failure

Trigger: Lemon Squeezy payment failed or cancelled.

Actions:
- Update billing deal and client status
- Notify account owner
- Send payment retry email
- Mark service At Risk
- Create finance follow-up task

## H. Social content

Trigger: content brief approved.

Actions:
- Create copy and design tasks
- Move content stage to Scheduled when both tasks are done
- Reminder 24 hours before post time
- After publish, task to log engagement
- Add the row to the reporting list

## I. Re-engagement

Trigger: no reply after 7 days.

Actions:
- Send second follow-up email
- Send SMS via Twilio
- Move deal to Nurture
- Add contact to low-intent list
