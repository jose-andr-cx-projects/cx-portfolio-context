# Project Implementation Agents — Implementation Checklist

## Status

**Rovo selected — staged implementation planning active (25 October 2026)**

This checklist records the work that would be required to move the agreed Project Implementation Agent Model into practical use.

José has explicitly selected CoM Rovo Studio for the two existing project agents after limited read-only capability tests. The phased plan below supersedes the earlier blanket pause, while retaining all quality, authority and approval gates.

Related model:

`project-implementation-agent-model.md`

---

## Implementation objective

Create a lightweight, testable implementation of:

1. Human-Centred Design Specialist
2. Agile Project Lead

that can operate across José's CX project portfolio while respecting organisational source-of-truth boundaries and using Strategic OS as strategic context rather than as the project delivery system.

---

# Gate 0 — Confirm the broader agentic model

Before implementation:

- [ ] Define the broader agentic operating model.
- [ ] Confirm where project implementation agents sit within that model.
- [ ] Confirm their relationship to Strategic OS specialists.
- [ ] Confirm whether project agents use the same human-facing control surface as Strategic OS agents.
- [ ] Confirm whether portfolio coordination belongs to the Agile Project Lead, Chief of Staff, another layer, or a deliberate combination.
- [ ] Confirm whether direct specialist selection remains the preferred interaction model.
- [ ] Confirm what should remain manual during the first pilot.
- [ ] Confirm that no existing agent can satisfy the need with a small extension instead.

**Gate condition:** proceed only if the two project implementation roles remain distinct and useful after the broader model is defined.

---



## Gate 0 interaction and platform exploration, agreed 24 October 2026

- [ ] Confirm the work-laptop, cloud-browser access requirements and organisational permission to use each candidate service.
- [ ] Define the minimum interaction contract: project selection, intentional specialist selection, visible responding role, verified context/source freshness, conversation continuity, and human approval before external changes.
- [ ] Confirm portfolio priorities and cross-project trade-offs remain with Chief of Staff, while project-level delivery flow remains with Agile Project Lead; validate overlap in the live Strategic OS agent specification.
- [ ] Assess GitHub Copilot Spaces for contextual project conversation using selected approved source files; verify separately whether GitHub custom agents can deliver the intended specialist experience in that surface.
- [ ] Compare with ChatGPT plus GitHub as the familiar interaction baseline, using the same bounded scenario and project context.
- [ ] Consider Relevance Chat only as a tested multi-agent interaction alternative, not an assumed requirement.
- [ ] Treat Fly.io as a later custom-app hosting option; do not build a new frontend or orchestration layer for this pilot.
- [ ] Assess whether GitHub Projects, Issues or Actions remove friction without duplicating organisational Jira/Confluence or producing ungoverned project status.
- [ ] Record observed quality of source grounding, specialist output, usability, continuity, permission constraints and manual overhead before choosing a runtime or interface.

**Proposed first test, not yet started:** Customer Account Management read-only conversation through GitHub Copilot Spaces with an Agile Project Lead lens. Ask for purpose/scope with source links; documented decisions, risks and dependencies with explicit unknowns; and the next smallest valuable increment with evidence. Then repeat comparable questions in ChatGPT plus GitHub. Consider Channel Strategy Y2 for a separate HCD case. Use approved, non-sensitive context only.

**Decision and pause:** The two-agent model remains agreed; initial interaction direction is cloud-accessible, conversation-first and project-context-aware. Platform choice, custom agents, pilot execution and automation remain deferred until José explicitly reopens implementation. This section documents future validation, not completed Gate 0 checks.

---

# Gate 1 — Confirm authoritative project inputs

For each pilot project:

