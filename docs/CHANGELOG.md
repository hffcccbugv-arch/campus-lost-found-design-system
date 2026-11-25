# Changes in this revision

Visual result: unchanged. The six day-theme screenshots (index and report at 320, 768, 1400) are byte-identical to the previous ones.

## css/tokens.css
- Renamed numbered tokens to role names (values unchanged): --font-size-1..4 -> --font-size-small, --font-size-body, --font-size-subheading, --font-size-page-heading; --space-1..4 -> --space-compact, --space-base, --space-card, --space-section; --radius-1, --radius-2 -> --radius-control, --radius-card.
- Removed --duration-base (defined, never used).
- Contrast comments rewritten and extended: every pair the system uses, day and night, recomputed with the WCAG formula by script. Added focus on surface, accent on paper and surface (marked decorative only), ink on accent, paper vs surface (decorative), paper on ink (pressed button), and the night-theme pairs for accent and focus.

## css/main.css
- All var() references updated to the new token names.
- .card[aria-current="true"] replaced by .card[data-state="featured"] (outline now uses --color-brand, same value as before).
- Added @media (prefers-reduced-motion: reduce) { .btn { transition: none; } } in the components layer, right after .btn, so it wins over the .btn transition. No !important, layer order unchanged.

## index.html
- The featured card uses data-state="featured" instead of aria-current="true". aria-current="page" stays on the navigation links (report.html unchanged).

## docs/P3_documentation.html and PDF
- Token tables rewritten with the rename table, day and night ratios, decorative pairs.
- Section 2 rewritten: 20 base-layer rows (what each replaces in the browser default, measured in Chrome 157, or marked as new behaviour), including label, checkbox and radio, :user-invalid, reduced motion, transitions, header, footer, nav, skip link, focus-visible.
- Section 3 measurements updated from the final build; section 4 explains the aria-current change and the reduced-motion fix.
- Specification sheets updated (new names, data-state, reduced motion). Governance note rewritten, 202 words.
- Section 8 now has tests T1 to T20 with results; who did what table; not-run list.
- Reflection: the paragraph is marked as AI-generated and an empty box is left for the student. Temptation report: two new AI entries and an empty box for the student.
- Print layout: page breaks, tables inside the page, screenshots grouped so none is cut. Missing image index_night_768.png was regenerated.

## docs/shots
- All screenshots regenerated from the final files, plus the new index_night_768.png.

## Not changed
- index.html and report.html content and layout, the grid, the four utilities, the night theme values, tests/state_fixture.html.
