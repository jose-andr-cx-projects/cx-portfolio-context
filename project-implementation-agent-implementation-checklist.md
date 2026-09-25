# Project Implementation Agents — Implementation Checklist

## Status

**Parked — do not implement yet**

This checklist records the work that would be required to move the agreed Project Implementation Agent Model into practical use.

It is not the current implementation sequence.

Do not start this checklist until the broader agentic model has been explored and José explicitly decides to begin implementation.

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

Implementation has **not started**.

No agent specifications, prompts, runtimes, automations, integrations or new Strategic OS framework components should be created from this checklist yet.

The next work is the broader framing of José's agentic model.

Reopen this checklist only after that framing is sufficiently clear and José explicitly chooses to begin implementation.
