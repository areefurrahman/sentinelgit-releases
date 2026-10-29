# Changelog

All notable changes to SentinelGit AI are listed here. The format follows
[Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and versions follow
[Semantic Versioning](https://semver.org/). The app's "What's new" dialog is built from this file.

## [Unreleased]

## [0.9.0] - 2026-10-24

The first public beta.

### Added

- Multi-agent audits of a `git diff`: SecOps Guardian, AI Slop Detector and Architecture Critic review your changes in parallel, plus any agents you create.
- The War Room: agents that disagree debate the contested findings in rounds, and a moderator records the verdict. Replay any past scan.
- The Diff Workbench: a targeted AI fix prompt and a patch checked with `git apply --check` for each finding. Applying a patch is always your click. A model-written patch with no context lines, a broken `@@` header or a one-space indent drift is rebuilt against your file first, so more of them apply.
- Auto-scan commits: turn it on for a repository and every new commit you make there is scanned on its own (that commit only). Off by default, since it uses your model key.
- Agent Studio: describe a rule in plain words; SentinelGit proposes a zero-token regex rule, a rule for an agent's prompt, or a new agent, and you decide.
- Three scan modes: uncommitted changes, a commit range, or files you choose.
- Your own model key (Google Gemini by default; Groq, OpenAI or Anthropic), kept in the OS keychain. Secrets found in a diff are redacted before any prompt is built.
- Repositories that stay current: branch, changed files and the last scan's open findings, refreshed as you work.
- Scan history with Markdown and JSON reports, keyboard shortcuts, a command palette (Ctrl/⌘+K) and dark, light or system themes.
- Installers for Windows, macOS and Linux with the backend bundled; no Python install needed.
- Opt-in update checks (Settings > About), off until you turn them on.
- Free, Pro and Team plans. The Free plan's limits apply until you activate a license key in Account & License; keys are verified offline and can be bound to one machine.
- A first-run tour and this "What's new" dialog.

[Unreleased]: https://github.com/areefurrahman/sentinelgit-releases/releases
[0.9.0]: https://github.com/areefurrahman/sentinelgit-releases/releases/tag/v0.9.0
