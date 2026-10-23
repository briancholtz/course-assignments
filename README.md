# Course Assignments

Browser-based assignments for an undergraduate leadership course, published with
GitHub Pages.

**Live site:** https://briancholtz.github.io/course-assignments/

## Contents

| Assignment | Folder | URL |
|---|---|---|
| Cultural Diversity Awareness Questionnaire | `cultural-awareness/` | https://briancholtz.github.io/course-assignments/cultural-awareness/ |

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

## Cultural Diversity Awareness Questionnaire

32 statements rated 1–5 (1 = never, 5 = always). The total is the **straight sum
of all 32 responses**, range 32–160. There are no reverse-scored items and no
subscales.

| Score   | Interpretation   |
|---------|------------------|
| 130–160 | Very high range  |
| 100–129 | High range       |
| 70–99   | Moderate range   |
| 40–69   | Low range        |
| 32–39   | Very low range   |

Confirmed against the published instrument, which directs the reader to "sum the
numbers you circled." The range labels above are the published ones; the
textbook assigns no personality profiles.

The page shows the bottom band as 32-39 rather than the published 0-39, since 32
items rated 1-5 cannot total below 32.

Source: Questionnaire 9.3, "Cultural Diversity Awareness Questionnaire," from
*Introduction to Leadership*, ch. 9, "Embracing Diversity and Inclusion",
pp. 252-257. Adapted there from Special Populations and CTE Illinois Leadership
Project. (2016). *Cultural Diversity Self-Assessment*.

This page was first built from a spreadsheet copy whose scoring column was
broken (its total resolved to `#REF!`), whose reverse-scoring formulas
contradicted the printed interpretation, and whose wording had drifted from the
published text in ten items. All three were corrected against the source.

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
