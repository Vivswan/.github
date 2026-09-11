# Contributing

Thanks for contributing! This document covers the conventions every change in this repository goes through. Toolchain-specific instructions (setup, build, and test commands) live in the repository's own `AGENTS.md` or README.

CI, settings, and standards files in Vivswan's repositories are managed by [Vivswan/repo-platform](https://github.com/vivswan/repo-platform); local edits to managed files are replaced on the next repo-platform sync.

## Pull requests

- Changes land through pull requests and are squash-merged; the PR title becomes the commit subject on the default branch.
- The PR title and every pushed commit subject must be a [Conventional Commit](https://www.conventionalcommits.org/en/v1.0.0/), for example `feat: add X` or `fix(parser): handle Y`. Releases are versioned from these subjects.
- By opening a pull request, or offering code in an issue or review for inclusion, you agree to the Contributions section of the repository's `LICENSE.md` where it has one, which licenses that code to the licensor - including for relicensing under any terms - unless you conspicuously say otherwise when you submit it.

## CI

- In repositories managed by repo-platform, CI gates on the `all-green` status check - the CI workflow's own `all-green` job, which needs every gating job and fails unless each result is success or skipped, with at least one success (the convention is documented in [repo-platform's all-green guide](https://github.com/vivswan/repo-platform/blob/main/docs/all-green.md)).
- Repository-specific checks live in the repository's `.github/workflows/checks.yml` where it has one; run the commands it lists locally before pushing.
- Those repositories' CI also runs a typography gate enforcing plain ASCII punctuation: no curly quotes, em-dashes, or invisible unicode.

## Security

Never report vulnerabilities in issues or pull requests: the repository's security policy (its Security tab) gives the private reporting route.

## Code of conduct

Participation in this project is governed by the repository's code of conduct (the Contributor Covenant unless the repository carries its own).
