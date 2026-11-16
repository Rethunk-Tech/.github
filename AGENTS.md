# AGENTS.md

Org defaults for Rethunk-Tech. `profile/README.md` is the public org page and the other root files are the community health defaults for every org repo without its own. Copyright is Rethunk.Tech, LLC.

## Layout

- `profile/README.md`: the org profile with its pinned repositories.
- `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, `SECURITY.md`, `SUPPORT.md`: org-wide defaults.
- `.github/workflows/ci.yml`: actionlint over the workflow files in this repo. Also CodeQL, dependency review and Scorecard. `.github/dependabot.yml` for the actions.
- `.doc-audit.json`: skips the HUMANS and AGENTS tier checks, which do not apply to a templates repo.
- `lefthook.yml` and `.gitleaks.toml`: pre-commit secret scan.

## Verify

`actionlint` on any workflow you edit (CI runs it), then `gitleaks git --redact --no-banner`.

## Invariants

- The legal name is "Rethunk.Tech, LLC" in every license and legal line, never "Rethunk Technologies".
- The profile lists only public repos that exist; update it in the same commit as a repo is created, renamed or archived.
- Actions are pinned to a full commit SHA with a version comment.
