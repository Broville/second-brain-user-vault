# Second Brain — Obsidian Vault Template

A personal knowledge management system built in Obsidian. Designed to be maintained with the help of an AI assistant (Claude), but fully functional as a standalone Obsidian vault.

---

## Philosophy

- **One inbox, many domains.** Everything enters through `INBOX.md`. From there it gets routed to the right domain folder.
- **AI is the note-taker, not the brain.** You bring the knowledge; the AI structures, links, and maintains it.
- **Friction-free capture.** If capturing something is hard, it won't happen. Keep INBOX.md always open.
- **Daily 5-min loop.** The system only works if you touch it regularly. The loop is short on purpose.

---

## Setup

1. Clone this repo or use it as a GitHub template
2. Open the folder in [Obsidian](https://obsidian.md)
3. Enable the **Templates** core plugin and point it at the `templates/` folder
4. Enable **Daily Notes** if you want dated journal entries
5. Start with `maps/master-map.md` — it's your home base

That's it. No plugins required beyond Obsidian's built-in core plugins.

---

## Folder Structure

```
/
├── INBOX.md          — Capture anything here, no rules
├── PROJECTS.md       — Status dashboard for all active domains
├── OPEN_LOOPS.md     — Unresolved questions taking up mental RAM
├── REVIEW.md         — Scheduled revisit queue
├── CHANGELOG.md      — Optional session log
│
├── templates/        — Reusable note templates
├── domains/          — Your knowledge, organized by topic
│   ├── books/
│   ├── music/
│   ├── entertainment/
│   └── health/
│
├── maps/             — Navigation and index files
├── inbox/            — Capture overflow and staging
└── journal/          — Dated session logs
```

---

## The Daily Loop

Run this once a day — takes 5 minutes:

1. **INBOX.md** — Scan for anything captured. Route each item to the right domain or delete it.
2. **OPEN_LOOPS.md** — Flag anything that can be decided or closed.
3. **REVIEW.md** — Check for anything due this week.
4. **CHANGELOG.md** — Write one line about what you did today (optional but useful).

---

## Domains

Domains are topic-specific folders under `domains/`. Each domain has:

- `CONTEXT.md` — What the domain is, how it works, conventions
- Content files — Notes, reviews, logs, trackers, etc.

### Included example domains

| Domain | What it tracks |
|--------|---------------|
| `books/` | Reading list, reviews |
| `music/` | Album reviews, listening log |
| `entertainment/` | Movie and show backlog + watched history |
| `health/` | Goals, vitals, progress log |

### Adding your own domain

1. Create `domains/your-domain/`
2. Add a `CONTEXT.md` explaining the domain's purpose and conventions
3. Add a row to `PROJECTS.md`
4. Add a section to `maps/master-map.md`

---

## Frontmatter Conventions

Every note should include YAML frontmatter. This enables graph view, filtering, and search:

```yaml
---
title: "Your Note Title"
domain: books
status: active
tags:
  - review
---
```

**Status values:**
- `active` — in use, current
- `paused` — intentionally stopped
- `loop` — unresolved, needs attention (surfaces in your open loops review)

---

## File Naming

- Lowercase, hyphen-separated: `my-topic-name.md`
- Dates in ISO format: `2026-03-31.md`
- Reviews named after the subject: `project-hail-mary.md`

---

## Using AI with This Vault

If you use Claude (or another AI assistant) with this vault:

1. Point the AI at `maps/master-map.md` as the starting point
2. Tell it your active domains and what you're working on
3. Ask it to route INBOX.md items, write reviews, or add notes directly to the right domain

The `domains/` folder structure is intentionally AI-readable — each domain's `CONTEXT.md` explains the conventions so an AI can contribute correctly without being re-briefed every session.

---

## Templates

| Template | Use for |
|----------|---------|
| `Book Review.md` | After finishing a book |
| `Album Review.md` | After a full album listen |
| `Entertainment Review.md` | After watching a film or show |
| `Show Episode Log.md` | Tracking a show episode-by-episode |

Use Obsidian's **Templates** core plugin to insert them (`Ctrl+P` → "Insert template").
