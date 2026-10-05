# Lead Generation Agency OS

Operating system for a lead-generation agency on a retainer plus commission model.

Stack named in this repo: HubSpot, Twilio, Claude, Lemon Squeezy.

This repo is the blueprint and the HubSpot setup lists. It is not PipelineEdge OS (`os.pipelineedge.in`). Do not copy retainer amounts, commission rates, or client books into call scripts.

## Map

| Path | What it is |
| --- | --- |
| [docs/01-pipelines.md](docs/01-pipelines.md) | Five HubSpot deal pipelines and stages |
| [docs/02-properties.md](docs/02-properties.md) | Contact, company, deal, ticket, and date properties |
| [docs/03-workflows.md](docs/03-workflows.md) | Nine workflow specs |
| [docs/04-automation.md](docs/04-automation.md) | Capture, reply, stage, Twilio, Lemon Squeezy, reporting logic |
| [docs/05-dashboard.md](docs/05-dashboard.md) | Monthly KPI sections and formulas |
| [docs/06-client-report.md](docs/06-client-report.md) | Client monthly report template |
| [docs/07-workflow-map.md](docs/07-workflow-map.md) | Stage path from capture to upsell |
| [hubspot/pipelines.csv](hubspot/pipelines.csv) | Pipeline and stage list |
| [hubspot/properties.csv](hubspot/properties.csv) | Properties to create |

## Operating path

Lead capture → qualification → discovery call booked → proposal sent → negotiation → closed won → retainer active → renewal check → monthly reporting → upsell.

## Rules

- HubSpot is the CRM. Do not add Salesforce, Zoho, or Pipedrive objects here.
- Commission and retainer fields live on deals and the billing pipeline. They are not spoken on calls.
- Lemon Squeezy is the billing source named in this blueprint. Payment success and failure update HubSpot; they do not send from the dialler.
- Twilio SMS and WhatsApp in this blueprint are follow-up only, after a no-reply or a missed meeting. Nothing auto-sends without the workflow conditions below.
