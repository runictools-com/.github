# RunicTools organization setup

## Confirmed requirements

- Source repositories for every service listed at `runictools.com` belong to `runictools-com`.
- Existing visibility, Git history, releases, issues, and production deployments remain intact.
- `eep0x10` and `RodrigoTR04` can maintain every active product.
- The organization has a clear public profile and reusable collaboration defaults.

## Repository map

| Product | Repository | Production |
| --- | --- | --- |
| Boardroom | `runictools-com/boardroom` | `kanban.runictools.com` |
| Game Promo Ranker | `runictools-com/game-promo-ranker` | `gamepromo.runictools.com` |
| Mesa20 | `runictools-com/mesa20` | `mesa20.runictools.com` |
| P3R 100% Guide | `runictools-com/p3r-100-guide` | `p3r.runictools.com` |
| P5R 100% Guide | `runictools-com/p5r-100-guide` | `p5r.runictools.com` |
| Pokefinder | `runictools-com/pokefinder` | `pokefinder.runictools.com` |
| WaaahGame | `runictools-com/waaahgame` | `waaah.runictools.com` |

## Organization contracts

- The `maintainers` team owns day-to-day write access to active products.
- Organization base permission stays `read`; repository write access is granted deliberately through teams.
- Members do not create new organization repositories by default. Owners can still create them.
- Active repositories use `main` as the default branch, remove merged branches automatically, and accept squash or merge commits.
- Issues are the shared backlog. Pull requests carry validation and deployment evidence.
- Vulnerabilities use GitHub private vulnerability reporting; credentials and production data never enter issues or Git.

## Execution slices and proof

1. **Ownership:** transfer the three personal repositories and resolve every public tool to an organization repository. Proof: GitHub reports the canonical `nameWithOwner` for all seven.
2. **Discoverability:** normalize product repository names, descriptions, homepages, and topics. Proof: organization repository inventory matches the product map.
3. **Collaboration:** create the maintainer team and assign both owners plus all active repositories. Proof: team membership and repository permission APIs return the intended state.
4. **Defaults:** publish the public `.github` repository and community health files. Proof: the organization overview renders the profile and GitHub exposes the default files.
5. **Local continuity:** update local `origin` URLs and verify every remote resolves without changing production checkouts or data.

## Containment and rollback

- GitHub preserves redirects from transferred and renamed repository URLs.
- Visibility is never changed as part of transfer or naming cleanup.
- Original branch refs are retained when adding `main`; no branch is deleted during setup.
- Production deploy directories and containers are not changed by this organization migration.

## Recommendations not enforced

- Use pull-request review for production, authentication, permissions, and persistent-data changes.
- Add repository-specific CI and branch rules only after each project's actual test commands are known; a generic required check could block both maintainers.
- Review the unrelated private organization repositories separately before archiving or renaming them.
