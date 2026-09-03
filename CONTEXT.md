# adobe/react-spectrum context
> refreshed 2026-09-03 | upstream default: main @ 5df68d8bb9a920e56e49526c42ea073ffe6c7e3f

## Identity & policies
- upstream: adobe/react-spectrum, default branch main, primary language TypeScript, English-first (yes — docs/issues/UI all English).
- CLA: Adobe CLA required for all third-party contributions (one-time sign at opensource.adobe.com/cla.html). Promotion prerequisite only; fork PRs don't run the CLA bot.
- AI-assisted PR policy: allowed — CONTRIBUTING has an "AI-assisted contributions" section and points assistants at AGENTS.md. Fork PR bodies carry no AI mention (disclosure happens only at Oli's manual upstream promotion).
- signed commits required: no.
- PR template: .github/PULL_REQUEST_TEMPLATE.md (fill verbatim; checklists ticked only when genuinely satisfied).
- external tracker: github.

## Conventions (verified from merged PRs)
- branch naming: mixed — kebab-case dominant for fixes (`fix-navigation-docs`, `fix-menu-docs-typeahead`, `fix-actionbutton-group`), some snake_case (`fix_navigation_docs`, `fix_translation_script`). Use `fix-<kebab>` for doc fixes.
- commit style: Conventional Commits (`docs:`, `fix:`, `feat:`).
- test command: `yarn test` (Jest), `yarn test:ssr`, `yarn test:browser`; lint `yarn lint` (oxlint + format + type-check + constraints).
- CI gates merge: lint, type-check, unit tests, Chromatic VRT (maintainers run VRT themselves).

## Maintainer picture
- active maintainers: devongovett, snowystinger, reidbarber, LFDanLu, ktabors, yihuiliao — very responsive (131 merged PRs in 60d, 8 distinct external contributors in last 30 merged).
- maintainers are strict about duplicates: they close duplicate PRs and admonish contributors to check for existing PRs before opening. Dedupe hard.

## Issue-area health
- Large open backlog (33 open good-first-issue/help-wanted). Many concrete bugs are claimed by open PRs or maintainer-contested. Trivial doc/typo cleanup is uncontested and low-risk.

## Gap ledger (dedupe — READ FIRST, never re-pick)
- `2026-08-26` #10468/#10471 (S2 TableView :has(), Virtualizer rounding) — dropped (no-genuine-fix-this-cycle): #10468 already fixed+merged upstream (#10469); #10471 claimed by open PR #10489. Swept backlog; everything concrete claimed/contested.
- `2026-09-03` self-found doc typos (13 fixes, 10 files: CONTRIBUTING + release notes + s2-docs + rfcs/2022-v3-resizable-columns) — pr-opened (fork PR, base=fork main, head fix-docs-typos). Deduped: no upstream PR touches these strings.

## Mined gaps (discovered, not yet attempted)
- `2026-09-03` doc typos in specs/accessibility (Table.mdx "decendants", Tooltip.mdx "relys", api/Toast.md "Accesibility") and rfcs (dom-props "intentially"/"passsed", slots "underlaying") — status: proposed (not included in this PR; available for a future pass).
