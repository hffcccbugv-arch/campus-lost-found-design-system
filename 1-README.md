# Campus Lost & Found: design system (Chapter 11 project)

A small design system for a campus lost-and-found service, and two proof pages built only from it.

- `css/tokens.css`: design tokens (colour, font, space, radius, duration), with measured contrast ratios in comments. A second token set (`data-theme="night"`) re-themes the pages without touching a component rule.
- `css/main.css`: declared layer order `@layer base, grid, components, utilities;` then the base (reboot), 12-column grid, components and four utilities. No `!important`.
- `index.html`, `report.html`: the two proof pages.
- `docs/P3_documentation_and_report.pdf`: specification sheets, governance note, tests, temptation report, reflection draft, requirement checklist.
- `tests/state_fixture.html`: test-only page for component states.

## Honest status
Built with an AI assistant (Instinct) at the student's request; the student must be able to explain every line. The reflection in the PDF is a draft for the student to edit. Not run: screen reader, second browser, touch device. See section 8 of the PDF for what was tested and by whom.
