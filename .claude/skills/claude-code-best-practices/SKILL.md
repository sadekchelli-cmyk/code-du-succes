---
name: claude-code-best-practices
description: "Reference guide for configuring and using Claude Code itself: settings.json options and environment variables, CLAUDE.md memory loading rules, skills frontmatter, subagent types, slash commands, MCP servers, CLI startup flags, and power-up features. Use when the user asks how to configure Claude Code, write a CLAUDE.md, build or debug a skill/subagent/command/hook, set up MCP servers, tune settings.json or permissions, or wants best practices for working with Claude Code in this repo."
---

# Claude Code Best Practices

Reference material for configuring and working with Claude Code itself, adapted from the community best-practices collection at [shanraisshan/claude-code-best-practice](https://github.com/shanraisshan/claude-code-best-practice).

## When to Apply

Use this skill when the task is about **Claude Code's own configuration and tooling** rather than the project's product code: writing or restructuring `CLAUDE.md`, adding a skill/command/subagent/hook, configuring `.claude/settings.json` or permissions, wiring up MCP servers, or choosing CLI flags/startup options.

Skip it for ordinary product work (landing page content, styling, etc.) — that's covered by other skills in this repo, not this one.

## Reference Index

Read the relevant file on demand rather than loading all of them — each is self-contained.

| Topic | File | Covers |
|-------|------|--------|
| Skills | `references/skills.md` | All 17 skill frontmatter fields, official bundled skills |
| Commands | `references/commands.md` | Slash command frontmatter, official built-in commands |
| Subagents | `references/subagents.md` | Subagent frontmatter, official built-in agent types |
| Memory | `references/memory.md` | How `CLAUDE.md` loads (ancestor vs. descendant), monorepo structuring |
| MCP servers | `references/mcp-servers.md` | Recommended MCP servers and configuration practices |
| Settings | `references/settings.md` | Full `settings.json` reference — permissions, hooks, sandbox, plugins, model config, env vars |
| CLI startup flags | `references/cli-startup-flags.md` | `claude` CLI flags and startup options |
| Power-ups | `references/power-ups.md` | The 10 built-in `/powerup` interactive lessons |

## Workflow

1. Identify which topic the task touches (skills, commands, subagents, memory, MCP, settings, CLI flags, or power-ups).
2. Read the matching `references/*.md` file for the authoritative field list and examples before writing config — don't guess frontmatter fields or settings keys from memory.
3. Apply the convention shown (e.g. skill directory layout with `SKILL.md` + `references/`, as used by this skill and `ui-ux-pro-max` in this repo) rather than inventing a new structure.
4. When a reference conflicts with the installed Claude Code version's actual behavior (flags/fields change between versions), trust observed behavior and note the discrepancy rather than forcing the doc's claim.

## Source & Attribution

Content adapted from [shanraisshan/claude-code-best-practice](https://github.com/shanraisshan/claude-code-best-practice) (MIT licensed), `best-practice/` directory, as of 2026-07-28. Screenshots/diagrams from the original `assets/` folder were dropped since they don't render usefully as skill reference text; links to sources are preserved in each file's "Sources" section.
