# CX Portfolio: Bitbucket-native architecture (migration candidate)

**Status:** Proposed organisational architecture package prepared in GitHub on 26 October 2026. **Not deployed to Bitbucket.** CoM owners must review access, source authority and publication rules before copying into the approved Bitbucket environment.

## Intent

Use existing CoM Atlassian systems for the day-to-day CX project portfolio; remove ongoing GitHub mirroring. Retain a small, deliberate **Strategic OS intake** that preserves reusable learning without exposing unapproved organisational records.

## Logical design

```
CoM work environment (approved access)
  Miro: visual collaboration       Teams: meeting evidence
             \                       /
              -> CX Project Companion (Rovo)
                   |- think: interpret / challenge / prioritise
                   |- propose: smallest next increment + Miro visual when useful
                   |- maintain: reviewed document changes
                   v
  Bitbucket workspace
    |- Bitbucket Projects: existing organisational groupings
    |- CX Portfolio project (proposed): cx-portfolio repository
    |- other project groups: project-specific repositories
    
  Confluence: published context and decisions as designated
  Jira: delivery commitments, statuses and ownership
                   |
        human-reviewed, permitted abstraction only
                   v
  Strategic OS intake (independent personal environment)
    decision / lesson / reusable method / strategic signal
    NO raw transcript, customer data, internal URL, unapproved content
```

## Bitbucket hierarchy

- **Workspace**: CoM Bitbucket workspace, exact workspace identity to be confirmed in CoM.
- **Bitbucket Project**: native organisational grouping for access / related repositories. Preserve existing projects and repo names; do not conflate Bitbucket Projects with repositories or folder trees.
- **Portfolio repo**: one private `cx-portfolio` repo within a suitable CoM Bitbucket Project. It indexes other project repositories and cross-project dependencies; it is **not** a replacement source of delivery status.
- **Project repositories**: each root `README.md` becomes a stable entry point, with links to existing files, Confluence context, Jira work and publishing contract. Avoid a new mandatory directory layout and do not copy source documents into portfolio repo.

## Source contracts

| Record | Default system | Rule |
|---|---|---|
| Project working Markdown / versioned logic | Bitbucket, where designated | Check specific repository's approved contract before editing |
| Published decisions, governance and context | Confluence, or a Bitbucket-backed published page | Identify approval authority and upstream publishing source |
| Tasks, dates, assignees, delivery states | Jira | Don't duplicate as authoritative checklists in Markdown |
| Visual working artefacts | Miro | Working hypotheses are not ratified decisions |
| Meeting discussion | Teams transcript / approved notes | Latest supplied evidence; confirm decisions and ownership |
| Portfolio snapshot / cross-project insights | cx-portfolio index | Linked, dated, evidence-qualified view only |

## Minimal project README contract

1. Project name, purpose and repository status (active / historical / prototype / handoff).
2. Link to current project document map (use existing paths).
3. Link to approved Confluence and Jira entries, if known; otherwise mark **to verify**.
4. One paragraph explaining source authority, how publication works and how to propose updates.
5. Latest review date / evidence status; **do not** assert live project status from README alone.
6. Optional: links to related projects and cross-project dependencies.

## Companion workflow

1. José supplies the latest Teams transcript, selected Miro export, data or instruction **within CoM**.
2. Companion reads relevant current repo files via exact entry-point links and existing authoritative pages. It does **not** need to discover all possible meetings.
3. Joint reasoning: what's new, which assumptions changed, what should happen next, and whether a Miro visual helps.
4. Prepare minimal source-specific edits and decisions requiring confirmation.
5. After approval, execute only with authorised permissions. Rovo's current tools do **not** support direct Bitbucket file edits/branches; provide targeted patch or full file to apply manually, then verify if possible.
6. Reconcile affected Confluence/Jira records according to the project publishing contract and verify; never claim automatic sync without proof.

## Migration to Bitbucket

1. Create/identify private CoM Bitbucket Project for cross-project coordination, respecting existing project groupings and permissions.
2. Create private `cx-portfolio` repo with the index and operating contract files in this package.
3. Add/refine README maps in existing CoM Bitbucket repositories *after inspecting their actual current contents*; GitHub documentation must never overwrite a newer Bitbucket source.
4. Define source contracts per repo, including Confluence publishing pipeline, access and Jira linkage; verify rather than assuming prior patterns work everywhere.
5. Turn off routine GitHub mirror updates only after confirming authoritative Bitbucket files and data-handling approvals. Archive/restrict obsolete copies as permitted, without deleting project evidence by default.
6. Preserve separate governed Strategic OS intake described in `strategic-os-intake.md`; never establish raw repository sync to a personal system.

## Validation gates

- [ ] Correct Bitbucket project/workspace names and access identified.
- [ ] Project repo paths and authoritative sources verified *in Bitbucket*.
- [ ] README points to valid current files (no historical path guess).
- [ ] Relevant Confluence publication and Jira links checked.
- [ ] No sensitive transcripts, personal data, secrets or restricted artefacts copied into personal GitHub.
- [ ] A transcript-driven update is reviewed, applied to correct source and read-back verified.
- [ ] Strategic OS intake boundary reviewed with applicable CoM information governance.

**Not a mandate:** No new agent, routine mirror, automatic sync engine or duplicate source of truth is created by this package.
