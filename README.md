# Blocks Cursor

Shared Cursor agents and skills for the Railblocks team.

## Structure

- `.cursor/agents/` - Custom subagents for specialized tasks
- `.cursor/skills/` - Agent skills for reusable workflows and patterns

## Agents

### context-gatherer
Explores codebases to gather relevant context from code and documentation. Use proactively when you need to understand how something works, find related code, or gather context before making changes.

### docs-lookup
Documentation lookup specialist using Context7 MCP. Use proactively when building third-party integrations, researching library/framework APIs, or needing up-to-date documentation for external tools.

## Skills

### create-rule
Create Cursor rules for persistent AI guidance. Use when the user wants to create a rule, add coding standards, set up project conventions, configure file-specific patterns, create RULE.md files, or asks about .cursor/rules/ or AGENTS.md.

### create-skill
Guides users through creating effective Agent Skills for Cursor. Use when the user wants to create, write, or author a new skill, or asks about skill structure, best practices, or SKILL.md format.

### create-subagent
Create custom subagents for specialized AI tasks. Use when the user wants to create a new type of subagent, set up task-specific agents, configure code reviewers, debuggers, or domain-specific assistants with custom prompts.

### migrate-to-skills
Convert 'Applied intelligently' Cursor rules (.cursor/rules/*.mdc) and slash commands (.cursor/commands/*.md) to Agent Skills format (.cursor/skills/). Use when the user wants to migrate rules or commands to skills, convert .mdc rules to SKILL.md format, or consolidate commands into the skills directory.

### update-cursor-settings
Modify Cursor/VSCode user settings in settings.json. Use when the user wants to change editor settings, preferences, configuration, themes, font size, tab size, format on save, auto save, keybindings, or any settings.json values.

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