- [ ] Document the project's authoritative organisational sources.
- [ ] Confirm the role of Confluence.
- [ ] Confirm the role of Jira.
- [ ] Confirm the role of Bitbucket or other project repositories.
- [ ] Confirm which GitHub repository is a mirror or observation layer.
- [ ] Identify any material project sources not visible to the agent.
- [ ] Define how stale or conflicting source information is handled.
- [ ] Define what project information must never be copied into an agent memory or repository.
- [ ] Confirm project-specific privacy, security and governance constraints.

**Gate condition:** the agent can distinguish authoritative project state from contextual or mirrored state.

---

# Gate 2 — Define minimum agent contracts

## Human-Centred Design Specialist

- [ ] Define mission.
- [ ] Define primary question.
- [ ] Define required inputs.
- [ ] Define optional inputs.
- [ ] Define supported HCD activities.
- [ ] Define expected outputs.
- [ ] Define evidence and confidence rules.
- [ ] Define phase-readiness logic where project phases are used.
- [ ] Define escalation triggers.
- [ ] Define prohibited actions.
- [ ] Define human-review points.
- [ ] Define success measures.

## Agile Project Lead

- [ ] Define mission.
- [ ] Define primary question.
- [ ] Define required inputs.
- [ ] Define optional inputs.
- [ ] Define supported delivery activities.
- [ ] Define expected outputs.
- [ ] Define risk, dependency and blocker logic.
- [ ] Define work-in-progress and sequencing principles.
- [ ] Define escalation triggers.
- [ ] Define prohibited actions.
- [ ] Define human-review points.
- [ ] Define success measures.

**Gate condition:** each role has a narrow implementation contract and does not duplicate an existing Strategic OS agent.

---

# Gate 3 — Choose bounded pilots

## Human-Centred Design Specialist pilot

Candidate:

`channel-strategy-y2`

Validate before use:

- [ ] project is still a suitable active HCD case;
- [ ] sufficient Discover / Define / Design evidence is accessible;
- [ ] there is a real upcoming design decision or activity;
- [ ] the pilot can produce observable value without changing project authority; and
- [ ] success can be assessed from a small number of real interactions.

## Agile Project Lead pilot

Candidate:

`customer-account-management`

Validate before use:

- [ ] project remains sufficiently active;
- [ ] delivery state can be observed from available sources;
- [ ] risks, assumptions, decisions and current work can be distinguished;
- [ ] there is a real flow or prioritisation problem to support; and
- [ ] the pilot can operate without creating a competing project-management system.

**Gate condition:** each agent has one real, bounded pilot with an identifiable implementation problem.

---

# Gate 4 — Define minimum context package

Avoid giving either agent the entire portfolio by default.

Define the minimum project context required for a useful run.

Possible components:

- [ ] project purpose;
- [ ] current outcome;
- [ ] current stage;
- [ ] active increment;
- [ ] project source rules;
- [ ] relevant decisions;
- [ ] current evidence;
- [ ] current assumptions;
- [ ] active risks;
- [ ] current dependencies;
- [ ] recent material changes; and
- [ ] links or references to authoritative sources.

For portfolio-level Agile Project Lead reviews:

- [ ] define the minimum summary required from each active project;
- [ ] avoid ingesting full project repositories unless the review requires it;
- [ ] distinguish portfolio signals from project-specific evidence.

**Gate condition:** context is sufficient for the task without creating unnecessary ingestion, duplication or maintenance.

---

# Gate 5 — Define Strategic OS context and escalation

- [ ] Identify which Strategic OS principles should always be available.
- [ ] Identify which Strategic OS context should be loaded only when relevant.
- [ ] Define when HCD Specialist escalates to Sensemaking.
- [ ] Define when HCD Specialist escalates to Stakeholder Journey.
- [ ] Define when HCD Specialist escalates to Shipping Coach.
- [ ] Define when Agile Project Lead escalates to Sensemaking.
- [ ] Define when Agile Project Lead escalates to Stakeholder Journey.
- [ ] Define when Agile Project Lead escalates to Shipping Coach.
- [ ] Define when either agent surfaces an issue to Chief of Staff.
- [ ] Define when reusable learning should be considered for Strategic OS.
- [ ] Prevent automatic multi-agent sequencing during the pilot unless explicitly required.

