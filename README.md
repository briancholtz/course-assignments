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
| Leadership Strengths Questionnaire | `leadership-strengths/` | https://briancholtz.github.io/course-assignments/leadership-strengths/ |
| Authentic Leadership Self-Assessment | `authentic-leadership/` | https://briancholtz.github.io/course-assignments/authentic-leadership/ |
| Emotional Intelligence Scale (WLEIS) | `emotional-intelligence/` | https://briancholtz.github.io/course-assignments/emotional-intelligence/ |
| Task and Relationship Questionnaire | `task-relationship/` | https://briancholtz.github.io/course-assignments/task-relationship/ |
| Conflict Style Questionnaire | `conflict-style/` | https://briancholtz.github.io/course-assignments/conflict-style/ |

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

## Leadership Strengths Questionnaire

30 items rated 1-5 (1 = very much unlike me, 5 = very much like me). Five
strengths of six items each, **summed** (not averaged), so each ranges 6-30.
No reverse-scored items and no overall total.

| Strength | Items |
|---|---|
| Implementer | 1, 6, 11, 16, 21, 26 |
| Innovator | 2, 7, 12, 17, 22, 27 |
| Encourager | 3, 8, 13, 18, 23, 28 |
| Analyzer | 4, 9, 14, 19, 24, 29 |
| Mediator | 5, 10, 15, 20, 25, 30 |

The same five ranges apply to every strength:

| Score | Interpretation |
|---|---|
| 26-30 | Very high range |
| 21-25 | High range |
| 16-20 | Moderate range |
| 11-15 | Low range |
| 6-10 | Very low range |

The textbook's stated purpose is to rank the five, so the page shows the profile
chart in fixed order and a separate list sorted strongest-first, with each
strength's range label. Ties for the top are reported as ties.

Source: Questionnaire 6.3, "Leadership Strengths Questionnaire," from
*Introduction to Leadership*, ch. 6, "Engaging Strengths", pp. 150-153.

## Authentic Leadership Self-Assessment

16 items rated 1-5 (1 = strongly disagree, 5 = strongly agree). Four dimensions
of four items each, **averaged** (range 1-5). No reverse-scored items.

| Dimension | Items |
|---|---|
| Self-Awareness | 1, 5, 9, 13 |
| Internalized Moral Perspective | 2, 6, 10, 14 |
| Balanced Processing | 3, 7, 11, 15 |
| Relational Transparency | 4, 8, 12, 16 |

The page reports the highest and lowest dimension (ties reported as ties), since
the reflection question asks which area to strengthen. An overall score is shown
as the average of the four, clearly labelled as a summary rather than a
separately published score.

**Built from the instructor's spreadsheet; no published copy was supplied.** The
item-to-dimension mapping was checked against item content and is coherent - each
item's wording matches its assigned dimension, all 16 are covered, none is
double-counted. Two things could not be verified and are flagged on the page:

- The spreadsheet **averages** each dimension to a 1-5 score. Published versions
  of this questionnaire are generally **summed**, giving 4-20 per dimension.
  Averaging and summing rank the dimensions identically, so the profile is the
  same either way; only the numbers differ.
