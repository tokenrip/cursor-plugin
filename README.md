# Tokenrip

Tokenrip is the shared workspace your AI agents work from. Claude, ChatGPT, Codex, Grok and Muse work from here. You approve what needs you and see the rest get done. Your files, tables and to-dos live in one place every agent you use can reach, from any AI app, with the decisions you pinned read by each agent before it starts. Work started in one conversation is there for the next one, in any tool, and for the people you share it with.

With Tokenrip connected, your assistant can:
- Save documents, notes and plans to a workspace, with version history.
- Keep tables, such as a lead list, a budget or an itinerary, and add or update rows.
- Track tasks: add them, see what's still open, start one, and mark it done.
- Load a workspace and pick up where another agent left off, including what changed since it last looked and why.
- Read the decisions you pinned, so every agent follows them.
- Search your files.
- Share: send a file by link, or add someone to a workspace as a viewer or editor.

Each agent connects with its own key, and you can disconnect any one of them from your dashboard. Changes to files, tables and tasks record which agent made them and why. Tools that delete content or let more people see it are marked as such, so apps that support it ask you before they run. What you save stays yours: you can download any file and read everything through the API.

Sign in with your email and a six-digit code.

## What this plugin does

This Cursor plugin connects your agent to Tokenrip's MCP server with one sign-in. Once connected, the agent reads and saves work in your Tokenrip workspaces, reports what it did, and asks in Tokenrip before steps that need you. A request it leaves there waits until you decide.

The plugin holds the server's address and one skill, `tokenrip`, which tells your agent to work from your Tokenrip workspace first: load it before answering, save with a one-sentence reason, and ask you in Tokenrip before steps outside it. No key, no script.

## Install

1. Add Tokenrip from the app's plugin list.
2. Sign in when asked, with your email and the six-digit code Tokenrip sends you. A free account is created at sign-in if you don't have one.

Or add `https://api.tokenrip.com/mcp` as a custom MCP server.

If you added Tokenrip as a custom MCP server before, remove it first, so the agent sees one Tokenrip server.

## Use

Ask the agent to pick up work in a workspace, for example: "Pick up the launch plan where we left off." It loads the workspace, reads your instructions there, and saves what it makes back to it.

What the agent did, and what it asks you to decide, appears on your Dashboard: https://tokenrip.com/operator

## Your data

- **What Tokenrip keeps:** your account (your email address and any profile details you add); what you and your agents put in (files, tables, tasks, folders and workspaces); the name of each connected app and the access granted to it; and a record of what each agent did, when, and whether it worked, with the short reason an agent gives for a change.
- **Agent requests:** what each request sent and got back is kept for 30 days so problems can be found and fixed. Secrets are removed first, and the contents of files, tables and connection calls are never kept, only their size.
- **Protection:** all traffic is encrypted in transit with TLS. API keys, app tokens and browser sessions are stored only as hashes; keys for services you connect are stored encrypted.
- **Who receives it:** the providers that run Tokenrip (hosting, file storage, network, email, analytics and payments, each named in the privacy policy), and the people and apps you choose to share with.
- **No sale, no ads, no training:** Tokenrip doesn't sell data, doesn't show ads, and doesn't use your content to train AI models.
- **Deleting:** delete content from the dashboard or through an agent. Deleted files, folders and workspaces stay in the trash for 30 days and can be restored. To delete your account, email support@tokenrip.com from the account's address.

The privacy policy is the full statement: https://tokenrip.com/privacy

## Disconnecting

Uninstalling the plugin does not revoke Tokenrip's access. Revoke the agent on the Agents page: https://tokenrip.com/operator/agents

## Documentation

Connecting over MCP: https://docs.tokenrip.com/getting-started/mcp-server

## Support

Email support@tokenrip.com, or see https://tokenrip.com/support

## Terms

https://tokenrip.com/terms

## License

MIT. See [LICENSE](LICENSE).
