# Hi, I'm Tyron 👋

Full-stack engineer from Vietnam. I ship things end-to-end — the API, the web app, the deploy — and lately I build a lot of them *with* AI agents rather than around them.

## 🌱 Currently learning

- **Robotics** — working up from electronics basics to ESP32 to small robots: sensors, motors, lithium power, an on-device voice assistant. I write up what I learn as [Bàn Ráp](https://bibaplay.com).
- **AI agents** — multi-agent orchestration, tool permissions and human-in-the-loop gates, keeping long-running agents cheap and safe to leave alone.

## Games & products

**[Tales of Ascension](https://play.google.com/store/apps/details?id=com.mgho.app)** · live on Google Play
Solo-built wuxia auto-battler card RPG. Next.js + Capacitor client, Go + PostgreSQL backend, Cocos Creator 3.8 combat engine.

**[Bàn Ráp](https://bibaplay.com)** · free, in Vietnamese · open source — [code](https://github.com/TyronNA/bibaplay)
Self-study electronics course for beginners — Ohm's law to ESP32 to robots. Every lesson has step-by-step breadboard pictures and a circuit simulator. The repo also holds the ESP32 robot firmware and its Gemini Live voice server.

## AI pipelines

The rule I build them by: deterministic code owns orchestration, retries and budgets; the model owns the judgement calls. Anything irreversible — a merge, a sent email, a submitted order — waits for a human.

| Pipeline | In → out |
| --- | --- |
| 🧑‍💻 **Multi-agent dev team in Slack** | a request in a Slack thread → PO / BA / Dev / Review sub-agents on the Claude Agent SDK → a PR in an isolated git worktree. GitHub and Jira are in-process tools; merging or approving a PR pops ✅ / ❌ buttons back into the thread. One long-lived session per thread, resumed across restarts. |
| 📋 **Ticket → plan → code** | a daemon watches the Jira board, works out which services a ticket touches and writes a versioned implementation plan. Approval must name the exact plan version a human read; only then does it implement, with per-task budget caps and bounded fix loops. |
| 📧 **Email intake agent** | customer order emails in a shared mailbox → structured orders in a Postgres review queue → a human approves before anything is submitted. |
| 💬 **Ops assistant** | internal chatbot (FastAPI + Gemini) that answers questions about live orders and drivers through read-only API tools, plus a code-knowledge index — docs, call graph and semantic search — over the backend services. Tool-loop limits and duplicate-call suppression built in. |
| 🎬 **History video pipeline** | a topic → researched script → voice → shots → finished MP4, for two YouTube history channels. Editorial rule changes are blind-judged against a narrative benchmark before they ship. |

## Agents & tooling

- **Dev Hub** — VS Code extension that runs Claude Code and Codex sessions across many repos from one window, plus a mobile web view to follow them from my phone. Zero runtime dependencies.
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
