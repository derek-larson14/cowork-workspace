# Co-Work Workspace

Starter workspace for [Delegate with Claude](https://delegatewithclaude.com), built for Co-Work (Claude's desktop app).

The first time you start a conversation, Claude reads the CLAUDE.md and walks you through setup: checking your connectors, installing the [delegate-cowork](https://github.com/derek-larson14/delegate-plugins/tree/main/plugins/delegate-cowork) plugin, and learning about your work.

## Setup

1. Download this folder (green button > Download ZIP)
2. Unzip it
3. Open the [Claude desktop app](https://claude.com/download)
4. Mount the folder in Co-Work
5. Say "help me get set up". Claude handles the rest.

## What's Inside

- `CLAUDE.md` - Guided first-run setup + context about how you work
- `scratch/` - Claude's working space for research and notes

Files like `tasks.md` and `delegation.md` get created during setup based on how you want to work. You can open this folder in [Obsidian](https://obsidian.md) to browse and edit files alongside Co-Work.

## Connectors

The [delegate-cowork](https://github.com/derek-larson14/delegate-plugins/tree/main/plugins/delegate-cowork) plugin uses MCP connectors instead of terminal tools. Enable these in Co-Work for the full experience:

| Connector | Used by |
|-----------|---------|
| Google Calendar | `/morning`, `/weekly`, `/meeting`, `/calendar` |
| Gmail | `/morning`, `/weekly`, `/mail` |
| Google Drive | File access, voice transcripts |
| Granola | `/meeting` |

GitHub and Granola connectors are optional. Every command gracefully skips connectors that aren't available.

## For Claude Code Users

If you prefer the terminal, use the [delegate workspace](https://github.com/derek-larson14/delegate) instead. It has 13 commands, [Obsidian](https://obsidian.md) plugins, and Mac-specific tools built in.

Learn more at [Delegate with Claude](https://delegatewithclaude.com).

---

By [Derek Larson](https://dtlarson.com). MIT License.
