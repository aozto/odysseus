# Odysseus 🚀

> Self-hosted AI workspace with MCP-native agents

## Overview

Odysseus is a lightweight, self-hosted AI workspace that brings MCP-native agent orchestration to your infrastructure. Built with Go for maximum performance.

## Features

- 🧩 **MCP-native** — First-class MCP protocol support for tool/agent interoperability
- 🔄 **Multi-model routing** — Route tasks between DeepSeek, Claude, and local models
- 📦 **Self-contained** — Single binary deployment, no Kubernetes required
- 🔌 **Plugin system** — Hot-swappable skills via MCP tool registry
- 📊 **Token optimization** — Automatic context compression saves 40-60% tokens

## Quick Start

```bash
# Coming soon
docker pull ghcr.io/aozto/odysseus:latest
```

## Architecture

```
┌─────────────────────────────────────────┐
│           Odysseus Core (Go)             │
│  ┌─────────┐  ┌────────┐  ┌──────────┐  │
│  │  Agent   │  │ Router │  │ Codex     │  │
│  │ Pool     │  │  Engine│  │ Runner    │  │
│  └─────────┘  └────────┘  └──────────┘  │
│  ┌────────────────────────────────────┐  │
│  │         MCP Protocol Layer         │  │
│  │  (Tools · Resources · Prompts)     │  │
│  └────────────────────────────────────┘  │
└─────────────────────────────────────────┘
```

## License

MIT
