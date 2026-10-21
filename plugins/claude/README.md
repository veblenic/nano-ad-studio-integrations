# Nano Ad Studio for Claude Code

This plugin connects Nano tools and adds the `nano-ad-workflow` skill.
The skill covers catalog selection, estimates, planning, plan review, rendering, and output retrieval.
A Nano Business plan is required.

## Install

Run this command with Claude Code 2.1.292 or later:

```sh
claude plugin install nano-ad-studio-assistant --marketplace https://nanoadstudio.com/integrations/claude/marketplace.json
```

Then complete these steps:

1. Start Claude Code and open `/mcp`.
2. Select Nano, sign in, and approve the Nano tools connection.
3. Ask: "Use Nano to list my brands."

Nano presents one permission grant for its tools.
Your assistant stores the connection. You do not copy an API key or edit a file.
Planning and rendering spend Credits and require your approval.

For Claude Code 2.1.224–2.1.291, use these commands instead:

```sh
claude plugin marketplace add https://nanoadstudio.com/integrations/claude/marketplace.json
claude plugin install nano-ad-studio-assistant@nano-ad-studio
```

See [Claude plugin installation](https://code.claude.com/docs/en/discover-plugins) and [OAuth connections](https://code.claude.com/docs/en/mcp#authenticate-with-remote-mcp-servers).

## Use and remove

Invoke `/nano-ad-studio-assistant:nano-ad-workflow` or ask Claude to use Nano.
If you already connected Nano through MCP, use the standalone skill to avoid duplicate tools.
Disconnect the assistant in [Nano Developer settings](https://nanoadstudio.com/settings/developer) to revoke its access.
Remove the plugin with `claude plugin uninstall nano-ad-studio-assistant@nano-ad-studio`.

This package includes no credentials, executable scripts, or hooks.
Nano hosts its own marketplace. It does not claim an Anthropic directory listing or verification.
