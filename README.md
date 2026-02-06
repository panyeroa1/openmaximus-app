# OpenMaximus App

This repository is the OpenMaximus workspace. It includes:

- `openMax` (submodule): the OpenMax mobile-style web app (UI + API).
- `clawhub` (submodule): OpenClaw/ClawHub reference repo.

## Quick Start (Local)

1. Clone and init submodules:

```bash
git clone https://github.com/panyeroa1/openmaximus-app.git
cd openmaximus-app
git submodule update --init --recursive
```

2. Run the OpenMax app:

```bash
cd openMax
npm install
npm run dev
```

Open:
- UI: `http://localhost:3000`
- API: `http://localhost:3001`

## What Works

- Conversations:
  - create conversation
  - save/load messages
  - search across messages
  - rename conversations
- OpenClaw instant skills:
  - execute real backend actions (shell commands)
- Ollama “brain”:
  - routes requests to either “respond” or “run_skill”

## VPS Notes

The API can be deployed on a VPS with PostgreSQL + Ollama installed. The API reads configuration from `.env` on the server (do not commit secrets).

