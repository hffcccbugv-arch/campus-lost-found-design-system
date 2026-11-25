# Campus Lost & Found: design system (Chapter 11 project)

A small design system for a campus lost-and-found service, and two proof pages built only from it.

- `css/tokens.css`: design tokens (colour, font, space, radius, duration), named by role (for example `--space-card`, `--radius-control`, `--font-size-page-heading`), with measured contrast ratios in comments, day and night. A second token set (`data-theme="night"`) re-themes the pages without touching a component rule.
- `css/main.css`: declared layer order `@layer base, grid, components, utilities;` then the base (reboot), 12-column grid, components and four utilities. No `!important`.
- `index.html`, `report.html`: the two proof pages.
- `docs/P3_documentation_and_report.pdf`: base-layer table, specification sheets, governance note, tests, temptation report, reflection, requirement checklist. Source: `docs/P3_documentation.html`. Every change in the latest revision is in `docs/CHANGELOG.md`.
- `tests/state_fixture.html`: test-only page for component states.

## Honest status
Built with an AI assistant (Instinct) at the student's request; the student must be able to explain every line. The reflection and the student's own temptation entries in the PDF are left empty for the student to write; the AI-written text next to them is marked as AI-generated. Not run: screen reader, second browser, touch device. See section 8 of the PDF for what was tested and by whom.
