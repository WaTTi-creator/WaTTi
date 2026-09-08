# GitHub Workflow — WaTTi Personal Universe

## Purpose

GitHub is the durable source-control layer for the Personal Universe. The repository is the place where stable source, architecture decisions, experiments, and recovery checkpoints can live independently of any visual builder.

## Current state

- Repository: `WaTTi-creator/WaTTi`
- Stable branch: `main`
- Working branch for this setup: `foundation/github-workflow`
- The existing Lovable application is **Dark Cinema Showcase**.
- Lovable source has not yet been imported into this repository.

## Safe development model

1. Keep `main` stable.
2. Create a feature branch for meaningful changes.
3. Make the smallest useful change first.
4. Review the diff before merging.
5. Merge only a verified change into `main`.
6. Keep Lovable as an optional builder rather than the only source of the project.

## Planned branches

- `main` — stable, recoverable project state
- `feature/universe-foundation` — Personal Universe architecture and core UI
- `feature/dark-media` — Dark Media world
- `feature/timeline` — timeline and chronology
- `feature/content-model` — universal content objects and relationships
- `experiment/*` — disposable experiments that should not affect stable work

## What GitHub can provide for this project

### Source control

- Full commit history
- Branches and isolated experiments
- Pull requests and review checkpoints
- Reversible changes

### Automation

Once application source is present, GitHub Actions can run:

- dependency installation
- linting
- type checking
- production builds
- deployment workflows

### Deployment

The project can later use GitHub Pages or another hosting provider. Hosting should remain replaceable; the Git repository remains the durable source.

### Collaboration with AI coding tools

The repository can be used from browser-based or local development environments and AI coding agents that support GitHub. This means Lovable does not need to be the only place where code can be created or maintained.

## Import rule

Do **not** recreate the Lovable application from memory and do **not** overwrite `main` with an unverified copy.

When importing the existing Lovable source:

1. Preserve the current Lovable commit as a reference checkpoint.
2. Import the source into a dedicated branch.
3. Verify routes, assets, build configuration, and responsive behavior.
4. Run checks before merging.
5. Record the source/version relationship in the project documentation.

## Long-term direction

The target architecture is:

`Personal Universe → Worlds → Content → Relationships → Timeline`

Dark Media is the first world, not the entire universe.
