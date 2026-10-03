# Aster Health Plan Search and Selection

A business analysis portfolio case study for a mobile health plan search experience. The work documents the journey from discovery and requirements through design, process analysis, solution mapping, and UAT preparation.

> **Project status:** Portfolio case study and requirements/design package. UAT cases are prepared but have not been executed. This repository is not a production application and does not represent an official Aster Health release.

## Project overview

Aster Health wants to make it easier for members to find and compare health plans through a mobile experience. The current project slice focuses on helping an authenticated member search the plan catalogue using required geographic criteria and selected plan preferences, review matching plans and cost-sharing information, then choose a plan-specific next step.

The source brief describes a broader mobile application. This case study is deliberately limited to the Plan Search and Selection module so its requirements and acceptance boundary remain clear.

## Member journey

1. Open Plan Search in the authenticated app.
2. Select required location criteria. State and City are required; source materials conflict on whether the third required geography is County or Country, so that rule remains open.
3. Choose an approved plan type and select one or more essential health benefits.
4. Submit the search and review matching plans, plan details, benefits, and approved cost-sharing information.
5. For a specific result, either use its **Talk to a Representative** phone link or follow its **Enroll** hyperlink. Each action must stay associated with the same plan row.
6. The module ends at the external enrollment handoff. Enrollment forms, navigation, and completion are outside this project slice.

## Scope

### Included

- Search criteria and required-field validation.
- Geographic selectors and their dependency rules, once approved.
- Plan-type selection and multi-select essential health benefits.
- Search request and plan catalogue response mapping.
- Results, plan details, no-match, error, and retry states.
- Plan-specific representative phone and enrollment hyperlinks.
- Accessibility, supported mobile platforms, privacy, and UAT considerations.

### Excluded

- Enrollment forms, enrollment decisions, or enrollment completion.
- Eligibility, coverage checks, claims, care finding, cost estimation, appointments, or teleconsultation.
- Acceptance testing of the external call center or enrollment destination.

## BA work represented

The project follows the BA workflow used across the portfolio: requirements and traceability; stakeholder survey and mapping; epics, user stories, specifications, and prioritization; wireframes and process flows; business, product, functional, and system requirements; collaborative Miro workshop material; As-Is and To-Be BPMN; gap analysis; solution mapping; and UAT planning.

The PRD is included as a product-level companion to the BRD, FRD, and SRS. Traceability IDs, story estimates, and proposed backlog states are working artifacts; they should not be treated as approved delivery commitments until stakeholders sign off.

## Project links

- **GitHub repository:** [Aster-health-plan-search](https://github.com/YashhBodhare/Aster-health-plan-search)
- **Google Drive project folder:** [Open the Aster Health project folder](https://drive.google.com/drive/folders/19yGp4mJGz6Py4eaNvigEeH4AsK6uBC5q?usp=sharing)

## Repository guide

- [`docs/DELIVERABLES.md`](docs/DELIVERABLES.md) — artifact inventory, suggested folders, and transfer status.
- [`docs/GITHUB-PUBLISHING.md`](docs/GITHUB-PUBLISHING.md) — steps to create and push the repository.
- [`docs/OPEN-DECISIONS.md`](docs/OPEN-DECISIONS.md) — decisions that must be resolved before requirements are baselined or dependent tests run.
- [`docs/05-uat/Aster-Health-UAT-Plan.docx`](docs/05-uat/Aster-Health-UAT-Plan.docx) — UAT scope, roles, entry/exit criteria, severity guide, and sign-off.
- [`docs/05-uat/Aster-Health-UAT-Execution-Tracker.xlsx`](docs/05-uat/Aster-Health-UAT-Execution-Tracker.xlsx) — 26 unexecuted test cases and readiness gates.
- [`CONTRIBUTING.md`](CONTRIBUTING.md) — documentation change and review conventions.

## Important assumptions and evidence notes

- The stakeholder survey report and its 100-response dataset are **simulated portfolio data**, not evidence that 100 real members responded. Keep the word “Simulated” in their filenames and labels if published.
- The As-Is process is an initial hypothesis based on the supplied project brief; validate it with Member Services before presenting it as an observed current-state process.
- Source documents use inconsistent geography and partner naming (including County/Country and TransTech/TransSec). See the open-decision log; do not silently normalize these conflicts.
- The UAT pack contains 26 cases, all marked **Not Started**. Tests that depend on unresolved rules must remain blocked until the expected behavior is approved.
- Use synthetic test data only. Do not commit real member, health, account, credential, or production integration data.

## Current status

The documented analysis and design artifacts are drafted. The next project steps are to resolve the open decisions, validate the As-Is workflow, reconcile requirement and decision identifiers across documents, approve a single baseline, then run UAT in an approved test environment. No production implementation or UAT execution is claimed here.

## Suggested next actions

1. Add the remaining artifacts from the inventory to their suggested folders.
2. Reconcile decision IDs and terminology across PRD, BRD, FRD, SRS, gap analysis, and solution mapping.
3. Confirm survey-data provenance and brand/asset permissions before making the repository public.
4. Review the README and document status labels, then choose the repository visibility.

## License and attribution

No license is included. Add a license only after confirming you have the right to publish every included document, image, logo, prototype, and source asset.
