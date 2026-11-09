# Pupfish Plugins

Claude Code plugin marketplace by [Pupfish Analytics](https://pupfish.io).

## Installation

### From the Claude Code desktop UI

1. In the left sidebar under **Personal plugins**, click the **+** button.
2. Choose **Create plugin → Add marketplace**.
3. In the URL field, enter `Pupfish-LLC/claude-plugins`, then click **Sync**.
4. Once the marketplace is synced, click the **+** button again and choose **Browse plugins** to install any of the plugins below.

### From the command line

```
/plugin marketplace add Pupfish-LLC/claude-plugins
/plugin install qlik-toolkit@pupfish
```

## Available Plugins

### [qlik-toolkit](https://github.com/Pupfish-LLC/qlik-toolkit)

Make Claude Code fluent in Qlik Sense. Install once and Claude becomes a Qlik developer you can delegate to, with deep platform knowledge, specialist agents for different tasks, and an automatic syntax check on every script.

- 12 skills covering data modeling, load scripts, expressions, performance, visualization, QA, source profiling, and Cloud MCP integration
- 7 specialist agents (data architect, script developer, expression developer, viz architect, requirements analyst, QA reviewer, doc writer) invoked on demand
- A PostToolUse hook that flags common Qlik script syntax mistakes before reload

Install: `/plugin install qlik-toolkit@pupfish`

### [qlik-agents](https://github.com/Pupfish-LLC/qlik-agents)

A multi-agent development pipeline for Qlik Sense. You provide source materials and requirements; the pipeline produces production-grade load scripts, expressions, visualization specs, QA reports, and documentation through a structured 9-phase workflow with approval gates and execution validation.

Most Qlik developers will prefer [qlik-toolkit](https://github.com/Pupfish-LLC/qlik-toolkit) for ad-hoc work. Reach for `qlik-agents` when you want the full structured pipeline from requirements through documentation.

Install: `/plugin install qlik-agents@pupfish`

### [model-picker](https://github.com/Pupfish-LLC/model-picker)

Use the right Claude model for the job. Ask Claude which model and effort level a piece of work needs, from Haiku 5.5 to Fable 5.2, and get one clear pick with the reason behind it.

- One skill that matches a task to a model and effort level, based on the stakes, the kind of work and how you pay for Claude
- The published evidence behind each pick, with sources and dates
- 8 ready-made agent files for Claude Code, installed only when you ask, plus a way to verify which model each agent really ran on
- Updated when Anthropic releases or changes a model

Install: `/plugin install model-picker@pupfish`

## Migrating from `pupfish-qlik`

The `pupfish-qlik` plugin was renamed to `qlik-toolkit` in 0.2.0. The plugin content is identical; only the name changed. If you have `pupfish-qlik` installed, the marketplace no longer lists it (so the Update button will not appear). To switch:

1. Re-sync this marketplace (Personal plugins → **+** → **Create plugin → Add marketplace**, enter `Pupfish-LLC/claude-plugins`, click **Sync**). Or from the CLI: `/plugin marketplace update`.
2. Uninstall the old plugin: `/plugin uninstall pupfish-qlik` (or remove it via the GUI).
3. Install the renamed plugin: `/plugin install qlik-toolkit@pupfish`.

## Author

[Pupfish Analytics](https://pupfish.io)
