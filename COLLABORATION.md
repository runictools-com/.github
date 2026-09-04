# Working together

You only need four GitHub concepts for the normal RunicTools workflow:

1. An **issue** records a bug, idea, or piece of work.
2. A **branch** isolates the changes for that issue.
3. A **pull request** shows the change and gives the other maintainer a place to review it.
4. A **merge** puts the approved change into the default branch.

## Recommended workflow

1. Create an issue when the work needs discussion or should not be forgotten.
2. Create a branch named `fix/short-name`, `feat/short-name`, or `docs/short-name`.
3. Make small commits with an outcome-focused message, such as `fix: preserve notes when switching workspaces`.
4. Open a pull request and complete its checklist.
5. Ask the other maintainer to review changes that affect production, persistent data, authentication, or shared interfaces.
6. Merge after automated checks and the relevant manual check pass.
7. Delete the merged branch. GitHub is configured to do this automatically.

## Responsibilities

- Both organization owners can administer every repository and recover access.
- The `maintainers` team is the normal collaboration group for active products.
- Repository secrets belong in GitHub Actions secrets or the production secret store, never in Git.
- Production databases, uploaded files, volumes, and backups are not source code and must never be committed.

## When a pull request is optional

An owner may commit directly for an urgent, low-risk correction. Use a pull request for authentication, permissions, persistent data, deployment, or broad refactors so the change has a review trail.
