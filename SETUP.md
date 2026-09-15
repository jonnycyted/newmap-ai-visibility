# Setup

The plugin works without any key: the `audit` tool runs New Map's free AI visibility audit for any website (one per domain per 30 days).

New Map clients can connect their own workspace so every other tool (weekly visibility, trends, the verbatim engine answers, prompt performance, competitor gaps, citations) reads their live data:

1. Ask your New Map account manager for an MCP key (it starts with `nm_`).
2. Set it as `newmap_api_key` in this plugin's configuration.
3. Reload. `tools/list` now shows the read tools next to `audit`, all scoped to your workspace.

Nothing is written to New Map from this plugin: every tool is read-only.
