# Workflow Automation — client case studies

**Project type:** Sanitized client case studies
**Evidence sources:** completed Upwork contracts (5.0), completed Fiverr orders and reviews, historical account audit
**Status:** delivered

Umbrella repository for automation engagements that are real but individually
small — the workflow builds, the integrations, and the "it worked last week and
it doesn't now" jobs.

---

## Engagements

### n8n workflow build — Upwork

A workflow designed and built to the client's requirements and delivered ahead of
schedule. Contract closed at **5.0**. The client's public review:

> "Delivered a clean, efficient solution ahead of schedule."
> — Upwork client, November 2025

**Tools.** n8n · APIs · webhooks

### Google Contacts backup automation — Upwork

Scheduled backup workflow in n8n.
→ Full write-up: **[n8n-google-contacts-backup](https://github.com/skmalikllc/n8n-google-contacts-backup)**

### Contact sync between two platforms — Upwork

iCloud ↔ Google Contacts reconciliation.
→ Full write-up: **[icloud-google-contacts-sync](https://github.com/skmalikllc/icloud-google-contacts-sync)**

### Make.com + Airtable automation failure — troubleshooting

An automation that had stopped firing. The scenario itself was fine; the fault was
a **stale Airtable View ID** — the view the scenario pointed at had been replaced,
so the trigger was watching something that no longer existed.

This is the shape most "broken automation" jobs take. Nothing is wrong with the
logic. Something it refers to moved, and the platform's error message does not say
so. The fix is tracing the reference, not rebuilding the workflow.

**Tools.** Make.com · Airtable

### Zapier / n8n / Make automation — Fiverr

Automation orders delivered through Fiverr, with client reviews recorded against
that service in the account history.

**Tools.** Zapier · n8n · Make.com

---

## Implementation notes

Workflow exports, scenario blueprints, node chains, API keys and webhook URLs are
intentionally omitted — those belong to the clients whose accounts they run in.
Where a detail is not documented, it is left out rather than reconstructed.

## Privacy

No client names, no credentials, no webhook secrets, no workflow exports.

## Related

- [contact-dedupe-mcp](https://github.com/skmalikllc/contact-dedupe-mcp) — open-source tool, the data-cleaning half of this work
- [automation-portfolio](https://github.com/skmalikllc/automation-portfolio)
