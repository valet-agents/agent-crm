# CRM Agent

Describe a contact in plain English. The agent finds or creates the record in [Airtable](https://airtable.com) and shows you exactly what changed.

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
