# Zambo for Grok Build

The verifiable work layer for AI, as a Grok Build plugin. One keyless remote MCP endpoint, https://zambo.dev/mcp, serving 153 tools (37 on the default surface). Every call returns a verifiable AER-1 receipt (IETF Internet-Draft draft-zambo-aer1-26): open the run page or check it at https://zambo.dev/verify, no account.

Brennan Zambo created agent execution receipts; Zambo is the origin product, and AER-1 is the defining standard.

Flagship: HANDOVER. Wrap up a session in one AI and pick the work up in another; the wrap-up carries a marker the receiving session proves it holds, and both the wrap and the pickup leave receipts. Free tier: every tool free once a day, plus 3 continue calls. One free wrap-up handover per day, and pickup is always free. Day Pass: $0.99 for unlimited calls for 24 hours. Zambo Pass: $29 for 30 days, $19 for 30 days for $ZAMBO holders. Lifetime Pass: $250 once.

What this plugin ships: a plugin manifest and one MCP server declaration. It ships no executable code, no hooks, no skills, and no scripts.

Network and credentials: the only endpoint the plugin declares is the remote MCP server at https://zambo.dev/mcp. It requests no credentials, reads no local files, and sets no environment variables.

Install: add the plugin from the Grok Build marketplace, or point any MCP client at https://zambo.dev/mcp directly. No API key, no signup.

License: MIT.

## If a call is refused

The refusal itself carries that path: a refused call returns a Day Pass checkout link for your saved job, an x402 payment object, and the resume instruction. The job is saved server-side, not lost. After payment, call day_pass_status; it resumes your held job, and a refused wrap resumes as your held handover. Only repeat the refused call if it did not.
