# Blocks Cursor

Shared Cursor agents, rules, skills, and MCPs for the Blocks team.
If you are confused about what any of the terms mean, [watch this first](https://www.youtube.com/watch?v=L_p5GxGSB_I)

## Purpose

This repo is a **shared library** of personal Cursor configurations that team members can copy into their own local setup. It's meant for local settings you want applied everywhere you work.

**This is NOT for repo-specific configurations.** Repo-specific agents, rules, and skills should live directly in that repo's `.cursor/` directory.

| Type | Location | Purpose |
|------|----------|---------|
| Personal (this repo) | Copy to `~/.cursor/` or your local config | Cross-repo, personal preferences |
| Repo-specific | Stored in each repo's `.cursor/` | Project-specific patterns and conventions |

## Structure

```
blocks-cursor/
├── agents/      → copy to ~/.cursor/agents/
├── rules/       → copy to ~/.cursor/rules/
├── skills/      → copy to ~/.cursor/skills/
└── mcp/
    ├── mcp.json → copy to ~/.cursor/mcp.json
    └── mcp.md   → reference only
```

## Agents

### context-gatherer
Explores codebases to gather relevant context from code and documentation. Use proactively when you need to understand how something works, find related code, or gather context before making changes.

### docs-lookup
Documentation lookup specialist using Context7 MCP. Use proactively when building third-party integrations, researching library/framework APIs, or needing up-to-date documentation for external tools.

## Rules

### delegate-to-subagents
Instructs the agent to actively look for opportunities to delegate tasks to subagents using faster models. Applies to all conversations.

## MCPs

MCP (Model Context Protocol) servers extend Cursor's capabilities with external tools and data sources. See [`mcp/mcp.md`](mcp/mcp.md) for full documentation on each server.

**Available MCPs:**
- **Context7** - Library/framework documentation lookup
- **Convex** - Backend queries, data management, logs
- **Greptile** - AI-powered code search and review
- **Axiom** - Logs and observability
- **PostHog** - Product analytics and feature flags

**Setup:** Copy `mcp/mcp.json` to `~/.cursor/mcp.json` and add your credentials.

## Skills

Skills are reusable capabilities for AI agents. They provide procedural knowledge that helps agents accomplish specific tasks more effectively. Think of them as plugins or extensions that enhance what your AI agent can do.

It's a open standard, you can [read the specification here](https://agentskills.io/home)

There are marketplaces to find and download skills built by other people such as:
- [skills.sh](https://skills.sh/)
- [context7 skills](https://x.com/Context7AI/status/2014702620758118768)

## Usage

1. Clone or pull this repository
2. Copy the configurations you want to your local `~/.cursor/` folder:
   ```bash
   cp -r agents/ ~/.cursor/agents/
   cp -r rules/ ~/.cursor/rules/
   cp -r skills/ ~/.cursor/skills/
   cp mcp/mcp.json ~/.cursor/mcp.json
   ```
3. Add your credentials to `~/.cursor/mcp.json` (replace placeholder tokens)
4. Restart Cursor to load the changes
5. Customize as needed — you maintain full control over your copy

The point is to **copy and own** these configurations, not reference them. This way you can modify them to fit your workflow without affecting others.

## Contributing

When adding new agents, rules, skills, or MCPs:
- Follow existing naming conventions (lowercase with hyphens)
- Include clear descriptions in the frontmatter
- Document usage in this README
- For MCPs, add documentation to `mcp/mcp.md`
