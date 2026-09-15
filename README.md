# CX Portfolio Context

## Purpose

This repository is the lightweight bridge between José's organisational CX project environment and Strategic OS.

It does not replace project documentation, delivery management or implementation repositories. Its role is to make the CX project portfolio easy for Strategic OS to discover, interpret and use through a personal strategic and career lens without changing the organisational source material.

## Operating model

```text
ORGANISATIONAL PROJECT ENVIRONMENT

Confluence
Agreed project context, decisions and endorsed artefacts
        │
        ▼
Jira
Delivery activity, ownership, sequencing and progress
        │
        ▼
Bitbucket
Project working assets → implementation → operationalisation
        │
        │ controlled private mirror
        ▼
────────────────────────────────────────
PERSONAL STRATEGIC ENVIRONMENT

GitHub CX Projects organisation
Private project mirrors
        │
        ▼
Strategic OS
Safe project summaries, strategic interpretation,
career evidence and reusable learning
```

## Core rule

> Bitbucket and the relevant organisational systems run the work. GitHub exposes a private mirror of that work to Strategic OS. Strategic OS interprets the work; it does not become the organisational project source of truth.

## Repository roles

| Layer | Role | Authority |
|---|---|---|
| Confluence | Agreed project context, decisions and endorsed stakeholder-facing artefacts where used by the project | Organisational project authority for that material |
| Jira | Delivery activity, ownership, sequencing, dependencies and progress | Delivery-management authority |
| Bitbucket | Organisation-managed project repository, implementation assets and transition toward operationalisation | Organisational Git authority |
| GitHub CX project mirror | Private mirrored project content made accessible to Strategic OS | Observation layer only |
| `cx-portfolio-context` | Portfolio index, mirror rules and Strategic OS bridge metadata | Bridge definition only |
| Strategic OS | Personal strategic interpretation, safe project summaries, reusable learning and career evidence | Authoritative for José's Strategic OS knowledge |

Individual projects may use these systems differently. The project's own documented source rules take precedence for project-specific material.

## Mirror rules

1. GitHub project repositories in `jose-andr-cx-projects` should remain faithful mirrors of their organisational project repositories where a Bitbucket source exists.
2. Organisational project changes should be made in the appropriate organisational system first and then mirrored to GitHub.
3. Do not add personal career analysis, Strategic OS interpretation or private stakeholder commentary to mirrored project repositories.
4. Do not mirror customer personal information, secrets, credentials, raw governed datasets or material that should remain only in an organisational system of record.
5. If Bitbucket and GitHub differ, treat Bitbucket as authoritative for the organisational repository and flag the divergence rather than silently reconciling it.
6. Strategic OS may use mirrored repositories as evidence inputs, but should retain only safe summaries, references, interpretations and reusable learning.
7. Do not automatically push Strategic OS conclusions or career analysis back into organisational systems.

## Strategic OS relationship

Strategic OS already provides `08_projects/` for project-specific Strategic OS artefacts, including safe summaries, links to organisational systems, decisions, outputs and lessons.

The intended relationship is:

```text
GitHub CX project mirror
        ↓
Strategic OS review
        ↓
08_projects/<project>/
Safe context, links, decisions, outputs and lessons
        ↓
Promote only when useful
        ├── 01_career/
        ├── 03_decision_briefs/
        ├── 04_frameworks/
        ├── 05_lessons_learned/
        ├── 06_stakeholder_patterns/
        └── 09_thought_leadership/
```

This keeps organisational project evidence separate from José's personal interpretation while still allowing Strategic OS to reason across the portfolio.

## Current portfolio

| GitHub mirror | Visibility | Role |
|---|---|---|
| `cx-current-state-sop-mapping` | Private | CX project mirror |
| `customer-account-management` | Private | CX project mirror |
| `channel-strategy-y2` | Private | CX project mirror |
| `reusable-cx-knowledge-architecture` | Private | CX project mirror |

## New project pattern

For a new CX project:

1. establish the organisational project and its source-of-truth rules;
2. use Bitbucket when the project requires an organisation-managed repository through implementation and operationalisation;
3. create a private GitHub mirror under `jose-andr-cx-projects` when Strategic OS access is useful;
4. add the mirror to this portfolio index;
5. create or update the corresponding Strategic OS project context only when there is useful strategic, decision, learning or career value to retain.

Do not create a GitHub mirror merely for completeness.

## Boundary

This repository should stay small.

It should contain portfolio-level bridge information only. Project content belongs in the individual project repository or the relevant organisational system. Strategic and career interpretation belongs in Strategic OS.
