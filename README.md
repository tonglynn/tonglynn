<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/profile-compact-dark.svg">
  <img src="assets/profile-compact-light.svg" width="100%" alt="Tong Lin — Coding agents, memory systems, and evaluation">
</picture>

I build coding agents and the infrastructure around them: asynchronous tool runtimes, evidence-backed memory, and independent evaluation. My work connects the agent that makes a change with the systems that remember and verify it.

`Python` · `AsyncIO` · `MCP` · `SQLite` · `pytest`

## Attest — governed memory for coding agents

[![MCP server](https://img.shields.io/badge/MCP-server-255fb2)](https://github.com/tonglynn/attest-agent-memory/blob/main/docs/MCP_DEMO.md)
[![Attest CI](https://github.com/tonglynn/attest-agent-memory/actions/workflows/ci.yml/badge.svg)](https://github.com/tonglynn/attest-agent-memory/actions/workflows/ci.yml)

**Learn from code review. Recall in scope. Let people review and retract.**

[Attest](https://github.com/tonglynn/attest-agent-memory) is an MCP server that turns review feedback into reusable team knowledge. A deterministic evidence gateway checks candidate notes against verified changes; repository and version scopes govern recall, while a separate admin interface handles human decisions.

**Open evidence:** [177 passing tests across Python 3.11–3.13](https://github.com/tonglynn/attest-agent-memory/actions/workflows/ci.yml) · [450 preregistered experiment runs](https://github.com/tonglynn/attest-agent-memory/tree/main/runs/main) · [60 synthetic attacks across six write channels](https://github.com/tonglynn/attest-agent-memory/tree/main/runs/poison_channels)

The main study measured **33% → 70% first-attempt pass rate** on 11 synthetic held-out tasks, repeated three times with one model. [Results](https://github.com/tonglynn/attest-agent-memory/blob/main/RESULTS.md) distinguish the original gate from later gateways, and report tradeoffs and negative findings.

[![Recorded Claude Desktop session: learning, evidence checks, and human review](https://raw.githubusercontent.com/tonglynn/attest-agent-memory/main/docs/assets/live_run.gif)](https://tonglynn.github.io/attest-agent-memory/)

<sub>Recorded Claude Desktop + MCP session in a synthetic billing repository. Agent, server, and tests ran for real; review comments and approver identities were simulated.</sub>

[Interactive demo](https://tonglynn.github.io/attest-agent-memory/) · [Code & setup](https://github.com/tonglynn/attest-agent-memory) · [Preregistered protocol](https://github.com/tonglynn/attest-agent-memory/blob/main/PREREGISTRATION.md) · [中文](https://github.com/tonglynn/attest-agent-memory/blob/main/README.zh-CN.md)

## Agent runtime & evaluation

### [MiniClaudeCode](https://github.com/tonglynn/MiniClaudeCode)

An asynchronous Python coding-agent runtime with deferred tools, streaming model responses, five permission modes, context compression, persistent memory, and resumable sessions.

**Release verification:** [122 passing tests and 26/26 offline contract checks](https://github.com/tonglynn/MiniClaudeCode/blob/main/VERIFICATION.md). CI covers Windows and Ubuntu on Python 3.12/3.13; one live model task passed independent verification.

[Runtime design](https://github.com/tonglynn/MiniClaudeCode/blob/main/docs/design.md) · [CI](https://github.com/tonglynn/MiniClaudeCode/actions/workflows/ci.yml) · [Live-run evidence](https://github.com/tonglynn/MiniClaudeCode/blob/main/evidence/live-smoke.json)

### [Audit](https://github.com/tonglynn/Audit)

An independent evaluation CLI: explicit task contracts, fresh fixtures, external agent execution, final-code verification, failure classification, and trace collection. Checks include timeout handling, protected-file changes, tampered verifier snapshots, and installed-wheel validation.

**Release verification:** [53 passing tests and 26/26 offline contract checks](https://github.com/tonglynn/Audit/blob/main/VERIFICATION.md), plus one real MiniClaudeCode integration run. Offline contract checks validate the evaluator; they do not measure model success rate.

[Contracts & telemetry](https://github.com/tonglynn/Audit/blob/main/docs/formats.md) · [CI](https://github.com/tonglynn/Audit/actions/workflows/ci.yml) · [Integration evidence](https://github.com/tonglynn/Audit/blob/main/evidence/live-smoke.json)

Also: [tiny-agent-harness](https://github.com/tonglynn/tiny-agent-harness), for hidden-test evaluation and ablations; [tabular classification skill](https://github.com/tonglynn/in6227-tabular-classification-skill), for reusable data-mining and reporting workflows.
