# CX Project Mirror Maintenance

## Purpose

Define the smallest reliable operating pattern for keeping private GitHub CX project mirrors aligned with their organisational Git source so Strategic OS can use current project evidence without turning GitHub into a competing project workspace.

## Operating rule

> Organisational Git is the source. GitHub is the private observation mirror. Strategic OS reads the mirror and interprets the work.

The flow is one way:

```text
Organisational project repository
        ↓
controlled one-way sync
        ↓
GitHub CX project mirror
        ↓
Strategic OS review and interpretation
```

Do not use the GitHub mirror to make project changes that should originate in the organisational environment.

## When to sync

Sync a project mirror when one of these conditions is true:

- a material project update has landed in the organisational repository;
- Strategic OS needs the current project state for a decision, review or evidence assessment;
- a major project milestone or playback has completed; or
- the GitHub mirror is known or suspected to be stale.

Do not create a scheduled sync merely for completeness. Add automation only if repeated real use shows that manual syncing is creating material friction or stale evidence.

## Before syncing

Confirm all of the following:

1. the organisational source repository is known and authoritative for the material being mirrored;
2. the target is the matching private repository under `jose-andr-cx-projects`;
3. the GitHub repository has not been used as a competing project workspace;
4. no secrets, credentials, customer personal information or restricted organisational material are being introduced; and
5. the intended source and target repository names have been checked rather than inferred from naming alone.

If the source-of-truth relationship is unclear, stop and resolve it before syncing.

## Standard sync pattern

Use a fresh temporary mirror clone so the GitHub repository receives the Git history and refs from the organisational source without relying on a long-lived local working copy.

```bash
git clone --mirror https://bitbucket.org/<workspace>/<repository>.git <repository>.git
cd <repository>.git
git remote add github https://github.com/jose-andr-cx-projects/<repository>.git
git push --mirror github
cd ..
rm -rf <repository>.git
```

Use the approved authentication method for each platform. Do not place access tokens, passwords or credentials in committed files, scripts or repository documentation.

`git push --mirror` is intentionally authoritative: Git refs that exist only in GitHub may be removed because the organisational repository is the source. This is another reason not to create independent GitHub-only project branches or project content.

## Validation after sync

After each sync, confirm:

- the GitHub repository is still private;
- the default branch is correct;
- the latest expected organisational commit is visible in GitHub;
- no unexpected GitHub-only project changes remain; and
- Strategic OS can read the repository through the GitHub connector when the project is needed for analysis.

A successful sync means the GitHub mirror faithfully exposes the organisational Git state. It does not change the project's documented source-of-truth rules.

## Divergence rule

If GitHub and the organisational repository differ unexpectedly:

1. treat the organisational repository as authoritative for Git content;
2. do not manually reconcile project content in GitHub;
3. identify whether the divergence came from an incomplete sync or an inappropriate GitHub-side change;
4. resolve the project state in the organisational environment if required; and
5. re-run the one-way sync.

Flag material divergence before Strategic OS uses the mirror as evidence.

## What the mirror does not copy

The Git mirror covers repository content and Git history. It does not make GitHub authoritative for, or necessarily reproduce:

- Confluence content;
- Jira activity;
- Bitbucket pull-request discussion or platform settings;
- repository secrets or credentials;
- organisational permissions;
- governed source data; or
- other systems-of-record content referenced by the project.

Strategic OS should therefore preserve source awareness when interpreting mirrored material.

## Maintenance posture

Keep this process deliberately lightweight.

- Prefer on-demand sync over scheduled automation.
- Prefer a clean one-way mirror over two-way synchronisation.
- Do not add project-specific sync machinery until repeated use demonstrates a real need.
- Do not add career interpretation or Strategic OS conclusions to the mirrored project repositories.
- Keep portfolio-level rules in `cx-portfolio-context` and project-specific source rules in the project itself.

The success criterion is not continuous technical synchronisation. It is that Strategic OS can reliably access sufficiently current, source-aligned project evidence when a strategic decision or review requires it.
