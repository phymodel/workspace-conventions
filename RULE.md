---
name: Workspace conventions
description: PhyModel Studio layout and editing conventions.
always: false
---

# Workspace conventions

- Prefer minimal, focused diffs; do not refactor unrelated code.
- Current workspace repos: **phymodel__studio** (ChatStudio + `web_editor/`), **phymodel__fbc-data-generation** (FBC Harness 独立包), **phymodel__llm-trainer** (训练 venv + llm/omni/dataprep).
- FBC Harness 由 ChatStudio 缓存同步到 `~/.chatstudio/cache/harnesses/fbc-data-generation/`；运行 FBC 脚本时使用该路径，并选用 llm-trainer 的 venv。
- Subagent personas under `.phymodel/subagents/<id>/SUBAGENT.md` — share via git; enable per Agent in the panel.
- Conversation exports live under `.phymodel/conversations/` — treat as user data, not templates.
- Use forward-slash relative paths from the workspace root in tool calls.
- Match existing naming, imports, and comment style in each subproject.