**Gate condition:** project implementation and strategic reasoning remain distinct but connected.

---

# Gate 6 — Define minimum runtime behaviour

For the first pilot, prefer a deliberately simple runtime.

- [ ] José intentionally selects the agent.
- [ ] José identifies the project or requests a portfolio review.
- [ ] Agent loads only required context.
- [ ] Agent identifies source authority and uncertainty.
- [ ] Agent performs one bounded implementation task.
- [ ] Agent returns a concise decision- or action-oriented output.
- [ ] José reviews the output.
- [ ] No external action occurs without explicit approval.
- [ ] No automatic write-back occurs during the initial pilot.
- [ ] No automatic multi-agent chain occurs during the initial pilot.

**Gate condition:** the workflow is useful before any additional orchestration is added.

---

# Gate 7 — Define agent-specific quality tests

## Human-Centred Design Specialist

Test whether the agent:

- [ ] distinguishes customer evidence from internal opinion;
- [ ] distinguishes evidence from assumptions;
- [ ] identifies material evidence gaps;
- [ ] avoids inventing customer needs;
- [ ] avoids premature solutioning;
- [ ] improves problem framing;
- [ ] recommends proportionate research rather than research for its own sake;
- [ ] identifies when enough evidence exists for the next decision;
- [ ] helps design a useful next experiment or validation activity; and
- [ ] produces a practical next move.

## Agile Project Lead

Test whether the agent:

- [ ] understands the intended project outcome;
- [ ] identifies the active increment;
- [ ] distinguishes tasks, blockers, dependencies, risks and decisions;
- [ ] identifies oversized or stalled work;
- [ ] challenges unnecessary parallel work;
- [ ] does not invent owners or deadlines;
- [ ] avoids generating unnecessary project controls;
- [ ] identifies when activity is disconnected from value;
- [ ] produces a useful next sequencing recommendation; and
- [ ] reduces rather than increases project-management overhead.

---

# Gate 8 — Run manual pilot tests

Before automation:

- [ ] Run HCD Specialist against one real Channel Strategy Y2 task.
- [ ] Run HCD Specialist against a second materially different HCD task.
- [ ] Run Agile Project Lead against one real Customer Account Management delivery problem.
- [ ] Run Agile Project Lead against a second materially different delivery problem.
- [ ] Record where agent context was insufficient.
- [ ] Record where agent advice duplicated an existing specialist.
- [ ] Record where agent outputs created unnecessary work.
- [ ] Record where human correction was required.
- [ ] Record whether the output changed a real project decision or next action.

**Gate condition:** repeated manual use demonstrates a genuine implementation advantage.

---

# Gate 9 — Assess value before automation

For each agent, assess:

- [ ] Did it improve decision clarity?
- [ ] Did it improve project movement?
- [ ] Did it surface important uncertainty earlier?
- [ ] Did it reduce manual synthesis?
- [ ] Did it reduce avoidable administration?
- [ ] Did it preserve source authority?
- [ ] Did it stay within its role?
- [ ] Did it complement rather than duplicate Strategic OS agents?
- [ ] Did it create enough value to justify a maintained runtime?

Possible outcomes:

- [ ] Continue as designed.
- [ ] Refine the role.
- [ ] Merge capability into an existing agent.
- [ ] Keep as an on-demand prompt/workflow rather than a persistent agent.
- [ ] Stop.

---

# Gate 10 — Only then consider integration and automation

Do not assume these capabilities require a complex runtime.

Only after successful pilots consider:

- [ ] direct project-system connectors;
- [ ] Jira read access;
- [ ] Confluence read access;
- [ ] portfolio context retrieval;
- [ ] GitHub mirror retrieval;
- [ ] Slack initiation;
- [ ] structured output persistence;
- [ ] approved Jira or Confluence write-back;
- [ ] scheduled portfolio reviews;
- [ ] event-driven triggers;
- [ ] agent-to-agent handoffs; and
- [ ] additional orchestration.

