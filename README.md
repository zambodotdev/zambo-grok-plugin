# Zambo for Grok Build

The verifiable work layer for AI, as a Grok Build plugin. One keyless remote MCP endpoint, https://zambo.dev/mcp, serving 153 tools (35 on the default surface). Every call returns a verifiable AER-1 receipt (IETF Internet-Draft draft-zambo-aer1-26): open the run page or check it at https://zambo.dev/verify, no account.

Flagship: HANDOVER. Wrap up a session in one AI and pick the work up in another; the wrap-up carries a marker the receiving session proves it holds, and both the wrap and the pickup leave receipts. Free tier: 20 calls + 1 wrap-up free every day; picking up in another AI is always free. Day Pass: $0.99 for unlimited calls for 24 hours. Zambo Pass: $29 for 30 days, $290 for 365 days, $19 for 30 days for $ZAMBO holders.

What this plugin ships: a plugin manifest and one MCP server declaration. It ships no executable code, no hooks, no skills, and no scripts.

Network and credentials: the only endpoint the plugin declares is the remote MCP server at https://zambo.dev/mcp. It requests no credentials, reads no local files, and sets no environment variables.

Install: add the plugin from the Grok Build marketplace, or point any MCP client at https://zambo.dev/mcp directly. No API key, no signup.

License: MIT.
