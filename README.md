# Lead Capture Automation (n8n)

Captures form/webhook submissions, logs them to Google Sheets, and sends 
an instant email notification — a common real-world automation for 
freelancers, small businesses, and sales teams.

## Demo
[Link to your Loom video here]

## How it works
1. **Webhook** receives a POST request with lead data (name, email, message)
2. **Google Sheets** appends the lead as a new row with a formatted timestamp
3. **Gmail** sends an HTML-formatted notification email with the lead details

## Tech used
- n8n (self-hosted via Docker)
- Google Sheets API
- Gmail API
- Webhook trigger (works with any form tool: Typeform, custom forms, etc.)

## Workflow file
See `lead-capture-workflow.json` — importable directly into any n8n instance.

## Notes
Built as part of a self-directed learning path transitioning into 
AI Automation / VA work.