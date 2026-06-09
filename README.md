# Newbury North — Construction Workspace

A single-page, CompanyCam-style dashboard built for Newbury North Associates' construction team by The Ain Hub at FGCU. One responsive HTML file, eight tabs, runs in any modern browser.

**Tabs:** Today · Projects · Timeline · Photos · Punch List · Submittals · Report · Crew

## Running locally

Just open `index.html` in a browser — no build step, no dependencies.

## Running on Replit

This repo is set up to deploy as a static site on Replit:

1. Import this repo into Replit.
2. Run it — `npx serve` will serve `index.html` on the assigned port.
3. (Optional) Promote to a Replit Deployment for a permanent URL + password protection (requires Replit Core).

## Heads up about data

The dashboard stores all data — projects, logs, photos, punch items, submittals — in the **browser's `localStorage`**. That means:

- Data lives on whichever device opened the page. It does not sync across phones, tablets, or computers.
- Clearing browser data wipes the dashboard.
- This is fine for individual use right now; a shared backend (Supabase / Firebase) is the next phase.

## Editing the dashboard

The canonical source is `index.html`. The workspace also has a working copy at:

```
Current Clients/Newbury North/NNA Builds/NNA Construction Workspace.html
```

When the source copy changes, replace `index.html` here and push.

## What's not in this repo

- Newbury North's confidential briefings, client docs, John Eder photo archive, and ShareSync credentials.
- The 7 Claude Code skills (`nna-daily-log`, `nna-punch-list`, `nna-photo-tagger`, etc.) — those live in the workspace under `.claude/skills/` and the `nna-tools` plugin bundle, not in this deploy repo.
