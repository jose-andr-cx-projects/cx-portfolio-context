# Strategic OS intake from CX project work

**State:** Governed handoff contract proposal, not an active integration. Replaces the assumption that full or periodic GitHub mirrors are required for Strategic OS access.

## Purpose

Preserve the strategic value of experience gained through CoM projects while leaving organisational project records in approved CoM systems. Strategic OS should learn from selected insights, not hold a private copy of the portfolio.

## Boundary

- **CoM side:** Bitbucket, Confluence, Jira, Miro, Teams and Rovo handle live delivery. Organisational content remains inside the approved environment.
- **Personal side:** Strategic OS receives **only information explicitly reviewed and permitted for external use**, such as abstracted methods, generalised decision patterns, non-sensitive achievements and strategic learning.
- **No direct sync** of CoM repository contents, raw meeting transcripts, stakeholder names, confidential metrics, internal links, personal information, technical credentials or unreleased project materials.
- A user requesting an intake draft is not equivalent to an information-owner approving its disclosure. If classification/permission is unclear, keep the candidate in CoM until cleared.

## Proposed minimum intake object

```yaml
intake_id: <local reference, no internal CoM identifier required>
created_on: YYYY-MM-DD
type: strategic_signal | reusable_method | decision_pattern | career_evidence_candidate | reflection
title: <generic non-sensitive title>
why_it_matters: <abstracted learning>
transferable_principle: <what applies beyond one project>
evidence_status: observed | proposed | validated
reviewed_for_external_use: false
reviewed_by: <role or authorised reviewer, if approved>
allowed_destination: none | strategic_os
next_review: <optional>
```

## Two-stage process

1. In CoM, Companion may suggest **intake candidates**, but does not export them automatically. Candidate remains internal; carry only an abstract title until review.
2. José and applicable content owner review information classification, specificity, privacy and intellectual-property obligations. Only a cleared, sanitised note is deliberately introduced into the Personal/Strategic OS intake lifecycle through an approved mechanism.

Strategic OS should apply its existing **incubation -> review -> promotion** process and distinguish learning candidates from authoritative principles. No new personal architecture layer is required. A citation back to a private CoM source should not be stored in an externally accessible note unless expressly authorised.

## Useful intake lenses

- Repeated cross-project constraints that suggest a reusable capability.
- Generalisable HCD / governance / programme management methods proven by use.
- Strategic decisions and trade-offs expressed without private operational specifics.
- Personal reflection or career evidence written and approved at a safe abstraction level.

## Exclusions and failure handling

If external use is not explicitly approved, keep the material solely in CoM. Do not copy a GitHub mirror first and review later. No assumed rights to transfer organisational data just because a user can view it. When in doubt, capture a reminder **within CoM** to revisit intake approval rather than exporting content.
