---
site: tonytinkers.com
updated: 2026-08-18
---

# Site intro

A running log of the things I build on the side — mostly small, purpose-built
apps for me and the people around me. I use github to store my work. https://github.com/aallevena

---

# Frosthaven Journal

- **Status:** User Acceptance Testing
- **URL:** https://frosthaven.tonytinkers.com
- **Tagline:** A scrapbook-style companion for our Frosthaven board game campaign — a timeline of what happened, and a tavern view of where the party stands, both built off the same event log. The goal is we remember the narrative across multi-week breaks. I imagine I could spin this off to other journalling relevant proejcts.

## What it does
- Timeline & journal of scenarios completed, characters retired, buildings built, and town events — filterable by character or scenario
- The Tavern: a live snapshot of buildings, unlocked/completed scenarios, prosperity, and the roster, editable directly or derived from logged events
- PDF export of the journal as a keepsake, filterable by date range or character
- One shared party passphrase — no individual accounts to manage

## Built with
Next.js, Supabase, Postgres, Puppeteer

## On the bench
Preview-environment env vars aren't set up yet — fine for now since everything ships straight to production off `main`.

---

# Goal Tracker

- **Status:** Live
- **URL:** https://goals.tonytinkers.com
- **Tagline:** Weekly and monthly goal tracking — a GitHub-contributions-style heatmap of what actually got done, plus an API so my other agents can read and log goals directly.

## What it does
- Success heatmap and tag breakdown across weekly, monthly, and time-bounded goals
- Per-user API keys so AI agents can create and read goals alongside the browser session. AI-native users never have to use the UX if they don't want to.
- Google OAuth sign-in, restricted to an email allowlist — invite only experience ;)
- Full goal API: create, update, delete, and pull stats by tag or time window

## Built with
Next.js, Prisma, Postgres, Auth.js, Recharts

## On the bench
Nothing! I consider this production.

---

# The Hunt

- **Status:** Development
- **URL:** https://thehunt.tonytinkers.com
- **Tagline:** A location-based scavenger hunt platform — browse, play, and create hunts made of clues tied to a place and a way to verify you found it.

## What it does
- Browse and search public hunts, filterable by tag and sortable by upvotes or recency
- Play ordered hunts (solve a clue to unlock the next) or unordered hunts (any order), verified by password or geolocation
- Create, edit, and publish your own hunts and clues once signed in
- Google sign-in, upvotes, and a profile of hunts completed, in progress, and created

## Built with
Next.js, Prisma, Postgres, Auth.js

## On the bench
QR/barcode and photo-match clues, live shared events with a leaderboard, and badges are designed into the data model but deferred to phase 2.

---

# Timeline

- **Status:** Development
- **URL:** https://timeline.tonytinkers.com
- **Tagline:** A private, invite-only app for logging family events — births, marriages, relocations, jobs — and seeing how everyone's lives line up across time, place, and age.

## What it does
- CRUD for people and life events, with flexible date precision (day, month, or year)
- Chronological timeline view of everyone tracked
- Age-comparison view for lining up two people's lives side by side. When did Ben Franklin really hit his stride?
- Google sign-in with invite-code access control and role-based permissions

## Built with
Next.js, Prisma, Postgres (Supabase), Auth.js

## On the bench
CSV/PDF export, a geographic movement map, relationship cross-paths, progeny timeline analysis, event photos, and AI-assisted event ingestion.

---

# Footer

- **Left:** Built & maintained by Tony

<!--
HOW TO USE THIS FILE:
- Each project is its own "# Heading" section with the same fields: Status, URL, Tagline,
  What it does (bullets), Built with (comma list), On the bench (one note).
- To add a new project, copy a whole project section (from "# Name" down to the next "---")
  and fill in your own fields.
- To remove a project, delete its whole section.
- Send the edited file back and it'll be rebuilt into the portfolio page.
-->
