# Lead Capture Automation (n8n)

Captures form/webhook submissions, logs them to Google Sheets, and sends 
instant notifications to multiple channels (Email and Slack) — a common 
real-world automation for freelancers, small businesses, and sales teams.

## Demo
https://www.loom.com/share/b76a2d9fa37346748541d10966e78b8b

## How it works
1. **Webhook** receives a POST request with lead data (name, email, message)
2. **Google Sheets** appends the lead as a new row with a formatted timestamp
3. **Gmail** and **Slack** each receive the lead details in parallel — 
   demonstrating multi-channel notification from a single data source

## Tech used
- n8n (self-hosted via Docker)
- Google Sheets API
- Gmail API
- Slack API (Bot Token)
- Webhook trigger (works with any form tool: Typeform, custom forms, etc.)

## Customization
Notification channels are easily added or swapped — this same pattern 
supports Discord, Telegram, SMS, or any other destination with an n8n 
node or HTTP API.

## Workflow file
See `lead-capture-workflow.json` — importable directly into any n8n instance.

## Notes
Built as part of a self-directed learning path transitioning into 
AI Automation / VA work.
