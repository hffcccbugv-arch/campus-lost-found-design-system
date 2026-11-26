# Requirements and priorities

Project: design system for a campus service, Campus Lost & Found (Chapter 11 project).

Status: written with an AI assistant (Instinct) at the student's request, from the brief as the student pasted it in chat. The original instructions PDF was not available to the assistant, so each brief item below must be re-checked by the student against the original file. No user research was done. Section 2 is assumed, not researched.

## 1. Requirements taken from the brief

| ID | Requirement (from the brief as pasted) | Priority | Where it is met | Tests |
|---|---|---|---|---|
| B1 | Token layer named by role, with a measured contrast ratio for every colour pair | Must | css/tokens.css | T1, T11 |
| B2 | Base layer with a note for each rule | Must | @layer base, documentation section 2 | T20 |
| B3 | Twelve-column grid with spans, an offset, a nested row, one breakpoint justified from content | Must | @layer grid, documentation section 3 | T6, T7 |
| B4 | Two components, each with two variants, a size axis and states; at most four utilities; declared layer order; no !important | Must | @layer components and utilities | T2, T3, T4, T8, T9, T14 |
| B5 | One specification sheet per component and a governance note of about 200 words | Must | documentation sections 5 and 6 | T20 |
| B6 | Two proof pages checked at 320, 768 and 1400 px, and a temptation report | Must | index.html, report.html, sections 7 to 9 | T6 to T14 |
| B7 | Reflection written by the student | Must | documentation section 10 | none (student's own) |
| B8 | PDF of the documentation and report | Must | docs/P3_documentation_and_report.pdf | T17 |

## 2. Assumed user needs (not researched)

These are assumptions about who uses a campus lost-and-found. They were not collected from real users. The student should replace or confirm them with what he has seen on campus.

| ID | Assumed need | Priority | Design response |
|---|---|---|---|
| U1 | A person who lost something wants to see found items quickly | Must | Item cards on the first page, found and lost marked by name and stripe |
| U2 | A person must be able to report a lost or found item with few fields | Must | Report form with item, place, date, and lost or found |
| U3 | The pages must be readable on a phone | Must | Mobile-first layout, tested at 320 px |
| U4 | Text must be readable by people with low vision | Must | Contrast ratios measured for every colour pair |
| U5 | The pages must work without a mouse | Should | Visible focus ring, skip link, keyboard order tested |
| U6 | A dark theme for night use | Could | data-theme="night" changes tokens only |
| U7 | Arabic-capable fonts in the font stack | Could | Noto Sans Arabic in --font-body |

## 3. Priority rule

- Must: the brief requires it, or the service cannot work without it.
- Should: it protects accessibility but the brief does not name it.
- Could: nice to have, no loss if missing.

## 4. Not in scope

A real backend. The report form is a demo and nothing is sent or saved.
