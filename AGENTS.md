This folder contains the source for a Skilled Agent originally built for the Valet runtime. Changes should follow the Skilled Agent open standard.

## Setup

### Connectors

- **airtable-mcp**: Airtable's official MCP server. Provides tools for managing bases, tables, records, and fields. The agent uses this for all CRM data operations — creating the CRM base/table, searching contacts, and updating records.

### Secrets

- **AIRTABLE_PERSONAL_ACCESS_TOKEN**: A personal access token from Airtable with read/write permissions on bases and records. Generate one at https://airtable.com/create/tokens — grant it `data.records:read`, `data.records:write`, `schema.bases:read`, and `schema.bases:write` scopes. Scope it to "All current and future bases" or the specific workspace where the CRM base should live.

### Channels

No channels are configured by default. This agent runs via the Valet console (`valet console`). See the "Extending This Agent" section in SOUL.md for ideas on adding SMS, email, Slack, or cron channels.

## Extending This Agent

This agent is a template. Here are common ways to extend it:

### Adding Channels
Attach a channel so the Agent-CRM can be updated from other surfaces:
- **SMS/Phone** (`twilio-webhook`): Text "Met Sarah at the conference, sarah@acme.com" to log a new contact
- **Email** (`agentmail`): Forward a business card photo or intro email to auto-create a contact
- **Slack** (`slack-mcp`): Use a Slack command to quickly look up or update contacts
- **Cron** (`cron`): Schedule a daily digest of contacts not reached out to in 30+ days