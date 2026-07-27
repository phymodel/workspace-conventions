---
name: Workspace conventions
description: PhyModel Studio layout and editing conventions.
always: false
---

# Workspace conventions

- Prefer minimal, focused diffs; do not refactor unrelated code.
- This repo is **phymodel_studio** (`web_editor/`). Sibling **phymodel_agi** holds llm/omni/dataprep and the training `venv`.
- Harness packages live under `.phymodel/harness/` in this repo (e.g. FBC). When running FBC from agi’s cwd: `python ../phymodel_studio/.phymodel/harness/...` and use agi’s `venv`.
- Subagent personas under `.phymodel/subagents/<id>/SUBAGENT.md` — share via git; enable per Agent in the panel.
- Conversation exports live under `.phymodel/conversations/` — treat as user data, not templates.
- Use forward-slash relative paths from the workspace root in tool calls.
- Match existing naming, imports, and comment style in each subproject.
