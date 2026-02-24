# Awesome Personal AI Assistants [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of open-source personal AI assistants you run on your own devices.

These are always-on, self-hosted AI agents that connect to your existing chat channels (WhatsApp, Telegram, Slack, Discord, etc.), remember context across conversations, and act on your behalf. They use LLMs as their reasoning engine but run locally under your control.

## Contents

- [Full-Featured](#full-featured)
- [Lightweight](#lightweight)
- [Bare Metal](#bare-metal)
- [Security-Focused](#security-focused)
- [Multi-Agent](#multi-agent)
- [Bridges & Orchestrators](#bridges--orchestrators)
- [IM Bot Platforms](#im-bot-platforms)
- [Agent Frameworks](#agent-frameworks)
- [Deployment](#deployment)
- [Memory Systems](#memory-systems)
- [Ecosystem](#ecosystem)
- [Comparison](#comparison)

## Full-Featured

- [OpenClaw](https://github.com/openclaw/openclaw) - The original personal AI assistant. Supports 14+ chat channels (WhatsApp, Telegram, Slack, Discord, Signal, iMessage, and more), skills system, voice I/O, and a live Canvas. Node.js gateway architecture with onboarding wizard. `Node.js` ![Stars](https://img.shields.io/github/stars/openclaw/openclaw)
- [nanobot](https://github.com/HKUDS/nanobot) - Ultra-lightweight assistant in ~4,000 lines of Python. Multi-provider (OpenAI, Anthropic, Gemini, DeepSeek, local), scheduled tasks, market analysis, and multi-platform chat (Telegram, Discord, Slack, Email). Research-ready codebase. `Python` ![Stars](https://img.shields.io/github/stars/HKUDS/nanobot)
- [ZeroClaw](https://github.com/zeroclaw-labs/zeroclaw) - Fast, small, and fully autonomous AI assistant infrastructure. Rust rewrite of the OpenClaw architecture — deploy anywhere, swap anything. `Rust` ![Stars](https://img.shields.io/github/stars/zeroclaw-labs/zeroclaw)
- [moltis](https://github.com/moltis-org/moltis) - Single binary personal assistant with long-term memory, sandboxed execution, voice I/O, MCP tools, and multi-channel access (web, Telegram, API). `Rust` ![Stars](https://img.shields.io/github/stars/moltis-org/moltis)
- [Sentient](https://github.com/existence-master/Sentient) - Personal AI assistant for everyone. Multi-provider, extensible plugin system, and local-first design. `Python` ![Stars](https://img.shields.io/github/stars/existence-master/Sentient)
- [Gaia](https://github.com/theexperiencecompany/gaia) - Proactive personal AI assistant for daily work, inspired by Jarvis. Scheduled automations and integrations for productivity workflows. `TypeScript` ![Stars](https://img.shields.io/github/stars/theexperiencecompany/gaia)
- [MARVIN](https://github.com/SterlingChin/marvin-template) - Template-based personal AI assistant that connects to the apps you need and handles your day. Easy to fork and customize. `Shell` ![Stars](https://img.shields.io/github/stars/SterlingChin/marvin-template)
- [personal-ai-assistant](https://github.com/kaymen99/personal-ai-assistant) - Multi-agent assistant connecting to WhatsApp, Slack, or Telegram. Manages emails, schedule, to-dos, messages, and daily research. `Python` ![Stars](https://img.shields.io/github/stars/kaymen99/personal-ai-assistant)

## Lightweight

- [NanoClaw](https://github.com/gavrielc/nanoclaw) - Fork-and-customize assistant built on Claude Agent SDK. Agents run in real Linux containers (Apple Container or Docker) with filesystem isolation. WhatsApp I/O, per-group memory, and scheduled tasks. Small enough to understand in 8 minutes. `TypeScript` ![Stars](https://img.shields.io/github/stars/gavrielc/nanoclaw)
- [Clawlet](https://github.com/mosaxiv/clawlet) - Single static binary with zero dependencies. Bundles SQLite + sqlite-vec for hybrid semantic memory search. Multi-provider (OpenAI, Anthropic, Gemini, OpenRouter, local). No CGO, no runtime — drop it on any machine. `Go` ![Stars](https://img.shields.io/github/stars/mosaxiv/clawlet)
- [Picobot](https://github.com/louisho5/picobot) - Runs on a $5 VPS or Raspberry Pi. ~8MB binary, ~28MB Docker image, ~10MB RAM idle. Telegram integration, persistent memory, tool calling, and skills — all in a single Go binary. `Go` ![Stars](https://img.shields.io/github/stars/louisho5/picobot)
- [MyClaw](https://github.com/stellarlinkco/myclaw) - Mini clawbot. Lightweight OpenClaw-inspired assistant targeting minimal footprint while keeping core functionality. `Go` ![Stars](https://img.shields.io/github/stars/stellarlinkco/myclaw)
- [lettabot](https://github.com/letta-ai/lettabot) - Personal AI assistant that remembers everything across Telegram, Slack, WhatsApp, and Signal. Built on Letta's persistent memory engine. `TypeScript` ![Stars](https://img.shields.io/github/stars/letta-ai/lettabot)

## Bare Metal

- [MimiClaw](https://github.com/memovai/mimiclaw) - Run OpenClaw on a $5 chip with no OS, no Node.js, no Linux. Bare-metal C implementation with local-first memory. Portable, shareable, and privacy-first. `C` ![Stars](https://img.shields.io/github/stars/memovai/mimiclaw)
- [SubZeroClaw](https://github.com/jmlago/subzeroclaw) - The minimal agentic loop in ~380 lines of C. 54KB binary, runs on a Raspberry Pi with 2MB RAM. Skill-driven daemon — one file, one loop, one tool. `C` ![Stars](https://img.shields.io/github/stars/jmlago/subzeroclaw)

## Security-Focused

- [IronClaw](https://github.com/nearai/ironclaw) - Defense-in-depth architecture with WASM-sandboxed tools, credential injection (secrets never exposed to tool code), prompt injection detection, and endpoint allowlisting. Dynamic tool building, Docker sandbox, web gateway, and routines engine. `Rust` ![Stars](https://img.shields.io/github/stars/nearai/ironclaw)

## Multi-Agent

- [TinyClaw](https://github.com/jlia0/tinyclaw) - Run multiple teams of AI agents that collaborate with chain execution and fan-out. Discord, WhatsApp, and Telegram channels. Supports both Anthropic Claude and OpenAI Codex. Live TUI dashboard for monitoring agent chains. `Node.js/Bash` ![Stars](https://img.shields.io/github/stars/jlia0/tinyclaw)

## Bridges & Orchestrators

- [takopi](https://github.com/banteg/takopi) - Telegram bridge for multiple coding agents (Codex, Claude Code, OpenCode, pi). Manages projects and git worktrees, streams progress, and supports parallel runs across agent sessions. Works with voice notes and scheduled messages. `Python` ![Stars](https://img.shields.io/github/stars/banteg/takopi)

## IM Bot Platforms

- [AstrBot](https://github.com/AstrBotDevs/AstrBot) - Agentic IM chatbot infrastructure integrating multiple IM platforms (QQ, WeChat, Telegram, Discord, and more), LLMs, plugins, and AI features. Production-ready with plugin marketplace. `Python` ![Stars](https://img.shields.io/github/stars/AstrBotDevs/AstrBot)
- [LangBot](https://github.com/langbot-app/LangBot) - Production-grade platform for building agentic IM bots. Supports Discord, Slack, LINE, Telegram, WeChat, Feishu, DingTalk, QQ, and more. Integrates with ChatGPT, DeepSeek, Claude, Gemini, Ollama, and other providers. `Python` ![Stars](https://img.shields.io/github/stars/langbot-app/LangBot)

## Agent Frameworks

- [pi](https://github.com/badlogic/pi-mono) - Monorepo of tools for building AI agents. Includes a unified multi-provider LLM API, agent runtime with tool calling, interactive coding agent CLI, Slack bot, terminal UI library, web UI components, and vLLM pod management. `TypeScript` ![Stars](https://img.shields.io/github/stars/badlogic/pi-mono)
- [pz](https://github.com/joelreymont/pz) - Drop-in replacement for pi rewritten in Zig. 1.7MB static binary, 3ms startup, 1.4MB RAM idle. Full feature parity plus TUI with syntax highlighting, image rendering, 582 tests, and zero-alloc hot path. `Zig` ![Stars](https://img.shields.io/github/stars/joelreymont/pz)

## Deployment

- [MoltWorker](https://github.com/cloudflare/moltworker) - Run OpenClaw on Cloudflare Workers. Edge deployment with serverless scaling, no VPS needed. `TypeScript` ![Stars](https://img.shields.io/github/stars/cloudflare/moltworker)

## Memory Systems

- [memU](https://github.com/NevaMind-AI/memU) - Memory system for 24/7 proactive agents. Designed to work with OpenClaw and similar assistants, providing persistent context and recall across sessions. `Python` ![Stars](https://img.shields.io/github/stars/NevaMind-AI/memU)

## Ecosystem

- [awesome-openclaw-skills](https://github.com/VoltAgent/awesome-openclaw-skills) - The official collection of OpenClaw skills. ![Stars](https://img.shields.io/github/stars/VoltAgent/awesome-openclaw-skills)
- [awesome-openclaw-usecases](https://github.com/hesamsheikh/awesome-openclaw-usecases) - Community collection of OpenClaw use cases. ![Stars](https://img.shields.io/github/stars/hesamsheikh/awesome-openclaw-usecases)
- [ClawRouter](https://github.com/BlockRunAI/ClawRouter) - Agent-native LLM router powering OpenClaw. `TypeScript` ![Stars](https://img.shields.io/github/stars/BlockRunAI/ClawRouter)
- [buildwithclaude](https://github.com/davepoon/buildwithclaude) - Hub for Claude Skills, Agents, Commands, Hooks, and Plugins for Claude Code, Claude Desktop, Agent SDK, and OpenClaw. `TypeScript` ![Stars](https://img.shields.io/github/stars/davepoon/buildwithclaude)

## Comparison

| Project | Language | Channels | Memory | Isolation | Multi-Provider | Multi-Agent |
|---------|----------|----------|--------|-----------|---------------|-------------|
| OpenClaw | Node.js | 14+ | Hybrid search | App-level | Yes | No |
| nanobot | Python | 6+ | Built-in | No | Yes | No |
| moltis | Rust | Web, Telegram, API | Long-term | Sandbox | Yes | No |
| Sentient | Python | Multi | Built-in | No | Yes | No |
| NanoClaw | TypeScript | WhatsApp | Per-group | Container | Anthropic | Swarms |
| Clawlet | Go | CLI | Semantic (SQLite) | No | Yes | No |
| Picobot | Go | Telegram | Persistent | Docker | Via OpenRouter | No |
| ZeroClaw | Rust | Multi | Built-in | Yes | Yes | No |
| MimiClaw | C | — | Local | Bare metal | No | No |
| SubZeroClaw | C | — | Skill files | None | Via API | No |
| IronClaw | Rust | Multi (WASM) | Hybrid search | WASM + Docker | NEAR AI | No |
| TinyClaw | Node.js/Bash | 3 | Persistent | Isolated workspaces | Claude + Codex | Teams |
| takopi | Python | Telegram | Session resume | Worktrees | Multi-engine | Parallel |
| AstrBot | Python | 8+ | Plugin-based | No | Yes | No |
| LangBot | Python | 10+ | Knowledge base | No | Yes | No |
| pi | TypeScript | Slack | Stateful | No | Yes | No |
| pz | Zig | CLI | Sessions | No | Yes | No |
| MoltWorker | TypeScript | (OpenClaw) | (OpenClaw) | Edge/Workers | (OpenClaw) | No |
| lettabot | TypeScript | 4 | Persistent (Letta) | No | Yes | No |

## Contributing

Contributions welcome! Read the [contribution guidelines](contributing.md) first.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related or neighboring rights to this work.
