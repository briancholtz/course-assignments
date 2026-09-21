# Course Assignments

Browser-based assignments for an undergraduate leadership course, published with
GitHub Pages.

**Live site:** https://briancholtz.github.io/course-assignments/

## Contents

| Assignment | Folder | URL |
|---|---|---|
| Cultural Awareness Inventory | `cultural-awareness/` | https://briancholtz.github.io/course-assignments/cultural-awareness/ |

The root `index.html` is the hub page students bookmark. Each assignment lives in
its own folder as `index.html`, so its URL stays short and stable.

## This repository is public

Everything committed here is visible to anyone, permanently — git keeps history,
so deleting a file in a later commit does not unpublish it.

**Do not commit:**

- Student submissions, grades, rosters, or anything naming a student (FERPA)
- Answer keys or scoring rubrics students should not see
- Draft or unreleased assessments

Anything in those categories belongs in a separate private repository.

The assignments themselves are safe to publish: they are self-contained pages
that transmit nothing. Student responses stay in the student's own browser and
reach the instructor only through whatever the student pastes into Canvas.

## Adding an assignment

1. Create a folder, e.g. `conflict-style/`
2. Put the page in it as `index.html`
3. Add a card to the root `index.html`
4. Commit and push to `main` — Pages redeploys automatically

## Cultural Awareness Inventory

32 statements rated 1–5 (1 = never, 5 = always). The total is the **straight sum
of all 32 responses**, range 32–160. There are no reverse-scored items and no
subscales.

| Range   | Profile      |
|---------|--------------|
| 130–160 | Rebel        |
| 100–129 | Change Agent |
| 70–99   | Neutral      |
| 40–69   | Traditional  |
| 32–39   | Unaware      |

Derived from a spreadsheet version whose scoring column was broken (its total
resolved to `#REF!`) and whose reverse-scoring formulas contradicted the printed
interpretation bands. The straight sum is what those bands describe.

### Degrading without JavaScript

Some learning management systems strip `<script>` tags from uploaded HTML. The
page is built so its core survives that: all 32 questions are static markup,
answer highlighting is pure CSS, and the running total plus the per-item readout
are computed with CSS counters and `:has()`.

Where scripts are blocked, students read their score off the page and type it in.
Where scripts run — as on this Pages site — they get band detection, saved
progress, and one-click copy of a paste-ready submission.

## Editing

Each page is a single self-contained HTML file. No build step, no dependencies,
no framework. Open it in any text editor.

Submission instructions are marked with `EDIT ME` comments.
