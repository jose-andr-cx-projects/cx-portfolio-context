# CX Portfolio Bridge Checklist

## Status

**Parked**

The portfolio bridge is sufficiently defined for current use. Do not expand it unless repeated real use exposes a gap.

## Completed

- [x] Create private GitHub organisation `jose-andr-cx-projects`.
- [x] Transfer the current CX project repositories into the organisation.
- [x] Set all current CX project mirrors to private.
- [x] Confirm ChatGPT/Codex GitHub connector access to the organisation.
- [x] Create private `cx-portfolio-context` repository.
- [x] Define the organisational project → private GitHub mirror → Strategic OS bridge.
- [x] Define one-way mirror rules and divergence handling.
- [x] Define on-demand mirror maintenance rather than continuous synchronisation.
- [x] Preserve project-specific source-of-truth rules and avoid adding Strategic OS interpretation to mirrored organisational repositories.

## Parked follow-up

Only revisit these items if real use shows they are needed:

- [ ] Validate the first real Bitbucket → GitHub resynchronisation after an organisational repo changes.
- [ ] Confirm whether any project needs a different mirror rule because its source-of-truth contract differs.
- [ ] Add lightweight automation only if manual mirror maintenance becomes repetitive or unreliable.
- [ ] Review the portfolio index when a new CX project needs Strategic OS access.

## Reopen criteria

Reopen this workstream only when one of the following occurs:

- a mirror becomes stale or diverges;
- a new project needs to join the portfolio;
- manual maintenance creates repeated friction;
- privacy or source-authority rules change; or
- Strategic OS cannot reliably interpret a project because the bridge metadata is insufficient.

## Next active workstream

Explore a governed Salesforce email-template maintenance and change process that connects CX-led business assessment, internal enterprise AI assistance, and the existing delivery ecosystem across Salesforce CRM, Atlassian and Microsoft 365.
