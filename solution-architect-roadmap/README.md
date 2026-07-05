# 🏛️ Solution Architect + AI — 35-Day Roadmap

A shared, trackable roadmap for two (or more) developers growing from Full Stack Developer → Enterprise Solution Architect, with AI architecture as a first-class discipline — not an afterthought.

**Live roadmap page:** enable GitHub Pages (see [SETUP.md](SETUP.md)) and this becomes `https://<your-username>.github.io/<repo-name>/`

---

## 📦 What's in this repo

```
.
├── index.html            → the visual roadmap (deploys via GitHub Pages)
├── docs/
│   └── days.tsv          → machine-readable day list (day, title, focus, phase)
├── labs/
│   └── day-01 … day-35   → one folder per day: checklist + space for your code/notes
├── scripts/
│   └── create_issues.sh  → bulk-creates a GitHub Issue per day using `gh` CLI
├── .github/
│   └── ISSUE_TEMPLATE/day.md → template for manually adding a day's issue
├── SETUP.md              → step-by-step: hosting + project board + issues
└── CONTRIBUTING.md        → how you and your study partner work together
```

## 🚀 Quick Start

1. **Fork or clone this repo** — one of you creates it, the other is added as a collaborator (or forks + PRs).
2. Follow **[SETUP.md](SETUP.md)** to:
   - Turn on GitHub Pages (free hosting for `index.html`)
   - Create a GitHub Project board (Kanban: To Do / In Progress / Done)
   - Bulk-create the 35 day-issues with one script
3. Each session: open the day's issue, work through the lab in `labs/day-XX/`, check off the 18-point checklist, then move the card to Done.
4. Compare notes with your partner in the issue comments before moving on — teaching each other a concept back is one of the fastest ways to actually retain it.

## 🧭 Roadmap Phases

| Phase | Days | Focus |
|---|---|---|
| Foundations | 1–5 | CS fundamentals, OS, networking, SE principles |
| Architecture Core | 6–10 | Architecture styles, DDD, API design, system design |
| Data & Persistence | 11–16 | DB architecture, SQL Server, NoSQL, caching, messaging |
| Distributed & Cloud | 17–24 | Distributed systems, Azure, Docker, Kubernetes |
| DevOps & Infra | 25–28 | CI/CD, IaC, IIS/Windows Server, Linux |
| Security | 29–30 | AuthN/AuthZ, security architecture, governance |
| Quality & Ops | 31–33 | Testing, observability, performance, HA/DR, cost |
| Multi-Stack | 34 | Frontend architecture + polyglot backend trade-offs |
| **AI Capstone** | **35** | LLM fundamentals, RAG, vector DBs, agents, MLOps/LLMOps |

Then an **Advanced Track** (Principal Engineer / Enterprise Architect — no fixed day count) covering EA frameworks, platform engineering, FinOps, AI platform architecture, and leadership — see `index.html` for the full breakdown.

## 🤝 Growing Together

This repo is built for **two learners, one pace**. See [CONTRIBUTING.md](CONTRIBUTING.md) for the collaboration workflow — issue comments, PR-based lab submissions, and how to keep each other honest on the "no skipping days" rule.
