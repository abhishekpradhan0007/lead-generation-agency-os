# HubSpot pipelines

Create these five deal pipelines. Stages are in order.

## A. Lead Generation

Purpose: track outbound and inbound prospects from first touch to close.

Stages:
1. New Lead
2. Contacted
3. Qualified
4. Discovery Call Booked
5. Proposal Sent
6. Negotiation
7. Closed Won
8. Closed Lost
9. Nurture

Properties used on these deals:
- Lead Source
- Campaign Name
- Channel
- Persona
- ICP Fit Score
- Product/Service
- Last Outreach Date
- Next Action Date
- Deal Owner
- Estimated Deal Value

## B. Client Retainer

Purpose: track the client relationship after acquisition.

Stages:
1. Prospect
2. Proposal Accepted
3. Onboarding
4. Retainer Active
5. Campaign Live
6. Expansion Opportunity
7. At Risk
8. Churned

Properties:
- Retainer Amount
- Contract Start Date
- Contract End Date
- Renewal Date
- MRR
- Client Status
- Client Tier
- Account Owner
- Services Included
- Revenue Forecast

## C. Social Media / Content

Purpose: posting, approvals, and reporting.

Stages:
1. Content Brief Created
2. Brief Approved
3. Copy Written
4. Design Ready
5. Scheduled
6. Published
7. Engaged
8. Reported

Properties:
- Platform
- Content Type
- Campaign
- Post Status
- Engagement Rate
- Reach
- Clicks
- Leads Generated
- Approval Status

HubSpot deals are a poor fit for a content calendar. Use this pipeline only if content must sit next to revenue deals. Otherwise create the same stages as tasks or a custom object.

## D. Commission Tracking

Purpose: commission logic and payout status.

Stages:
1. Qualified Lead
2. Deal Created
3. Proposal Shared
4. Closed Won
5. Commission Calculated
6. Payout Pending
7. Paid
8. Disputed

Properties:
- Commission %
- Commission Amount
- Closed Revenue
- Invoice Reference
- Payout Date
- Pay Status
- Source Partner
- Referral Source

## E. Billing / Retainer

Purpose: payments and renewals from Lemon Squeezy.

Stages:
1. Payment Pending
2. Payment Received
3. Retainer Active
4. Renewal Due
5. Renewed
6. Payment Failed
7. Cancelled

Properties:
- Invoice Number
- Subscription ID
- Billing Cycle
- Renewal Amount
- Payment Status
- Last Payment Date
- Due Date
- Customer ID
