# AGENTS.md — pi-mcp-adapter fork

This is Luke's fork of `nicobailon/pi-mcp-adapter`.

## Local divergence

- Direct MCP tools default to deferred loading for Pi prompt-cache stability.
- Config knob: `directToolLoading: "deferred" | "eager"` globally under `settings` or per server.
- Omitted `directToolLoading` means `"deferred"`.
- Use `"eager"` only for tiny, frequently-used direct tools that must be callable without `tool_search`.

## Upstream

- `origin` = `git@github.com:valkyriweb/pi-mcp-adapter.git`
- `upstream` = `git@github.com:nicobailon/pi-mcp-adapter.git`
- Do not blindly pull/merge upstream; inspect and cherry-pick per `fork-maintenance`.
