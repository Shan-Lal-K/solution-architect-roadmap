# ⚙️ Setup Guide

Everything here is **free**. No credit card, no paid tier required.

## 1. Create the repo

1. Go to [github.com/new](https://github.com/new)
2. Name it e.g. `solution-architect-roadmap`
3. Set it to **Public** (required for free GitHub Pages on personal accounts) or Private if you're on a paid/education plan
4. Upload this folder's contents (or `git init` + `git remote add` + `git push` from your machine)
5. Add your friend as a **Collaborator**: repo → Settings → Collaborators → Add people

## 2. Turn on free hosting (GitHub Pages)

1. Repo → **Settings** → **Pages** (left sidebar)
2. Under "Build and deployment" → Source: **Deploy from a branch**
3. Branch: `main`, folder: `/ (root)` → **Save**
4. Wait ~1 minute, then your roadmap is live at:
   `https://<your-username>.github.io/<repo-name>/`
5. Every time you push a change to `index.html`, the live page updates automatically.

> Alternative: **Netlify** or **Cloudflare Pages** — drag-and-drop the folder in their dashboard, also free, slightly faster redeploys. GitHub Pages is simplest since you're already using GitHub for issues/tracking.

## 3. Set up the Project board (Kanban)

1. Repo → **Projects** tab → **New project** → choose **Board** template
2. Create 3 columns: `To Do`, `In Progress`, `Done`
3. Once issues exist (next step), add them to the board — each day becomes a draggable card

## 4. Bulk-create the 35 day issues

Requires the [GitHub CLI](https://cli.github.com/) (`gh`) — free, official GitHub tool.

```bash
# one-time setup
gh auth login

# from inside your cloned repo folder
bash scripts/create_issues.sh
```

This creates one issue per day (`Day 01: CS Fundamentals I` … `Day 35: AI System Architecture`), each with a checklist and a link to its `labs/day-XX/` folder.

**No `gh` CLI / prefer manual?** Use `.github/ISSUE_TEMPLATE/day.md` — click **Issues → New Issue** and pick the "Day Template," fill in the number/title/focus from `docs/days.tsv`, repeat 35 times.

## 5. Daily workflow (for both of you)

1. Open today's issue.
2. Work through the lesson (Claude teaches it) + hands-on lab in `labs/day-XX/`.
3. Fill in the 18-point checklist in that folder's `README.md`, commit your code/notes there.
4. Comment on the issue with what clicked / what didn't — this is the "grow together" part.
5. Move the card to **Done** on the Project board.
6. Only move to the next day once **both of you** have checked off the current one — see `CONTRIBUTING.md`.

## 6. Optional: notifications

Turn on **Watch → All Activity** on the repo (top right button) so you both get notified when the other comments or completes a day.
