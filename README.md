<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/profile-compact-dark.svg">
  <img src="assets/profile-compact-light.svg" width="100%" alt="Tong Lin — Developer tools for coding agents">
</picture>

I build developer tools for coding agents, with a focus on memory, execution, and evaluation. Most of my work is in Python.

## Attest

[![A recorded Claude Desktop session: learning, evidence checks, and human review](https://raw.githubusercontent.com/tonglynn/attest-agent-memory/main/docs/assets/live_run.gif)](https://tonglynn.github.io/attest-agent-memory/)

<sub>Recorded with Claude Desktop and the Attest MCP server. Open the project for the interactive walkthrough.</sub>

**Memory that coding agents can learn from, and people can review and retract.**

[Attest](https://github.com/tonglynn/attest-agent-memory) turns code-review feedback into reusable project knowledge. An evidence gateway checks proposed notes against verified changes, scopes them to the relevant repository and version, and routes uncertain notes for human review. It is available as an MCP server.

In a preregistered experiment, held-out first-attempt pass rate rose from **33% without memory to 70% with Attest**. This was an author-designed synthetic benchmark with one model and 11 held-out tasks, repeated three times; the results report covers the tradeoffs and later security experiments.

[Try the demo](https://tonglynn.github.io/attest-agent-memory/) · [Code & setup](https://github.com/tonglynn/attest-agent-memory) · [Results & limitations](https://github.com/tonglynn/attest-agent-memory/blob/main/RESULTS.md) · [中文](https://github.com/tonglynn/attest-agent-memory/blob/main/README.zh-CN.md)

## Other projects

### [MiniClaudeCode](https://github.com/tonglynn/MiniClaudeCode)

A local coding agent with an asynchronous Python runtime, streaming model responses, permission controls, and resumable sessions. Built to explore tool execution, context compression, and persistent memory.

[Runtime design](https://github.com/tonglynn/MiniClaudeCode/blob/main/docs/design.md) · [Verification](https://github.com/tonglynn/MiniClaudeCode/blob/main/VERIFICATION.md)

### [Audit](https://github.com/tonglynn/Audit)

A CLI for evaluating coding agents against explicit task contracts. Runs agents in fresh fixtures, checks their final implementations independently, and records failures and execution traces for comparison.

[Contracts & telemetry](https://github.com/tonglynn/Audit/blob/main/docs/formats.md) · [Verification](https://github.com/tonglynn/Audit/blob/main/VERIFICATION.md)

Also: [tiny-agent-harness](https://github.com/tonglynn/tiny-agent-harness), for hidden-test evaluation and ablations; [tabular classification skill](https://github.com/tonglynn/in6227-tabular-classification-skill), a reusable data-mining and reporting workflow.
