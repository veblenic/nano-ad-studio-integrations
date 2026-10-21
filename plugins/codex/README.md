# Nano Ad Studio for Codex

This plugin connects Nano tools and adds the `nano-ad-workflow` skill.
The skill covers catalog selection, estimates, planning, plan review, rendering, and output retrieval.
A Nano Business plan is required.

## Install

Run these commands:

```sh
codex plugin marketplace add https://github.com/veblenic/nano-ad-studio-integrations.git
codex plugin add nano-ad-studio-assistant@nano-ad-studio
```

Then complete these steps:

1. Restart Codex and open its MCP connections.
2. Select Nano, sign in, and approve the Nano tools connection.
3. Ask: "Use Nano to list my brands."

Nano presents one permission grant for its tools.
Your assistant stores the connection. You do not copy an API key or edit a file.
Planning and rendering spend Credits and require your approval.

See [OpenAI's plugin guide](https://developers.openai.com/plugins/build/plugins) and [Codex MCP configuration](https://learn.chatgpt.com/docs/extend/mcp).

## Connect without the skill

Use these commands if you only need Nano's MCP tools:

```sh
codex mcp add nano_ad_studio --url https://api.nanoadstudio.com/mcp
codex mcp login nano_ad_studio
```

Use either the plugin or this direct connection to avoid duplicate tools.

## Remove

Disconnect the assistant in [Nano Developer settings](https://nanoadstudio.com/settings/developer) to revoke its access.
Remove the plugin with `codex plugin remove nano-ad-studio-assistant@nano-ad-studio`.

This package includes no credentials, executable scripts, or hooks.
Nano maintains its own marketplace. It does not claim an OpenAI directory listing or verification.
