# Blocks Cursor

Shared Cursor agents, rules, and skills for the Railblocks team.
If you are confused about what any of the terms mean, [watch this first](https://www.youtube.com/watch?v=L_p5GxGSB_I)

## Purpose

This repo is a **shared library** of personal Cursor configurations that team members can copy into their own local setup. It's meant for local settings you want applied everywhere you work.

**This is NOT for repo-specific configurations.** Repo-specific agents, rules, and skills should live directly in that repo's `.cursor/` directory.

| Type | Location | Purpose |
|------|----------|---------|
| Personal (this repo) | Copy to `~/.cursor/` or your local config | Cross-repo, personal preferences |
| Repo-specific | Stored in each repo's `.cursor/` | Project-specific patterns and conventions |

## Structure

- `.cursor/agents/` - Custom subagents for specialized tasks
- `.cursor/rules/` - Rules that apply to all conversations
- `.cursor/skills/` - Agent skills for reusable workflows and patterns

## Agents

### context-gatherer
Explores codebases to gather relevant context from code and documentation. Use proactively when you need to understand how something works, find related code, or gather context before making changes.

### docs-lookup
Documentation lookup specialist using Context7 MCP. Use proactively when building third-party integrations, researching library/framework APIs, or needing up-to-date documentation for external tools.

## Rules

### delegate-to-subagents
Instructs the agent to actively look for opportunities to delegate tasks to subagents using faster models. Applies to all conversations.

## Usage

1. Clone or pull this repository
2. Copy the configurations you want to use:
   - Copy to `~/.cursor/` for global personal settings
   - Or copy to a specific project's `.cursor/` directory
3. Customize as needed — you maintain full control over your copy

The point is to **copy and own** these configurations, not reference them. This way you can modify them to fit your workflow without affecting others.

## Contributing

When adding new agents, rules, or skills:
- Follow existing naming conventions (lowercase with hyphens)
- Include clear descriptions in the frontmatter
- Document usage in this README
