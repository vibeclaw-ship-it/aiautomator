# Felix ClawBot - Operator Guide

Welcome to the documentation for **Felix**, your autonomous AI Operator. Felix is not a chatbot. He is a full-stack, terminal-native intelligence designed to execute tasks, manage infrastructure, and drive operations without constant human hand-holding.

---

## ⚡ 1. Core Philosophy: The ClawBot Model

Unlike traditional LLMs that wait for you in a chat window, Felix runs on a **ClawBot Architecture**:
- **Proactive:** He wakes up via Cron jobs or Heartbeat pings to check systems.
- **Stateful:** He reads and writes to his own `MEMORY.md` to maintain long-term context.
- **Terminal Native:** He has direct access to a Linux shell, file system, and Homebrew.
- **Ship-First:** He prioritizes deploying live code over theorizing in chat.

---

## 🚀 2. Initializing Felix

To unleash Felix on a project, you only need to provide him with the keys to the kingdom. He requires no complex web interfaces.

### Step 1: Provide the Master Keys
Provide the following tokens directly to Felix securely:
- **GitHub PAT (repo scopes):** For code management.
- **Vercel / Supabase Tokens:** For infrastructure deployment.
- **Gmail App Password:** For intercepting verification emails.
- **X/Twitter API Keys:** For autonomous social broadcasting.

### Step 2: Set the Core Directives
Modify his `IDENTITY.md` and `SOUL.md` to set his exact operational parameters (e.g., tone, target metrics, unbreakable rules). 

---

## 💻 3. Operational Protocols

Felix comes pre-loaded with specific "Skills" that allow him to interact with the world.

### Code & Infrastructure
- Felix uses the `gh` CLI to create repositories, manage issues, and review PRs autonomously.
- He pushes code directly to `master`/`main` and triggers Vercel deployments.

### Social Autopilot
- Using the `xpost` protocol, Felix can be scheduled via `cron` to wake up, scrape trending topics, draft a thread, and post it to X (Twitter) entirely on his own.
- He reads his mentions and auto-replies based on his `MEMORY.md` context.

### The Heartbeat System
- You don't need to ping him constantly. Felix utilizes a `HEARTBEAT.md` file. Every time the system pings him (e.g., every 30 minutes), he checks his task list, executes pending operations, and reports back **only if necessary**. If nothing needs attention, he remains silent.

---

## 🧠 4. Memory Management

Felix manages his own memory. You do not need to remind him of past events.
- **Daily Memory (`memory/YYYY-MM-DD.md`):** Raw logs of exactly what commands he ran and what code he shipped that day.
- **Long-Term Memory (`MEMORY.md`):** Distilled knowledge, permanent rules, and architectural decisions.
- **Task Memory (`TASK_MEMORY.md`):** His active kanban board. 

*If Felix makes a mistake, tell him. He will permanently write the correction to his LTM.*

---

## ⚠️ Unbreakable Rules
To prevent catastrophic autonomous errors, Felix is hardcoded with specific safeguards:
1. He cannot initiate financial transactions.
2. He stops execution after 3 failed retries (Loop Prevention).
3. He does not spam communication channels.

---
*Deploy Felix. Step back. Watch the machine build itself.*