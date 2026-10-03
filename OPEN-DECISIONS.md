# Open decisions — Aster Health Plan Search

Resolve and record an approver, decision date, evidence, and affected artifact updates for each item. The identifiers below follow the current UAT readiness tracker. Earlier documents use different numbering; reconcile those references into one canonical decision log before baselining.

| ID | Decision needed | Proposed owners | Main impact |
|---|---|---|---|
| D-01 | Confirm whether the third mandatory geography is **County** or **Country**; approve the location hierarchy and catalogue. | Product Owner, Plan Data Owner | Search criteria, selectors, source mapping, validation, UAT-04/05 |
| D-02 | Approve plan-type values and behavior, the essential-benefit catalogue, and whether benefit matching uses all, any, or another rule. | Product Owner, Plan Data Owner | Filters, results, requirement wording, UAT-06/08 |
| D-03 | Confirm the authoritative plan-data/GDS system, legal partner name, interface owner, and test contract. | Sponsor, Integration Lead | Integration boundary, data ownership, request/response mapping, UAT-09 |
| D-04 | Approve result/detail fields, cost-sharing definitions and units, data freshness, and missing-value handling. | Plan Data Owner, Product Owner | Results, detail screens, member interpretation, UAT-10/11 |
| D-05 | Approve plan-to-phone and plan-to-enrollment destination mappings, device behavior, link validation, and fallbacks. | Member Services, Enrollment Owner | Per-row action integrity, external handoffs, UAT-16/21 |
| D-06 | Approve no-match/error/retry rules, supported platforms, accessibility criteria, and privacy/logging expectations. | Product, Integration, QA, Security/Privacy | Resilience and quality baseline, UAT-12/15 and UAT-23/25 |
| D-07 | Decide whether Helpdesk is in this module; define operational ownership, analytics events, and success measures. | Product, Member Services, Sponsor | Scope, support route, measurement, UAT-22/26 |

## Baseline rule

Do not treat proposed behavior as approved. Update dependent requirements, stories, wireframes, BPMN, solution-map rows, and UAT expected results after each decision. Keep each issue's approval evidence and link the decision to the affected requirement and test IDs.
