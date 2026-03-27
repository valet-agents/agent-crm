# CRM Agent

A simple CRM agent backed by Airtable. Bootstraps a Contacts table automatically and processes natural language to create, find, and update contacts. Designed as a template to extend with channels like SMS, email, or Slack.

## Prerequisites
- An [Airtable](https://airtable.com) account with a personal access token (`data.records:read`, `data.records:write`, `schema.bases:read`, `schema.bases:write` scopes)
- A base named **Agent-CRM** in your Airtable workspace (the agent will create the Contacts table automatically)

<table>
  <tr>
    <td><strong>CONNECTORS</strong></td>
    <td><code>airtable-mcp</code></td>
  </tr>
  <tr>
    <td colspan="2" align="center">
      <br />
      <a href="https://dashboard.valet.dev/setup/configure?from=github.com/valet-agents/agent-crm">
        <img src="https://raw.githubusercontent.com/valet-agents/agent-crm/main/.github/deploy-button.svg" alt="Deploy Agent →" height="40" />
      </a>
      <br /><br />
    </td>
  </tr>
</table>
