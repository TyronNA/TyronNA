# Hi, I'm Tyron 👋

Full-stack engineer from Vietnam. I ship things end-to-end — the API, the web app, the deploy — and lately I build a lot of them *with* AI agents rather than around them.

## Games & products

**[Tales of Ascension](https://play.google.com/store/apps/details?id=com.mgho.app)** · live on Google Play
Solo-built wuxia auto-battler card RPG. Next.js + Capacitor client, Go + PostgreSQL backend, Cocos Creator 3.8 combat engine.

**[Bàn Ráp](https://bibaplay.com)** · free, in Vietnamese
Self-study electronics course for beginners — Ohm's law to ESP32 to robots. Every lesson has step-by-step breadboard pictures and a circuit simulator.

## AI pipelines

The rule I build them by: deterministic code owns orchestration, retries and budgets; the model only owns the creative calls. Nothing expensive runs until a cheap gate has passed.

**Archivist** — a history topic in, a finished MP4 out: researched script → voice → shots → render, for two YouTube history channels (world / Vietnam). Editorial rule changes are blind-judged against a narrative benchmark before they ship.

## Agents & tooling

- **Dev Hub** — VS Code extension that runs Claude Code and Codex sessions across many repos from one window, plus a mobile web view to follow them from my phone. Zero runtime dependencies.
- **Slack agent orchestrator** — Claude Agent SDK service: per-thread sessions persisted in SQLite, GitHub / Jira adapters, isolated git worktrees for dev tasks.
- **Read-only review bot** — @mention in Slack → Claude reviews a local repo. Write tools are hard-blocked, down to `&&`-chained shell commands.
- **Home lab** — an always-on Intel N100 box running the bots, a GitHub Actions runner and Postgres in Docker, reachable over Tailscale.

## Stack

- **Backend** — Go (Gin, GORM), Node.js, Python, PostgreSQL, Docker
- **Frontend** — Next.js (App Router), React, TypeScript, Tailwind, Zustand
- **Games** — Cocos Creator, Capacitor
- **AI** — Claude Agent SDK, Claude Code / Codex, multi-agent workflows, TTS / image / video generation, FFmpeg
- **Ops** — Linux, Docker, GitHub Actions, Tailscale, self-hosting

## Contact

- LinkedIn — [tyron-nhat-anh](https://www.linkedin.com/in/tyron-nhat-anh-a484a4154/)
- Email — nguyennhatanh96@gmail.com
