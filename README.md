# VC Social Hub

A social media work tracking dashboard for Vantage Circle's marketing team. Plan, track, and manage content across LinkedIn, Reddit, and Instagram — with personal branding sections for executive thought leadership.

**Live:** [deepmoneyy07.github.io/social-media-tracker](https://deepmoneyy07.github.io/social-media-tracker/)

---

## Features

### Dashboard Overview
- Quick stats: total posts, published count, active reminders, strategies
- Today's scheduled posts at a glance
- Post status breakdown (Draft / Scheduled / Published)
- Upcoming reminders and active strategies

### Content Calendar
- Day-wise post planning across **LinkedIn**, **Reddit**, and **Instagram**
- Platform tabs for filtered viewing
- Each post includes: date, title, copy, caption, notes, status, and time
- **Notion-like detail overlay** — click any post to open a full editing view with auto-save
- **Bulk select & delete** — select multiple posts and delete in one action
- **Smart file import** — upload CSV, TSV, or Excel files with auto-format detection and fuzzy column mapping

### Strategy & Plans
- Add, edit, and delete strategies with status tracking (To Do / In Progress / Done)
- Filter by status
- Due dates and platform tagging

### Reminders
- Add reminders with date, time, and priority (High / Medium / Low)
- Filter: All / Pending / Done
- Mark reminders as complete

### Executive Personal Branding
- **Partha's Brand** — LinkedIn posts, thought leadership topics, posting schedule
- **John's Brand** — LinkedIn posts, thought leadership topics, posting schedule

---

## Tech Stack

- **Single-file HTML/CSS/JS** — no build tools, no framework, no dependencies
- **localStorage** for data persistence — works offline, instant saves
- **SheetJS** (CDN) for Excel/CSV import parsing
- **GitHub Pages** for hosting via GitHub Actions

---

## Project Structure

```
.
├── index.html                  # Main dashboard (all HTML/CSS/JS)
├── seed-data.js                # Q2 2026 pre-loaded content calendar (36 posts)
├── README.md                   # This file
├── LICENSE                     # MIT License
├── .gitignore                  # Git ignore rules
├── .github/
│   └── workflows/
│       └── pages.yml           # GitHub Pages auto-deployment
├── Documents/
│   ├── Content-Calendar/       # Q2 content calendar & framework analysis
│   ├── Plans/                  # Reddit strategy & marketing plans
│   └── Rewards-and-Recognition/# Vantage Rewards platform docs
├── Skills/
│   ├── vantage-circle-social-copywriting/   # Social copywriting skill
│   ├── vantage-circle-content-strategy/     # Content strategy skill
│   ├── vantage-circle-reddit-skill/         # Reddit marketing skill
│   └── vantage-circle-engagement-intelligence/ # Engagement intel skill
└── Install/
    └── *.skill                 # Packaged skill files for Claude Code
```

---

## How It Works

### Data Flow
1. **First visit** — Dashboard loads seed data from `seed-data.js` (Q2 2026 content calendar with 36 pre-written posts)
2. **User makes changes** — Edits, additions, and deletions save instantly to `localStorage`
3. **Subsequent visits** — Data loads from `localStorage`, seed data is ignored
4. **New browser/device** — Gets fresh seed data, then localStorage takes over

### Content Calendar Seed Data
The Q2 2026 calendar includes 36 posts across 3 platforms (April-June):
- **12 LinkedIn posts** — AIDA, BAB, PAPA frameworks with VC brand voice
- **12 Reddit posts** — PAS framework, community-first tone for r/humanresources
- **12 Instagram reels** — Timestamped reel scripts with captions and hashtags

All posts include full copy, captions, internal notes with framework metadata, and optimal posting times.

---

## Deployment

The dashboard auto-deploys to GitHub Pages on every push to `main` via the workflow in `.github/workflows/pages.yml`.

To deploy manually:
```bash
git add -A
git commit -m "Update dashboard"
git push origin main
```

---

## Local Development

Serve the project locally:
```bash
npx serve . -l 5555
```
Then open [http://localhost:5555](http://localhost:5555)

---

## Skills & Documents

### Claude Code Skills
Custom skills for Vantage Circle content creation (located in `Skills/`):

| Skill | Purpose |
|-------|---------|
| **Social Copywriting** | Platform-specific posts with VC brand voice (LinkedIn, Reddit, Instagram, Twitter, Email) |
| **Content Strategy** | Brand guide, content library (959 posts), messaging frameworks, SEO |
| **Reddit Marketing** | Authority posts, community analysis, case studies, lead qualification |
| **Engagement Intelligence** | Monthly market intel: Reddit pain points, LinkedIn trends, research synthesis |

### Strategy Documents
Located in `Documents/`:
- **Q2 2026 Content Calendar** — Full multiplatform calendar with themes, frameworks, and lead magnets
- **Reddit Strategy** — 3-skill ecosystem plan for Reddit authority building
- **Rewards & Recognition** — Vantage Rewards platform documentation

---

## Brand Guidelines

- **Colors:** Dark professional UI with purple/violet accents (#6d5cff)
- **Voice:** Data-driven, authentic, problem-first (never corporate-speak)
- **Core message:** Peer recognition drives 20%→60% adoption, 18-23% retention improvement
- **Differentiator:** Peer-first, values-tied, frictionless recognition culture

---

## License

MIT License. See [LICENSE](LICENSE) for details.
