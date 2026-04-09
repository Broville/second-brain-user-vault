---
title: Books Domain — Context
domain: books
status: active
tags:
  - books
  - context
---
# Books Domain

> Track your reading, capture reviews while they're fresh, and build a personal reading log over time.
> Last updated: YYYY-MM-DD

---

## Purpose

A friction-free reading log. When you finish a book, capture your thoughts using the Book Review template before the details fade. Over time this becomes your own annotated library.

---

## Scope

- **Fiction** — novels, novellas, short story collections
- **Nonfiction** — essays, memoirs, reference, how-to
- **Out of scope** — audiobooks you passively listened to (optional to include — your call)

---

## How It Works

1. When you start a book: add a row to `MASTER_LIST.md` with status `reading`
2. When you finish: use the **Book Review** template (`templates/Book Review.md`) to create a review file
3. Update the row in `MASTER_LIST.md` to `read` with your rating
4. File the review as `domains/books/[slug].md` (e.g. `project-hail-mary.md`)

---

## Conventions

- **Status values:** `to-read` · `reading` · `read` · `abandoned`
- **Rating:** 1–5 (or whatever scale you prefer — just be consistent)
- **File naming:** lowercase, hyphen-separated title slug: `the-name-of-the-wind.md`

---

## Linked Files

- [`MASTER_LIST.md`](MASTER_LIST.md) — full reading log with status and rating
- [`../../templates/Book Review.md`](../../templates/Book%20Review.md) — review template
