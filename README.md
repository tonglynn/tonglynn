<picture>
  <source media="(max-width: 600px) and (prefers-color-scheme: dark)" srcset="assets/cards/header-mobile-dark.svg">
  <source media="(max-width: 600px)" srcset="assets/cards/header-mobile-light.svg">
  <source media="(prefers-color-scheme: dark)" srcset="assets/cards/header-dark.svg">
  <img src="assets/cards/header-light.svg" width="100%" alt="Tong Lin — Coding agents, memory systems, and independent evaluation. Python, AsyncIO, MCP, SQLite.">
</picture>

I build coding agents and the systems that help teams remember, inspect, and verify their work.

## Selected work

<a href="https://github.com/tonglynn/attest-agent-memory">
  <picture>
    <source media="(max-width: 600px) and (prefers-color-scheme: dark)" srcset="assets/cards/attest-mobile-dark.svg">
    <source media="(max-width: 600px)" srcset="assets/cards/attest-mobile-light.svg">
    <source media="(prefers-color-scheme: dark)" srcset="assets/cards/attest-dark.svg">
    <img src="assets/cards/attest-light.svg" width="100%" alt="Attest: MCP memory server with an evidence gateway, scoped recall, and human review. 177 passing tests; 450 preregistered study runs; 60 synthetic attacks. One model, synthetic benchmark; limits and negative findings are public.">
  </picture>
</a>

[![MCP server](https://img.shields.io/badge/MCP-server-285fa8)](https://github.com/tonglynn/attest-agent-memory/blob/main/docs/MCP_DEMO.md) [![Attest CI](https://github.com/tonglynn/attest-agent-memory/actions/workflows/ci.yml/badge.svg)](https://github.com/tonglynn/attest-agent-memory/actions/workflows/ci.yml)

[Interactive demo](https://tonglynn.github.io/attest-agent-memory/) · [Results & limitations](https://github.com/tonglynn/attest-agent-memory/blob/main/RESULTS.md) · [Preregistered protocol](https://github.com/tonglynn/attest-agent-memory/blob/main/PREREGISTRATION.md) · [中文](https://github.com/tonglynn/attest-agent-memory/blob/main/README.zh-CN.md)

<a href="https://github.com/tonglynn/MiniClaudeCode">
  <picture>
    <source media="(max-width: 600px) and (prefers-color-scheme: dark)" srcset="assets/cards/runtime-mobile-dark.svg">
    <source media="(max-width: 600px)" srcset="assets/cards/runtime-mobile-light.svg">
    <source media="(prefers-color-scheme: dark)" srcset="assets/cards/runtime-dark.svg">
    <img src="assets/cards/runtime-light.svg" width="100%" alt="MiniClaudeCode: async coding-agent runtime with deferred tools, streaming, permissions, context compression, and resumable sessions. Release evidence: 122 tests, 26 offline contract checks, Windows/Ubuntu CI, one live model task.">
  </picture>
</a>

[Runtime design](https://github.com/tonglynn/MiniClaudeCode/blob/main/docs/design.md) · [Release verification](https://github.com/tonglynn/MiniClaudeCode/blob/main/VERIFICATION.md) · [Live-run evidence](https://github.com/tonglynn/MiniClaudeCode/blob/main/evidence/live-smoke.json)

<a href="https://github.com/tonglynn/Audit">
  <picture>
    <source media="(max-width: 600px) and (prefers-color-scheme: dark)" srcset="assets/cards/audit-mobile-dark.svg">
    <source media="(max-width: 600px)" srcset="assets/cards/audit-mobile-light.svg">
    <source media="(prefers-color-scheme: dark)" srcset="assets/cards/audit-dark.svg">
    <img src="assets/cards/audit-light.svg" width="100%" alt="Audit: independent coding-agent evaluation with task contracts, fresh fixtures, final-code verification, and failure traces. Release evidence: 53 tests and 26 offline contract checks, plus one real MiniClaudeCode integration run.">
  </picture>
</a>

[Contracts & telemetry](https://github.com/tonglynn/Audit/blob/main/docs/formats.md) · [Release verification](https://github.com/tonglynn/Audit/blob/main/VERIFICATION.md) · [Integration evidence](https://github.com/tonglynn/Audit/blob/main/evidence/live-smoke.json)

<sub>Release checks for MiniClaudeCode and Audit validate reconstructed fixtures and the evaluator. Each has one live model task; these are not full model benchmarks.</sub>

<details>
<summary>More projects</summary>

- [tiny-agent-harness](https://github.com/tonglynn/tiny-agent-harness) — Hidden-test evaluation and ablations.
- [Tabular classification skill](https://github.com/tonglynn/in6227-tabular-classification-skill) — Reusable data-mining and reporting workflows.

</details>
