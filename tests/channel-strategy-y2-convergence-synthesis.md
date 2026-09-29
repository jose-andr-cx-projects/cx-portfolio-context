# Channel Strategy Y2 — Convergence Synthesis

## Status

Active working synthesis for the Channel Strategy Y2 Convergence-to-Views test.

This is a project sensemaking layer, not an organisational system of record.

Original organisational sources remain authoritative. The GitHub Channel Strategy Y2 repository is an observation-layer mirror of exported Confluence material.

## Purpose

Converge the minimum useful Channel Strategy Y2 evidence once so it can support multiple views without repeatedly re-synthesising the same material.

Current baseline covers existing Intelligent Front Door Discover, Define and Design material. Off-Platform Search test results and Sustainability POC learning will be added as new evidence when available.

## Evidence discipline

Use:

**Source → Evidence / observation → Learning → IFD implication → Design requirement → Design question → Q1 value signal → Confidence / gap**

Do not treat working Design requirements as approved business or technical requirements.

## Baseline synthesis

| Source | Evidence / observation | Learning | IFD implication | Design requirement | Design question | Q1 value signal | Confidence / gap |
| --- | --- | --- | --- | --- | --- | --- | --- |
| IFD Discover — interaction-mode model | Discovery separates interaction mode from channel and finds that support mode needs to be assigned at task level. The same broad customer reason can require Routine, Guided or Assisted support. Accessibility, language, failed self-service, urgency and exceptional circumstances can change the required support level. | Channel alone is a poor proxy for customer support need. The front door needs to respond to the task and circumstances. | IFD should recognise enough about intent, task and context to match the customer to an appropriate level of guidance or assistance. | Preserve Routine → Guided → Assisted as an interaction lens rather than designing channel-specific experiences. | What is the minimum information needed to recognise when an apparently routine task needs Guided or Assisted support? | Discovery moved the strategy from channel categories toward a reusable task-level interaction model. | Discovery conclusion is sufficiently mature to inform Define and Design. Specific task classifications still require journey-level validation. |
| IFD Discover → Define | Discovery identifies recurring broad issues including unclear information, routing problems, fragmented context, avoidable contact and channel switching. Define explicitly warns that these remain broad until validated against individual journeys. | Broad CX pain points are useful for locating opportunity, but not sufficient as journey-level requirements. | IFD Design should use a bounded journey to test which broad patterns are actually material in context. | Keep evidence status visible and validate material journey-specific circumstances, constraints and exceptions before converting them into requirements. | Which broad Discovery patterns materially affect the selected journey, and which do not? | Q1 established an evidence discipline that prevents the IFD concept from becoming a generic solution looking for a problem. | Broad problem patterns supported; journey-level significance varies. |
| IFD Define | Define focuses the work on the first clearly defined IFD opportunity rather than redesigning the whole journey or prescribing a solution. Desired outcomes include easier pathway identification, clearer next-step information, support matched to need and better context at handoff. | The useful unit of Design is a specific connected-interaction problem with a decision to support, not an enterprise front-door solution. | IFD should be developed through bounded service cases while looking for patterns that may transfer. | Use the smallest useful Design test that can improve pathway clarity, information, routing, support or continuity. | What is the smallest future-state interaction we can test that materially improves the selected customer problem? | Define translated broad Channel Strategy direction into a bounded Design opportunity and measurable customer/service outcomes. | Define source is in progress. Earlier generic opportunity tables remain open; the Design page now contains the progressed parking-infringement direction. |
| IFD Design — parking/infringement problem | People dealing with a parking infringement can experience a fragmented journey across information, payment, review and support. The journey may begin off-platform and customers may need to understand the rule, options, evidence and next step before choosing a pathway. | The front-door problem begins before a form or owned channel and continues across multiple interactions. | IFD needs to connect discovery, understanding, pathway choice and appropriate support rather than optimise one touchpoint. | Begin wherever the customer begins; recognise intent and relevant context; guide toward authoritative information, the right pathway and support. | Can a connected front-door response reduce unnecessary searching, uncertainty, channel switching and repeated contact without forcing different circumstances into one pathway? | Q1 made Connected Interactions tangible through a real compliance journey rather than an abstract channel model. | Broad problem is marked partially validated and suitable for Design with explicit gaps. Specific circumstances and service rules vary in maturity. |
| IFD Design — context overlay | The Design brief defines context as customer circumstance + operational context + service constraints. Current scenarios include routine resolution, misunderstanding the rule, possible system/equipment failure, exceptional circumstances and returning after an earlier contest. These are explicitly design contexts, not confirmed segments. | Intent alone is not enough. Material context can change information, evidence, pathway, support or controls. | IFD needs a context-sensitive response without assuming personalisation or a single standard flow. | Identify only context that materially changes the appropriate response and adapt information, routing, support or controls accordingly. | Which context signals genuinely change the appropriate response, and which add complexity without improving the interaction? | Q1 progressed the concept from simple intent routing toward a more credible model of connected interaction based on material customer circumstances. | Scenarios have mixed status: working scenario, reported/hypothesis, working hypothesis and open. Must be tested rather than treated as requirements. |
| IFD Design — information & knowledge | Customers need to understand what happened, what applies, legitimate options, what they need to provide and what happens next. The need for clearer information is established; exact contextual variation remains open. | Knowledge is part of the interaction logic, not supporting content added after routing. | IFD requires authoritative, customer-readable information that can change where context materially affects options or next steps. | Explain the situation before action; present legitimate options around customer intent; make prerequisites visible before entry; explain what happens after action. | What information is universal, and what must change based on circumstance, action, authority or previous interaction? | Q1 connected service information architecture directly to the IFD experience rather than treating content as a separate workstream. | Overall need partially validated; several detailed requirements are strong working directions but exact service rules remain open. |
| IFD Design — connected experience | Design explicitly states that connected does not mean one pathway for everyone. It means enough continuity and understanding to provide the right next interaction for the customer's circumstances within legitimate constraints. | Connection is continuity of understanding and response, not consolidation into a single channel or interface. | IFD can work across existing pathways if it improves recognition, continuity and transition between them. | Preserve existing pathways where appropriate and prototype connective logic before assuming platform replacement. | What context must persist across handoffs so the next interaction feels like continuation rather than restart? | Q1 clarifies what “Connected Interactions” means operationally and avoids equating it with a chatbot, portal or single channel. | Strong Design principle; exact continuity/data needs remain to be established. |
| IFD Design — off-platform entry | The journey may begin through Google, AI-enabled search, an infringement notice or another source. The Design brief says City of Melbourne cannot control every external answer and should improve the authoritative source material external systems rely on. | The front door is an experience boundary, not only a City-owned interface. | Discoverability and machine/human interpretability of authoritative information become part of IFD Design. | Optimise authoritative source information; support customer-language entry; make next actions explicit; distinguish information from formal action; design for human and machine readability. | What must be true of authoritative information so an off-platform customer can understand the issue, receive safe guidance and reach the correct owned pathway? | Q1 extends Connected Interactions beyond owned channels and creates a concrete Off-Platform Search testable hypothesis. | Active testing required. Exact performance of search and AI surfaces must not be assumed. |
| IFD Design — Design posture | The current Design source says the next step is not technology selection. Stakeholders should validate the brief, identify the uncertainties that matter and choose the smallest useful Design activities. | The Design phase should operate as a decision engine: method follows uncertainty. | Sprint preparation should be driven by unresolved questions from the synthesis rather than a predetermined workshop sequence. | Decision first; smallest useful test; match method to uncertainty; preserve evidence status; keep human support and technology options open. | Which unresolved questions are important enough that answering them would change the next Design or investment decision? | Q1 has progressed far enough to enter focused Design without claiming implementation or scale readiness. | Design brief is in progress. Stakeholder validation and approach selection remain active work. |

## Emerging convergence spine

The current evidence supports this working sequence:

**Customer task and circumstance → interaction mode → authoritative information / knowledge → intent and routing → context and continuity → support / escalation → identity or authority where necessary → appropriate pathway**

This is a synthesis of the current evidence, not a confirmed enterprise architecture.

## Current Design questions

The baseline points to a small set of unresolved questions for Design:

1. What is the minimum information needed to recognise customer intent and material context?
2. Which contextual differences genuinely require a different response?
3. What information is universal and what must adapt?
4. What context needs to persist across pathways or handoffs?
5. When should the interaction move from Routine to Guided or Assisted support?
6. What can safely be understood off-platform, and where must the customer transition to an owned pathway?
7. Which of these interaction patterns appear useful beyond parking/infringements?

These questions should be refined as new evidence arrives rather than expanded into an exhaustive requirements catalogue.

## Next evidence inputs

Add, rather than separately re-synthesise:

- Off-Platform Search test results;
- Sustainability POC learning; and
- material stakeholder validation that changes the Design brief.

Each new input should update the synthesis only where it changes current understanding.
