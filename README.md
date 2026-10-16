# Princeton RC agent kit

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Princeton RC Badge](https://img.shields.io/badge/Princeton_RC-2026--Current-%23F58025.svg?logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGlkPSJMYXllcl8xIiB2aWV3Qm94PSIwIDAgMzkyLjkgNTAwIj48ZGVmcz48c3R5bGU+LmNscy0xLC5jbHMtM3tzdHJva2Utd2lkdGg6MH0uY2xzLTN7ZmlsbDojZmZmfTwvc3R5bGU+PC9kZWZzPjxwYXRoIGQ9Ik0zODIgMjExYzE3LTgwIDktMTM4IDktMTM4QzI1OCAxMDkgMTk2IDAgMTk2IDBTMTM1IDEwOSAyIDczYzAgMC05IDU4IDkgMTM4aDM3MVoiIGNsYXNzPSJjbHMtMSIvPjxwYXRoIGQ9Ik0xMSAyMTFhNDgxIDQ4MSAwIDAgMCAxODUgMjg5IDU0NSA1NDUgMCAwIDAgMTM0LTE1M2MyOC00OCA0My05NSA1Mi0xMzZIMTFaIiBzdHlsZT0iZmlsbDojZjU4MDI1O3N0cm9rZS13aWR0aDowIi8+PHBhdGggZD0iTTE5NiAyMTggNjMgMzQ3YzEyIDIxIDI2IDQzIDQzIDY0bDkwLTg5IDkxIDg5YzE3LTIxIDMxLTQzIDQzLTY0TDE5NiAyMThaIiBjbGFzcz0iY2xzLTEiLz48cGF0aCBkPSJtMTc2IDg2LTE4IDNjLTkgMi0yMCAzLTMwLTF2ODZjNCAzIDExIDMgMTcgM2wzMC00YzctMSAxNC0xIDIwIDNWOTFjLTUtNi0xMi02LTE5LTVaTTIzNSA4OWwtMTktM2MtNi0xLTEzLTEtMTggNXY4NWM2LTQgMTMtNCAxOS0zbDMxIDRjNSAwIDEzIDAgMTctM1Y4OGMtMTAgNC0yMSAzLTMwIDFaIiBjbGFzcz0iY2xzLTMiLz48cGF0aCBkPSJtMTk2IDE5MSAxMC0xdi02YTM0NyAzNDcgMCAwIDAgNzAgMFY5OGwtOC0xdjc4cy0xIDMtNSA0Yy05IDMtMTUgMi0yMyAxbC0xNy0zYy05LTEtMTktNC0yNSA1di0xaC0zdjFjLTItMy00LTQtNi01LTYtMi0xMyAwLTE5IDBsLTE4IDNjLTcgMS0xMyAyLTIyLTEtNC0xLTUtNC02LTRWOTdsLTggMXY4NmM0IDEgMTcgMyAzMCAzIDIwIDAgMzktMyA0MS0zdjZsOSAxWk0xMDUgMTA5aDh2MTZoLTh6TTEwNSAxNTFoOHYxNWgtOHpNMjg4IDEyNWgtOHYtMTZoOHpNMjg4IDE2NmgtOHYtMTVoOHoiIGNsYXNzPSJjbHMtMyIvPjxwYXRoIGQ9Im0xNTIgMTA0LTMgMS01IDEyLTEgMXYtMWwtMy01LTEtNC0yLTMtMi0xdi0xaDh2MWwtMyAxaDFsMyA5IDMtNyAxLTItMi0xLTEtMWg3djFNMTY3IDExN2gtMTR2LTFoMmwxLTJ2LTlsLTMtMXYtMWgxM3Y0bC0zLTNoLTV2NWgybDItMXYtMWgxdjZoLTFsLTEtM2gtM3Y0bDEgMXYxaDVsMy0zdjRNMTg0IDEwN2gtMWwtMS0yLTItMWgtMnYxMGMwIDIgMSAyIDMgMnYxaC04di0xbDMtMXYtOWwtMS0yaC0ybC0zIDN2LTRoMTR2NE0xNTEgMTMwaC0xbC0xLTItMi0yaC0ydjExbDMgMmgtOGMyIDAgMi0xIDMtMnYtMTFoLTNsLTMgM3YxLTVoMTR2NU0xNjcgMTQwbC03LTFoLTcgMWwyLTF2LTEwYzAtMi0xLTItMi0ydi0xaDEybDEgMXYzaC0xbC0yLTItMS0xaC00djVoMmwxLTEgMS0xaDFsLTEgMyAxIDNoLTFsLTItMi0xLTFoLTF2NmwxIDFoM2wyLTFzMi0xIDItM2gxdjRsLTEgMU0xNzcgMTQwbC0zLTFoLTJ2LTRoMWwxIDIgMyAyIDItMSAxLTJ2LTFsLTItMS0zLTEtMi0yLTEtMmMwLTIgMi00IDQtNGw0IDF2LTFoMXY1aC0xbC0xLTMtMy0xLTIgMiAyIDIgMiAxIDIgMWMyIDEgMiAyIDIgNHMtMiA0LTUgNE0xNTcgMTYyaC0xNHYtMWgybDEtM3YtOGwtMy0yaDEzdjNoLTFsLTItMmgtNXY1aDJsMi0xdi0yaDF2N2wtMS0xLTEtMmgtM3Y1bDEgMWg1bDMtM3Y0TTE3NyAxNDhjLTEgMC0yIDEtMiAzdjExaC0xbC0xMC0xMXY4bDEgMmgydjFoLTd2LTFsMy0xdi05bC0xLTF2LTFsLTItMWg1bDcgOCAyIDJ2LTdsLTEtMi0yLTFoNy0xTTIyNCAxMDRjLTEgMC0yIDAtMiAzdjEwaC0xbC0xMC0xMXY4bDEgMmgydjFoLTd2LTFsMy0xdi04bC0xLTJ2LTFoLTJ2LTFoNWw3IDggMiAydi03bC0xLTJoLTJ2LTFoN3YxTTIzNyAxMDVsLTMtMi0yIDItMiA1IDEgNSAzIDJjMiAwIDMtMSAzLTJsMS01LTEtNW0yIDEwYy0xIDItMyAzLTUgM2wtNS0zLTItNSAyLTVjMi0yIDQtMiA1LTJsNCAxYzIgMSA0IDMgNCA2IDAgMi0xIDQtMyA1TTI2MCAxMDRsLTMgMS01IDEyLTEgMXYtMWwtMy01LTEtNC0yLTMtMi0xdi0xaDh2MWwtMiAxIDMgOSAzLTcgMS0yLTItMS0xLTFoN3YxTTIyMCAxMzBoLTFsLTEtMi0yLTJoLTJ2MTFsMyAyaC04YzIgMCAyLTEgMy0ydi05bC0xLTJoLTJsLTMgM3YxLTVoMTR2NU0yMjggMTI4bC0xIDItMSAzaDRsLTItNW05IDEyaC0xbC0zLTEtMyAxdi0xbDItMS0xLTItMS0yaC00bC0yIDN2MWwyIDFoLTYgMWwyLTEgMS00IDMtNSAxLTJ2LTJoMWwxIDEgMiA2IDIgMyAxIDMgMiAxdjFNMjU5IDE0MGwtNi0xaC0xIDFsMS0ydi0xMGwtMyA2LTEgMy0xIDNoLTFsLTEtMi01LTExdjEwYzAgMiAxIDMgMyAzdjFoLTFsLTMtMWgtM2wyLTEgMS0ydi04bC0xLTJoLTJ2LTFoNmwxIDEgNCA5IDEtMiAzLTYgMS0yaDV2MWwtMiAxdjhsMSA0aDF2MU0yMjAgMTUyaC0xbC0xLTItMy0xaC0xdjEwYzAgMiAxIDIgMyAydjFoLTh2LTFsMi0xdi0xMWgtMmwtMyAzaC0xdi00aDE1djRNMjM3IDE0OGwtMiAyLTYgMTJoLTFsLTItNi0yLTQtMS0yLTItMmg3bC0yIDF2MWw0IDkgMy03di0ybC0yLTJoNk0yNTkgMTYyaC03di0xaDFsMS0ydi0xMGwtMyA3LTEgMi0xIDNoLTFjLTEgMCAwIDAgMCAwbC0xLTItNS0xMHY5YzAgMiAxIDMgMyAzdjFoLTZ2LTFsMi0xdi0xMWwtMi0xaDZsNCAxMCAxLTIgMy03IDEtMWg1bC0yIDF2OWwxIDNoMXYxIiBjbGFzcz0iY2xzLTEiLz48L3N2Zz4=&labelColor=%235A575B)](https://researchcomputing.princeton.edu/)

A small set of project instructions for AI coding assistants working with
Princeton Research Computing (RC) clusters. The guidance is primarily for
researchers and developers who use Princeton RC systems and want their
assistant to account for cluster-specific documentation, policies, and
workflows.

## Files

- [`AGENTS.md`](AGENTS.md) contains the shared instructions. It directs
  assistants to use current Princeton RC documentation as the source of truth
  and summarizes practical guidance for Slurm, storage, modules, Python, and
  other common cluster tasks.
- [`CLAUDE.md`](CLAUDE.md) imports `AGENTS.md` for Claude Code, so the same
  guidance is available without maintaining a separate copy.

## How to use

### Use across projects (recommended for beginners)

#### Codex

Put `AGENTS.md` at `~/.codex/AGENTS.md`.

#### Claude Code

Put both `CLAUDE.md` and `AGENTS.md` in `~/.claude/`. Claude Code loads
`CLAUDE.md`, which imports the adjacent `AGENTS.md`.

#### Google Antigravity

Add the contents of `AGENTS.md` to your global rules in Antigravity's agent
settings. Global rules are managed in the application rather than by placing
this file in the project.

#### GitHub Copilot

Add the guidance to your personal instructions in Copilot settings, if that
option is available for your Copilot plan and client. Otherwise, use the
project-specific setup below.

### Use in one project only

Project-level files keep the guidance scoped to a project and shareable with
collaborators.

#### Codex

Put `AGENTS.md` in the project root.

#### Claude Code

Put both `CLAUDE.md` and `AGENTS.md` in the project root.

#### Google Antigravity

Add the guidance as a project rule under `.agent/rules/`.

#### GitHub Copilot

Create `.github/copilot-instructions.md` and copy the relevant guidance into
it. Copilot's repository instructions use that filename rather than loading
`AGENTS.md` directly in every client.

For personalization, edit the **User-specific preferences** section near the
bottom of `AGENTS.md`. For example, add your preferred programming language,
tools, or workflow there. Keep cluster-wide policies and shared recommendations
in the main guidance, and put individual preferences in that section.

### Where to run your assistant

For the best compatibility with Princeton RC environments, we strongly
recommend using it in an RC-supported cluster environment with access to your
project files—for example, a terminal tool or VS Code connected through Remote
SSH. Confirm the assistant works on the remote project and can read its
instructions; a local desktop app may lack access to cluster files, modules,
and software even if it connects to a remote service. Check the tool's
documentation, follow node-specific rules, and submit compute workloads through
Slurm.

The files provide context and guardrails, not a substitute for checking current
RC documentation or your project's requirements. User-level instructions apply
across projects; use project-level files when you want different guidance for a
particular project. Removing these instructions or adding abusive or
policy-violating instructions does not exempt users from RC policies. Accounts
are subject to review, and misuse may result in suspension or removal, as
provided under applicable policies.

For work involving a cluster, identify the relevant cluster and partition and
check the current Princeton RC guidance before suggesting commands or running
jobs. In particular, verify Slurm/QOS limits before preparing or submitting
test jobs. Cluster policies and available software can change.

## Contributing

Contributions are welcome, especially corrections that improve clarity or
reflect changes in Princeton RC guidance. Please open a pull request and include
a link to relevant current RC documentation when proposing policy or command
updates. Maintainers review contributions as time allows, so a response or
merge may take a while; not every proposal can be accepted. Keep shared guidance
in `AGENTS.md` rather than duplicating it in assistant-specific files.

## License

This project is available under the [MIT License](LICENSE).
