# Contributing to Tokens United

Thanks for working with us. This guide applies across Tokens United repositories and is aimed at our team and the collaborators, contractors, and candidates who build alongside us. The goal is simple: keep our work consistent, secure, and easy to review.

By participating, you agree to uphold our [Code of Conduct](./CODE_OF_CONDUCT.md).

## Before you start

- Make sure there's an issue describing the work. For anything non-trivial, agree on the approach first.
- Read the repository's own `README.md` and any `CLAUDE.md` / architecture docs — each project documents its own setup, conventions, and non-negotiables.
- Never commit secrets. All configuration comes from environment variables, prefixed `TU_` (e.g. `TU_DATABASE_URL`). If you think a secret was exposed, stop and follow our [Security Policy](./SECURITY.md).

## Branches

Work on a focused branch off the project's default branch — one feature or fix per branch:

```
feat/<scope>      # a new capability
fix/<scope>       # a bug fix
refactor/<scope>  # restructuring without behaviour change
chore/<scope>     # tooling, deps, housekeeping
docs/<scope>      # documentation only
```

Never push directly to `main`.

## Commits

- Keep commits small and atomic — the project should work after each one.
- Write subjects in the imperative mood: *"add invoice tax line"*, not *"added"* or *"adds"*.
- Use a conventional prefix where the repo already does: `feat:`, `fix:`, `refactor:`, `chore:`, `docs:`, `test:`, `perf:`.
- Explain the *why* in the body when it isn't obvious.

## Pull requests

Open a PR against the default branch using the repository's PR template. A good PR:

- **Is small and reviewable.** Split large changes into a sequence of PRs.
- **Describes what and why**, links the issue it closes (`Closes #123`), and includes a clear test plan.
- **Passes the checks** — lint, type-check, and tests all green. Don't bypass hooks with `--no-verify`; if a check blocks you, fix the cause.
- **Adds no secrets**, and respects the project's architecture and style rules.
- **Respects access control.** Where the change touches data or actions, permissions and roles (RBAC) must be enforced server-side — never assume the frontend will hide it.

## Code quality, in short

- Match the surrounding code: its naming, structure, and conventions.
- Prefer reusing or extending existing components, hooks, and services over adding duplicates.
- Handle errors explicitly and validate input at the boundaries.
- Update docs when behaviour changes.

## Security & conduct

- Security issues go through the [Security Policy](./SECURITY.md) — privately, never in a public issue or PR.
- All interaction is governed by our [Code of Conduct](./CODE_OF_CONDUCT.md).
- Need help or have a question? See [SUPPORT](./SUPPORT.md).

We review every contribution with care and appreciate the effort you put in. Thank you for helping us build well.
