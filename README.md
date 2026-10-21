# Nano Ad Studio integrations

Connect Claude Code or Codex to Nano Ad Studio tools and the `nano-ad-workflow` skill.
A Nano Business plan is required.
Sign in to Nano once and approve one grant for its tools.
The assistant can read your catalog, estimate Credits, plan ads, review plans, render approved ads, and retrieve outputs.
Planning and rendering spend Credits and require your approval.

## Claude Code

With Claude Code 2.1.292 or later, run:

```sh
claude plugin install nano-ad-studio-assistant --marketplace https://nanoadstudio.com/integrations/claude/marketplace.json
```

Open `/mcp`, select Nano, and complete sign-in.
For older clients, read the [Claude Code instructions](plugins/claude/README.md).

## Codex

Run these commands:

```sh
codex plugin marketplace add https://github.com/veblenic/nano-ad-studio-integrations.git
codex plugin add nano-ad-studio-assistant@nano-ad-studio
```

Restart Codex, select Nano in its MCP connections, and complete sign-in.
Read the [Codex instructions](plugins/codex/README.md) for a direct MCP connection without the skill.

## Check access

Ask your assistant: "Use Nano to check my Credits and list my brands. Do not plan or render an ad."
An empty brand list is valid. A saved installation alone does not confirm access.
Disconnect an assistant in [Developer settings](https://nanoadstudio.com/settings/developer) to revoke its connection.

This repository contains integration packages only.
The packages contain no credentials, application source, executable scripts, or hooks.
Nano's marketplace is separate from OpenAI's and Anthropic's directories.

[Support](mailto:support@nanoadstudio.com) · [Privacy](https://nanoadstudio.com/legal/privacy) · [Terms](https://nanoadstudio.com/legal/terms)
