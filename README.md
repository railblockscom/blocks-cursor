# Blocks Cursor

Shared Cursor agents and skills for the Railblocks team.

This repository is for Railblocks team members to share personal skills and subagents they use and want to share with others.

## Structure

- `.cursor/agents/` - Custom subagents for specialized tasks
- `.cursor/skills/` - Agent skills for reusable workflows and patterns

## Agents

### context-gatherer
Explores codebases to gather relevant context from code and documentation. Use proactively when you need to understand how something works, find related code, or gather context before making changes.

### docs-lookup
Documentation lookup specialist using Context7 MCP. Use proactively when building third-party integrations, researching library/framework APIs, or needing up-to-date documentation for external tools.

## Usage

To use these agents and skills in your project:

1. Clone this repository
2. Copy the `.cursor/agents/` and `.cursor/skills/` directories to your project root
3. Or reference them from your personal Cursor configuration

## Contributing

When adding new agents or skills:
- Follow the existing naming conventions (lowercase with hyphens)
- Include clear descriptions in the frontmatter
- Document usage in this README
