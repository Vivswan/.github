# .github

Default community health files for every repository under this account that does not carry its own, public and private alike. GitHub serves `CONTRIBUTING.md`, `SECURITY.md`, and `CODE_OF_CONDUCT.md` from here to any repository that lacks a file of the same name, and the issue forms as one set to any repository with no `.github/ISSUE_TEMPLATE/` of its own.

| File | Served to a repository without its own | Purpose |
|---|---|---|
| `CONTRIBUTING.md` | contributing guidelines link on new issues and pull requests | pull request, commit, CI, and licensing conventions shared by every repository |
| `SECURITY.md` | the Security tab's policy | the private vulnerability reporting route |
| `CODE_OF_CONDUCT.md` | the code of conduct badge and community profile | the unmodified Contributor Covenant v2.1 |
| `.github/ISSUE_TEMPLATE/bug_report.yml` | the new-issue chooser | bug report form |
| `.github/ISSUE_TEMPLATE/feature_request.yml` | the new-issue chooser | feature request form |
| `.github/ISSUE_TEMPLATE/config.yml` | the new-issue chooser | disables blank issues and links the private security reporting route |

A repository that needs its own version of `CONTRIBUTING.md`, `SECURITY.md`, or `CODE_OF_CONDUCT.md` commits that file; GitHub then serves the repository's copy for that file and the defaults for the rest. The issue forms are one set: a repository with any file under its own `.github/ISSUE_TEMPLATE/` uses only that set, so it must carry its own chooser config and security link too. Repository-specific toolchain instructions belong in each repository's `AGENTS.md` or README, not here.
