# Princeton RC agent kit

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Princeton RC Badge](https://img.shields.io/badge/Princeton_RC-2026--Current-%23F58025.svg)](https://researchcomputing.princeton.edu/)

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
