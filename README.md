# Course Assignments

Browser-based assignments for an undergraduate leadership course, published with
GitHub Pages.

**Live site:** https://briancholtz.github.io/course-assignments/

## Contents

| Assignment | Folder | URL |
|---|---|---|
| Cultural Diversity Awareness Questionnaire | `cultural-awareness/` | https://briancholtz.github.io/course-assignments/cultural-awareness/ |
| Transformational Leadership Inventory (adapted) | `transformational-leadership/` | https://briancholtz.github.io/course-assignments/transformational-leadership/ |
| Ethical Leadership Style Questionnaire | `ethical-leadership/` | https://briancholtz.github.io/course-assignments/ethical-leadership/ |

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

## Transformational Leadership Inventory (adapted)

28 items rated 1-7 (1 = strongly disagree, 7 = strongly agree). Scored as seven
dimension averages, not a total. Items **3, 11 and 17 are reverse-scored** (a
rating of v counts as 8 - v).

| Dimension | Items | n |
|---|---|---|
| Articulating a Vision | 4, 12, 18, 20, 24 | 5 |
| Providing an Appropriate Model | 5, 8, 26 | 3 |
| Fostering Acceptance of Group Goals | 16, 22, 25, 28 | 4 |
| High Performance Expectations | 1, 10, 14 | 3 |
| Individualized Support | 3(R), 7, 9, 11(R) | 4 |
| Intellectual Stimulation | 19, 21, 23, 27 | 4 |
| Contingent Reward *(transactional)* | 2, 6, 13, 15, 17(R) | 5 |

The first six dimensions are transformational; contingent reward is transactional.
The source publishes no cutoff scores or norms, so the page asserts none - it shows
the profile across dimensions and says to compare them to each other.

**This is an adaptation.** The published instrument is worded for followers rating
a leader ("Has a clear understanding of where we are going"). Items here are
reworded to the first person for self-assessment, so the original validation
evidence does not directly apply. The page states this in its footer. Two further
wording changes: "employees" became "others", since students may not manage
anyone, and item 27's published text is missing a word ("some of basic
assumptions"), rendered here as "some of their basic assumptions".

Source: Podsakoff, P. M., MacKenzie, S. B., Moorman, R. H., & Fetter, R. (1990).
Transformational leader behaviors and their effects on followers' trust in leader,
satisfaction, and organizational citizenship behaviors. *Leadership Quarterly,
1*(2), 107-142. Items and factor structure from Table 3, pp. 118-119.

Unlike the MLQ, the TLI has no commercial licensor and is used in the literature
with citation.

## Ethical Leadership Style Questionnaire

Forced choice, not a rating scale. Ten situations, each with the same six
responses; the score for a perspective is the number of times its letter was
chosen, so the six scores always sum to 10.

| Letter | Perspective |
|---|---|
| A | Duty Ethics |
| B | Utilitarian Ethics |
| C | Virtue Ethics |
| D | Caring Ethics |
| E | Egoism Ethics |
| F | Justice Ethics |

The highest count is the student's primary or dominant style, the second-highest
next, and so on. Ties are common with only ten choices across six categories, and
the page reports them as ties rather than picking a winner. There are no cutoff
scores: the textbook states all perspectives have merit and there is no "best"
one, so the page asserts no ranking beyond the student's own counts.

**These are sample items** - the textbook prints an abridged version of a longer
instrument and points to www.leaderdecisionmakingsurvey.com for the full
questionnaire. The page says so in its footer.

Source: Application 11.3, "Sample Items From the Ethical Leadership Style
Questionnaire," from *Introduction to Leadership*, ch. 11, "Addressing Ethics in
Leadership", pp. 313-318.