For every integration, ask:

> Does this remove repeated friction or improve decision quality enough to justify the additional complexity?

If not, keep the workflow manual.

---

# Implementation completion criteria

Implementation should not be considered successful because an agent runs technically.

A useful implementation should demonstrate that:

- [ ] the agent solves a repeated real project problem;
- [ ] its role is distinct from existing Strategic OS agents;
- [ ] its source model is reliable;
- [ ] it improves a real project decision, learning step or delivery increment;
- [ ] it preserves human approval;
- [ ] it does not create a competing system of record;
- [ ] it does not increase documentation burden;
- [ ] its output can be trusted within explicit caveats;
- [ ] its runtime is simple enough to maintain; and
- [ ] repeated use justifies retaining it.

---

# Current position

Rovo is the agreed CoM platform. Initial Agile Project Lead configuration and advisory testing were performed by José; HCD implementation and source-write workflows are not yet evidenced. Follow the staged Rovo plan below. Nothing here authorises unattended writes, agent self-publishing or merging, or transferring CoM material into personal systems.

---

# Approved staged Rovo implementation plan (25 October 2026)

**Decision:** No more basic connectivity tests. Proceed toward using both agreed specialist agents in CoM Rovo. This is authorisation to develop the two capabilities and plan controlled integrations, **not approval for unattended publication or cross-system write access**.

## Phase 1: Establish operational baselines

- [x] Rovo chosen as the CoM project-agent interaction environment.
- [x] Manual agent editor, knowledge selectors and tool catalogue inspected.
- [x] Agile Project Lead initially assessed against CAM Jira/Confluence project evidence.
- [x] Direct Bitbucket read of a known substantive README reported successful (Test 05; accuracy independently unverified).
- [ ] Inventory current Agile Project Lead configuration (name, instruction version, knowledge, tools, agent visibility, account identity, human review).
- [ ] Create/configure the **HCD Specialist** in Rovo using the already-agreed role boundaries.
- [ ] Identify one approved project/meeting example for each agent; keep transcripts in CoM-approved locations.
- [ ] Define per-project source contract: authoritative Bitbucket files, published Confluence pages, Jira delivery objects, access/approval owner and sync method.

**Exit:** Both agents can operate in advisory mode with an explicit, source-aware project scope and no write tools.

## Phase 2: Transcript-driven next-step extraction (highest priority)

- [ ] Confirm CoM-approved Teams transcript access/retention and whether a built-in Rovo connector can access transcript content. Do not assume catalogue listing means enabled access.
- [ ] First use a user-provided approved transcript or its approved internal link in the CoM environment; no external copying.
- [ ] HCD Specialist extracts validation outcomes, customer vs stakeholder evidence, open questions, assumptions, design decisions pending ratification, and the smallest next learning/validation activity.
- [ ] Agile Project Lead turns the reviewed findings into a small valuable delivery increment, dependencies, blocked decisions, proposed Jira task changes and acceptance criteria.
- [ ] Standardise a lightweight handoff object: project, meeting URL/date, source excerpt, signal type, confidence, owner/approver, current evidence, proposed next step, target file/issue, approval status.
- [ ] Require explicit human confirmation for decisions, commitments, ownership and external communications. Meeting discussion alone does not authorise updates.
- [ ] Preserve traceability between the transcript, source evidence, approval and proposed changes.

**Exit:** A real approved Teams meeting example yields accurate, useful next-step proposals with no invented decisions or owners and less manual synthesis.

## Phase 3: Bitbucket-first controlled updates

