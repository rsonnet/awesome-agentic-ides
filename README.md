# Awesome Agentic IDEs [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of Agentic Development Environments (ADEs) — tools that integrate AI coding agents into terminal, GUI, or TUI interfaces.

## Comparison

| Tool | Git Worktree GUI | Terminal Agent | No Auth Required | Open Source | Diff Viewer | Notes |
|---|:---:|:---:|:---:|:---:|:---:|---|
| [Emdash](https://emdash.sh) | ✅ | ✅ | ✅ | ✅ | ✅ | slow on interactions. open worktree with editor of choice |
| [Superset.sh](https://superset.sh) | ✅ | ✅ | ✅ | ✅ | ✅ | packaged installer requires login. git clone version doesn't require login. so have to manually update from latest master/release. good worktree support with sub workspaces. slow  |
| [Hive](https://github.com/morapelker/hive) | ✅ | ✅ | ✅ | ✅ | ✅ | a bit buggy and slow. opened editor panes are not synced with worktrees |
| [Superzent](https://github.com/currybab/superzent) | ✅ | ✅ | ✅ | ✅ | ✅ | fork of the Zed editor inspired by superset.sh |
| [1code.dev](https://1code.dev) | ✅ | ❌ | ❌ | ✅ | ✅ | Wraps Claude/Codex APIs directly; asks for API keys instead of using CLI agents. main agent pane is owned by the tool and cannot simply have a terminal running claude/codex in main agent pane |
| [Agentastic](https://www.agentastic.dev/) | ✅ | ✅ | ✅ | ❌ | ✅ | Perfect for worktree management and terminal integration. Code browsing needs better UX. `$ code .` works just fine from the terminal. slow diff viewing |
| [Warp](https://www.warp.dev) | ❌ | ✅ | ✅ | ❌ | ✅ | Built-in AI only; no worktree GUI |
| [DevSwarm](https://devswarm.ai/) | ✅ | ✅ | ❌ | ❌ | ✅ | Perfect for code browsing because every worktree has its own vscode server inside it. So clicking any tab on the worktree pane on the left shows its own vscode in the main pane. But auth required and not opensource. Switching worktrees/workspaces has no lag but creating new worktrees have some lag (and it's likely due to creating vscode server instances for each) |
| [cmux](https://github.com/nicholasgasior/cmux) | ❌ | ✅ | ✅ | ✅ | ❌ | Splitting + sidebar terminals, slick UX, no diff viewer. worktrees can be autocreated in workspaces using plugins/scripts |
| [dmux](https://github.com/zdcthomas/dmux) | ❌ | ✅ | ✅ | ✅ | ❌ | Pain to use |
| [Air.dev](https://air.dev) | - | - | ❌ | ❌ | ✅ | Requires Claude/Codex login |
| [Conductor](https://conductor.build) | - | - | ❌ | ❌ | ✅ | Requires GitHub login |
| [Catnip](https://github.com/wandb/catnip) | - | - | - | ✅ | - | Requires Docker/Colima; complex install |
| [Fleetcode](https://github.com/built-by-as/FleetCode) | - | - | - | ✅ | - | npm install issues |

**Legend:** ✅ supported · ❌ not supported · `-` unknown/not applicable/couldn't verify

## Column Definitions

- **Git Worktree GUI** — Built-in UI for creating, switching, and managing Git worktrees.
  Lets you spin up isolated branches side-by-side without leaving the tool, so multiple agents can work on different tasks in parallel without stepping on each other.

- **Terminal Agent** — Runs a locally installed CLI agent (e.g. Claude Code, Gemini CLI, Codex CLI) in a real terminal pane rather than wrapping the provider's API directly.
  This means you keep full control over your agent's configuration, context, and billing. Tools that lack this force you into their own API wrapper, which may limit model choice, tool use, or MCP server support.

- **No Auth Required** — No mandatory login or account creation to use the tool itself.
  You bring your own CLI agent and API keys. Compatible with LiteLLM, local proxies, or any custom setup — the tool doesn't gate access behind its own auth wall.

- **Open Source** — Source code is publicly available under an open-source license.
  You can inspect, modify, self-host, and contribute. Closed-source tools may disappear, change pricing, or add restrictions without notice.

- **Diff Viewer** — Built-in UI for reviewing code changes made by the agent.
  Shows a side-by-side or inline diff of what the agent modified, so you can approve, revert, or edit changes before committing.
