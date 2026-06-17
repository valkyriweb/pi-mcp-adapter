# AGENTS.md — pi-mcp-adapter fork

This is Luke's fork of `nicobailon/pi-mcp-adapter`.

## Local divergence

- Direct MCP tools default to deferred loading for Pi prompt-cache stability.
- Config knob: `directToolLoading: "deferred" | "eager"` globally under `settings` or per server.
- Omitted `directToolLoading` means `"deferred"`.
- Use `"eager"` only for tiny, frequently-used direct tools that must be callable without `tool_search`.

## Mac resource pressure

If work changes MCP loading, tool metadata caching, UI server lifecycle, or local helper processes, read `~/Projects/personal/mac-resource-ops/VISION.md` and `~/Projects/personal/mac-resource-ops/docs/resource-graph.md` first. Prefer deferred/lazy loading, bounded local helpers, explicit cleanup paths, and no undocumented persistent pressure.

## Upstream

- `origin` = `git@github.com:valkyriweb/pi-mcp-adapter.git`
- `upstream` = `git@github.com:nicobailon/pi-mcp-adapter.git`
- Do not blindly pull/merge upstream; inspect and cherry-pick per `fork-maintenance`.
