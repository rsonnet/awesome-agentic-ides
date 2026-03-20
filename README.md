# Awesome Agentic IDEs [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of Agentic Development Environments (ADEs) — tools that integrate AI coding agents into terminal, GUI, or TUI interfaces.

## Comparison

| Tool | Type | Git Worktree GUI | Terminal Agent | No Auth Required | Open Source | Notes |
|---|---|:---:|:---:|:---:|:---:|---|
| [Agentastic](https://www.agentastic.dev/) | GUI | ✅ | ✅ | ✅ | ❌ | Perfect for worktree management and terminal integration. Code browsing needs better UX. `$ code .` works just fine from the terminal |
| [Emdash](https://emdash.sh) | GUI | ✅ | ✅ | ✅ | ✅ | slow on interactions |
| [Warp](https://www.warp.dev) | Terminal | ❌ | ✅ | ❌ | ❌ | Built-in AI only; no worktree GUI |
| [cmux](https://github.com/nicholasgasior/cmux) | Terminal | ❌ | ✅ | ✅ | ✅ | Splitting + sidebar terminals, slick UX, no code viewer |
| [dmux](https://github.com/zdcthomas/dmux) | TUI | ❌ | ✅ | ✅ | ✅ | Pain to use |
| [1code.dev](https://1code.dev) | GUI | - | ❌ | ❌ | - | Wraps Claude/Codex APIs directly; asks for API keys instead of using CLI agents |
| [Air.dev](https://air.dev) | GUI | - | ❌ | ❌ | - | Requires Claude/Codex login |
| [Superset.sh](https://superset.sh) | GUI | - | - | ❌ | ❌ | Requires GitHub/Google login |
| [Conductor](https://conductor.build) | GUI | - | - | ❌ | ❌ | Requires GitHub login |
| [Catnip](https://github.com/wandb/catnip) | GUI | - | - | - | ✅ | Requires Docker/Colima; complex install |
| [Fleetcode](https://github.com/built-by-as/FleetCode) | GUI | - | - | - | ✅ | npm install issues |

**Legend:** ✅ supported · ❌ not supported · `-` unknown/not applicable/couldn't verify

## Column Definitions

- **Git Worktree GUI** — automatic worktree creation/switching built into the UI
- **Terminal Agent** — shells out to a locally installed CLI agent (e.g. Claude Code, Gemini CLI, Codex CLI) rather than wrapping the provider API itself
- **No Auth Required** — no mandatory login to agent providers; compatible with LiteLLM or any local proxy setup
- **Open Source** — source code publicly available
