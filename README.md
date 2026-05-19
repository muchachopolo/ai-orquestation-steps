# AI Orchestration Methodology — Teaching Guide

A single-page interactive tutorial that teaches team members how to use Claude Code CLI to orchestrate AI agent teams for building complete products.

**Live:** [GitHub Pages link after deployment]

## How to Run Locally

```bash
npm install
npm run dev     # Opens http://localhost:3000
```

## How to Deploy

Push to `main` — GitHub Actions deploys to GitHub Pages automatically.

---

## Presentation Script

Use this as your speaking guide when presenting this page to your team. Each section corresponds to a section on the webpage.

### Opening (2 min)

> "I want to show you how I've been using AI to build entire products — not just get code suggestions, but orchestrate full development teams autonomously. In our last project, I typed about 20 short prompts across a few sessions and got: 10 documentation files, 11 implemented sprints, 3 installable PWAs, and a full CI/CD pipeline. Let me show you how."

**Show:** Hero section with the stats.

---

### What is Claude Code CLI? (3 min)

> "Claude Code is different from ChatGPT or Copilot. It runs in your terminal, has full access to your project, and can spawn sub-agents — specialized AI workers that operate in parallel. Think of it like hiring a team on demand. You become the product owner, not the developer."

**Show:** The "What is Claude Code?" section. Walk through prerequisites.

**Key point:** "You don't need to know how to code to use this. You need to know how to define what you want."

---

### The Core Philosophy (3 min)

> "Three principles make this work:"
>
> 1. **Documentation first** — "We never write code before documenting. The AI needs context to make good decisions. Without documentation, it guesses. With documentation, it executes."
>
> 2. **Agent teams, not solo** — "We don't ask one AI to do everything. We define specialized roles: architects who design, developers who implement, QA who tests. They check each other's work."
>
> 3. **Autonomous execution** — "Once the rules and docs are solid, we tell it to go. No approval needed for each file. The pipeline IS the quality control."

**Show:** The 3 cards in the Philosophy section.

---

### The 8-Step Process (10 min)

Walk through each step on the page. Key moments:

**Step 1 — Business Problem:**
> "Notice I'm not talking about tech here. I'm describing the problem like I'd tell a friend. The AI figures out the actors, the constraints, the flows. You describe WHAT, it figures out HOW."

**Step 2 — Agent Orchestration:**
> "This is the secret. Before any code, I ask Claude to write the rules for its own team. Who are the agents? What's the pipeline? What's forbidden? This becomes law."

**Step 5 — THE MAGIC PROMPT (emphasize):**
> "This is where it gets crazy. I type one sentence and walk away. Claude reads the roadmap, spawns architects, gets designs validated, implements features, writes tests — sprint after sprint. I come back to a working product."

**Step 6 — Nudges:**
> "Sometimes it gets stuck — context fills up, sessions restart. A one-liner like 'continue' or 'you seem stuck' is enough. The rules in CLAUDE.md survive every restart."

---

### CLAUDE.md Deep Dive (5 min)

> "This file is the brain of the operation. Every agent, every sub-agent, every new session — they ALL read this file first. It's your project constitution. Put your tech stack, your rules, your UX philosophy, your orchestration pipeline in here. The more specific, the better the output."

**Show:** The code block with the CLAUDE.md structure.

**Demo idea:** Open your terminal, show a real CLAUDE.md, show how agents reference it.

---

### Prompt Patterns (5 min)

> "Notice how short my prompts are. The magic isn't in writing long, detailed prompts. It's in having great documentation that the AI already loaded. My prompts are just triggers."

**Click through each accordion:**
- The Business Story — "describe problems, not solutions"
- The Constraint Injection — "short, imperative, permanent"
- The Architect Invocation — "review before implementing"
- The Unleash Command — "the moment you let go"
- The Infrastructure Ask — "describe constraints, not solutions"

---

### Common Mistakes (3 min)

> "These are the traps I fell into and that you'll fall into too:"

Walk through each mistake. The big ones:
- **Starting with code** — "everyone's instinct, always wrong"
- **Autonomy without rules** — "chaos, not productivity"
- **Micromanaging** — "defeats the purpose"

---

### Results & Quick Start (3 min)

> "Here's what 20 prompts produced. And here's the template you can copy for your next project. The sequence matters — don't skip steps."

**Show:** Results stats, then the Quick Start code block.

---

### Closing (2 min)

> "The key takeaway: invest 80% of your time in documentation and 20% in prompts. A well-documented project runs on 'continue' and 'don't stop'. You're not writing code — you're directing a team. Think like a CTO, not a developer."

**Q&A:** Open for questions.

---

## Presentation Tips

- **Total time:** ~35 minutes + Q&A
- **Best format:** Live demo alongside the page. Have a terminal with Claude Code ready to show real agent spawning.
- **Avoid:** Showing your actual business project (keep examples generic)
- **Emphasize:** That this works for ANY tech stack, not just Laravel/React
- **Demo suggestion:** Start a fresh project live, type the business problem, show how Claude generates documentation in real-time
- **Audience engagement:** Ask them what business idea they'd use, then show how to phrase it as a first prompt

## Tech Stack

- Single HTML file
- TailwindCSS via CDN
- Google Fonts (Inter + JetBrains Mono)
- Zero build step
- Deployed via GitHub Pages