- The interpretation guide ("around 4-5 high, around 3 moderate, around 1-2
  low") comes from the spreadsheet. Because it says "around", the page prints it
  as a guide and does not stamp a band label on any dimension.

Terminal periods were added to the item wording for consistency with the other
pages.

Source: Authentic Leadership Self-Assessment Questionnaire, Peter G. Northouse,
*Leadership: Theory and Practice*.

## Emotional Intelligence Scale (WLEIS)

16 items rated 1-5 (1 = strongly disagree, 5 = strongly agree). Four dimensions
of four items each, **averaged** (range 1-5). **No reverse-scored items.**

| Dimension | Items |
|---|---|
| Self-Emotions Appraisal (SEA) | 1, 2, 3, 4 |
| Others-Emotions Appraisal (OEA) | 5, 6, 7, 8 |
| Use of Emotion (UOE) | 9, 10, 11, 12 |
| Regulation of Emotion (ROE) | 13, 14, 15, 16 |

This is the standard WLEIS structure and matches the instructor spreadsheet's
own dimension formulas, which were used as-is.

### What was not reproduced from the spreadsheet

- **Stray reverse scoring.** A vestigial column applied `LOOKUP(...{5,4,3,2,1})`
  to items 6 and 12. Both are positively worded ("I am a good observer of
  others' emotions", "I would always encourage myself to try my best") and the
  WLEIS has no reverse-scored items. That column fed nothing, so the sheet's
  own output was unaffected, but it is not carried over here.
- **Three broken cells** dividing empty cells by 10, and a column of item codes
  (`N1`, `P3`, `M7`, ...) belonging to some other instrument.

### Flagged, not silently resolved

- The spreadsheet uses a **1-5** response scale. The published WLEIS is
  generally administered with **seven** points. The page follows the
  spreadsheet and says so in its footer.
- The interpretation guide ("around 4-5 high, around 3 moderate, around 1-2
  low") comes from the spreadsheet. Because it says "around", the page prints it
  as a guide and stamps no band label on any dimension.

Apostrophes were added to items 5 and 6 ("friends' emotions", "others'
emotions") and a terminal period to item 11.

Source: Wong, C. S., & Law, K. S. (2002). The effects of leader and follower
emotional intelligence on performance and attitude: An exploratory study.
*The Leadership Quarterly, 13*(3), 243-274.

## Task and Relationship Questionnaire

20 items rated 1-5 (1 = never, 5 = always). Two scores, each the **sum** of ten
items, so each ranges 10-50. No reverse-scored items and no overall total.

| Score | Items |
|---|---|
| Task | odd-numbered: 1, 3, 5, 7, 9, 11, 13, 15, 17, 19 |
| Relationship | even-numbered: 2, 4, 6, 8, 10, 12, 14, 16, 18, 20 |

The same four ranges apply to each score. Note the published set has four bands,
not the five the other Northouse questionnaires use, and names the second one
"moderately high" rather than "moderate":

| Score | Interpretation |
|---|---|
| 40-50 | High range |
| 31-39 | Moderately high range |
| 21-30 | Low range |
| 10-20 | Very low range |

The textbook frames the result as a **comparison** between the two scores, so the
page leads with both side by side and states which is higher and by how many
points. The textbook gives no cutoff for how close counts as "very similar", so
the page reports the gap and says no cutoff exists rather than inventing a
threshold for declaring a profile balanced. An exact tie is reported as equal.

Source: Questionnaire 4.3, "Task and Relationship Questionnaire," from
*Introduction to Leadership*, ch. 4, "Attending to Tasks and Relationships",
pp. 92-94.

## Conflict Style Questionnaire

The only two-rating instrument in the set. Every one of the 25 items is rated
**twice** - once for a conflict with Person A and once for a conflict with
Person B - so students give 50 ratings and each style yields two scores.
Comparing them is the textbook's stated purpose.

25 items rated 1-5 (1 = never, 5 = always). Five styles of five items each,
**summed** (range 5-25) per person. No reverse-scored items and no overall total.

| Style | Items |
|---|---|
| Avoidance | 1, 6, 11, 16, 21 |
| Competition | 2, 7, 12, 17, 22 |
| Compromise | 3, 8, 13, 18, 23 |
| Accommodation | 4, 9, 14, 19, 24 |
| Collaboration | 5, 10, 15, 20, 25 |

| Score | Interpretation |
|---|---|
| 21-25 | Very strong style |
| 16-20 | Strong style |
| 11-15 | Average style |
| 6-10 | Weak style |
| 5 | Very weak style |

The textbook prints the bottom range as 0-5. Five items rated 1-5 cannot total
below 5, so 5 is the only score it can contain; the page shows 5 and says why.

The results name each person's most dominant style, whether the two match, and
which style shifts most between the relationships. Ties are reported as ties.
The page carries the textbook's caution that this is **not a personality test
that labels or categorizes you**, and that scores reflect one particular
conflict at one time.

### Chart colors

The two series needed a categorical palette, the only chart in the set that
does. Both modes were checked with the dataviz validator and pass all five
checks against their own surface: light `#149184` / `#b8801c`, dark `#14a08f` /
`#b2882a`. A legend is always shown, and every bar carries a direct value label.
Bars are drawn from 0 rather than from the 5-point floor, so a style at its
minimum still renders a visible bar instead of nothing.

Source: Questionnaire 10.3, "Conflict Style Questionnaire," from *Introduction
to Leadership*, ch. 10, "Managing Conflict", pp. 288-290. Adapted there from
Rahim, M. A., & Magner, N. R. (1995), *Journal of Applied Psychology, 80*(1),
122-132; in Wilmot, W., & Hocker, J. (2011), *Interpersonal Conflict*,
pp. 146-148.