- [ ] Select one project where its documented source contract identifies a Bitbucket Markdown object as authoritative.
- [ ] Resolve the exact current file path and branch in the browser; do not depend on historical commits or autonomous tree listing.
- [ ] Agent drafts a **specific file change** with before/after, source references, rationale and reversible diff. No automatic commit.
- [ ] Confirm supported Rovo tool actions and effective agent identity; if file editing is not available, use a human-applied patch or a separately approved repository workflow.
- [ ] Adopt reviewer approval and preferably PR-based changes for consequential source updates. Avoid write/merge tools by default.
- [ ] Verify committed content and record commit/PR reference only after observed success.

**Exit:** One approved transcript-derived change reaches the correct Bitbucket source, with an auditable approval trail, no unsupported claims of automatic write capability.

## Phase 4: Publish and reconcile Confluence and Jira

- [ ] Inspect the project's existing Bitbucket-to-Confluence publishing configuration, trigger, mapping, failure behaviour and permissions.
- [ ] Publish only approved source changes using the project's documented publishing process; avoid manually maintaining competing authoritative versions.
- [ ] Confirm published Confluence page content/version corresponds to intended Bitbucket revision; log mismatches without silently overwriting either source.
- [ ] Draft Jira issue creation/update or linkage based on the approved delivery increment. Require human approval, accurate owner/status and explicit dependency.
- [ ] Apply through authorised Jira tooling only after the tool permissions, audit and rollback path are verified.
- [ ] Verify each resulting Jira/Confluence record directly and store links with the underlying Bitbucket change and meeting decision.
- [ ] If any downstream update fails, mark the item **partially synchronised** and surface a human reconciliation action.

**Exit:** One source-approved project change is traceable through Bitbucket, Confluence and Jira, with explicit differences recorded rather than concealed.

## Phase 5: Regular project operating experience

- [ ] Start with intentional selection of project and HCD/Agile specialist in Rovo; no hidden agent chains.
- [ ] After approved project meetings, present a compact review: validated findings, decisions for confirmation, next learning step, next delivery increment, blockers and pending source updates.
- [ ] Support a concise weekly project review and optional portfolio view only after current-source retrieval is dependable.
- [ ] Measure next-step usefulness, accurate decision classification, source-parity accuracy, human corrections, time saved, successful controlled updates and maintenance burden.
- [ ] Consider automated transcript ingestion, agent-to-agent handoff, recurrent summaries or write-back **only** after demonstrated repeated value and separate permissions/security approval.

**Exit:** José receives decision-ready next steps and can approve reliable, low-admin updates without a second project-management system.

## Hard constraints and outstanding technical unknowns

- CoM-only agent execution and original organisational content; no personal ChatGPT connector or copy of raw Teams transcripts into personal GitHub/Strategic OS.
- A Bitbucket knowledge checkbox is not evidence of complete repo indexing; current tree listing, full commit log and PR retrieval were not demonstrated.
- Test 04's outdated file path invalidated its permission diagnosis. Test 05 gave a **provisional** substantive known-file read, not an independently audited accuracy claim.
- Rovo tools may expose create/merge PR actions; do not give these to HCD or Agile agents without specific approved scope and enforceable review gates.
- Determine whether Teams transcript access is supported and authorised, whether Rovo can propose Bitbucket file changes, and how existing publishing and Jira reconciliation actually operate.
- Where organisational access or governance policy disallows automated writes, retain human copy/commit/update as the supported implementation.
- Do not label a phase or integration complete until it has observed evidence. Preserve source-specific authority even when Confluence/Jira and Bitbucket are out of sync.

## Decision log

- **25 October 2026:** José chooses Rovo for CoM CX project agents; basic retrieval testing ends.
- **Primary product value:** Teams validation and meeting evidence -> next HCD/Agile steps -> approved Bitbucket source changes -> verified Confluence/Jira consistency.
- **Roles:** retain HCD Specialist and Agile Project Lead.
- **Governance:** staged delivery, human approval, project-level source contracts, no automatic integration with personal OS.
