<div align="center">

![header](https://capsule-render.vercel.app/api?type=waving&color=gradient&height=130&section=header&fontSize=120)

<h1>pearl's Profile 🧐</h1>

**🔒 FDS Engineer** · Fraud Detection Systems
Building production fraud-detection pipelines by day, shipping AI-agent side projects by night.

<br>

[![Streak](https://streak-stats.demolab.com?user=pearlzzi98&theme=vue-dark)](https://git.io/streak-stats)

</div>

<br>

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| 📊 **Logging / Observability** | ELK (Elasticsearch, Logstash, Kafka), Filebeat, Grafana |
| 🗄️ **Datastores** | MariaDB, Redis, Elasticsearch |
| ⚙️ **Backend / Infra** | Node.js, Python, Docker Compose, Terraform, GCP, Tailscale, Cloudflare |
| 🤖 **AI** | Claude (Anthropic), agent tooling & automation |

<br>

## 🚀 Currently Building

> _A small personal cloud where my FDS/security instincts meet AI-agent tinkering. **devbox** is the always-on hub that develops and runs the other two. (repos private — descriptions below.)_

### 🖥️ devbox — always-on cloud dev hub
Moves my Claude Code workspace onto an always-on GCP VM so the session survives even when my local PC is off — laptop, phone, and browser are just stateless UI windows onto the same tmux session via Remote Control.
- **Stateless devices, stateful hub** — code execution, repos, secrets, and dotfiles all live on the VM; nothing runs locally
- **Locked-down by default** — no public ingress, Tailscale-only SSH, secrets injected at apply time (never committed)
- **Self-starting** — systemd user services + linger bring up tmux and the Remote Control servers on every boot
- **Stack** — Terraform (HCL) · Bash · PowerShell · Docker · GCP · Tailscale

### 🍁 MapleParty Bot — KakaoTalk open-chat party finder
A MapleStory party-recruitment bot driven by chat commands (`/create`, `/join`, `/kick`, `/delegate`), running an Android trust anchor against a containerized GCP backend.
- **Self-updating over RSA-signed bundles** — the phone polls the server for new bot logic and runs it only after **signature verification**, so it self-heals after a reboot with no ADB
- **Hands-off CI/CD** — one `main` push runs the integration tests, deploys to staging, smoke-tests, then promotes the *same commit SHA* to prod — no manual gate
- **Dual-runtime, hedged** — a MessengerBotR + Iris (redroid containerized Android) design so a break in one runtime can cold-fall-back to the other instead of taking the service down
- **Security & monitoring** — request/error counters, suspicious-path detection → Discord alerts, Redis-backed message stats on Grafana dashboards
- **Stack** — Node.js · Express · MariaDB · Redis · Caddy (auto-HTTPS) · Grafana · Docker Compose on GCP, over Tailscale

### 📻 Morning Briefing — TTS news alarm (PWA)
A PWA that wakes me with an alarm and reads the morning's curated news aloud — no paid API, no server.
- **Live:** https://morning-briefing-2dw.pages.dev/
- **How** — Google News RSS → **Google Cloud TTS (Chirp3-HD)** via a Cloudflare Worker key-proxy, with Web Speech API fallback
- **Curated** — three rotating themes I actually follow: AI/semiconductors/power, AGI & big-tech, and Seoul real estate
- **PWA** — installable, Service Worker background alarms, network-first HTML so new deploys land instantly
- **Stack** — Vanilla JS · Service Worker · Cloudflare Pages + Workers

<br>

## 🤖 Interests

| Topic | Details |
|-------|---------|
| 🧠 **AI Agents** | Autonomous & multi-agent architecture with Claude — wiring agents into real workflows |
| 🔐 **Agent Security** | Securing agents in production: prompt injection, tool misuse, privilege escalation, signed-code execution |
| 📈 **Detection & Monitoring** | Carrying FDS instincts (anomaly detection, alerting, dashboards) into side projects |

<br>

## 🌱 Off the Clock

| | |
|---|---|
| 🚴 **Cycling** | Weekly long rides (Zone 2–5) |
| 💪 **Gym** | 3–4×/week — cable row, lat pull, pec fly, rear delt |
| 🎮 **Gaming** | PC: DBD, GTA5 (GTA6 soon) · Mobile: MapleStory |

<br>

<div align="center">

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&height=130&section=footer&fontSize=120)

</div>
