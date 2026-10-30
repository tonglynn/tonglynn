# Tong Lin

AI agent engineering · Python · Context engineering · Evaluation harnesses

I build coding-agent tools with a focus on reliable execution, useful context, controllable permissions, and verifiable outcomes.

## Featured projects

### [MiniClaudeCode](https://github.com/tonglynn/MiniClaudeCode)

A local coding-agent CLI built with Python, AsyncIO, Rich, and SQLite, with OpenAI-compatible and Anthropic-compatible backends.

- **Agent runtime:** streaming tool calls, 13 tools with deferred activation, concurrent reads, and resumable sessions.
- **Context and memory:** four-stage compression, persistent notes, semantic side queries, and asynchronous recall.
- **Execution controls:** five permission modes, declarative rules, dangerous-command checks, and validated edits.
- **Audit harness:** independent verification, execution traces, failure classification, and strategy ablations.

Release checks: **122 local tests passed**, **26 offline contract/verifier checks passed**, and **one live coding task independently verified**. These are separate checks; the offline results are not a model completion benchmark.

[Source and setup](https://github.com/tonglynn/MiniClaudeCode) · [Runtime design](https://github.com/tonglynn/MiniClaudeCode/blob/main/docs/design.md) · [Verification evidence](https://github.com/tonglynn/MiniClaudeCode/blob/main/VERIFICATION.md) · [中文说明](https://github.com/tonglynn/MiniClaudeCode/blob/main/docs/README.zh-CN.md)

### [Audit](https://github.com/tonglynn/Audit)

An independent **Offline Evaluation CLI for Coding Agents**, organized around task contracts, evidence collection, and multidimensional metric aggregation.

- Runs external agents in fresh fixture copies and independently verifies their final Python implementations.
- Collects execution traces, file changes, timing, reported usage, and four classes of failure.
- Supports repeated strategy comparisons, incremental reports, and an optional MiniClaudeCode adapter.

Release checks: **53 local tests passed**, **26 offline contract checks passed**, and **one real MiniClaudeCode task independently verified**. Process telemetry is labeled agent-reported; outcome verification runs separately.

[Source and setup](https://github.com/tonglynn/Audit) · [Contract and telemetry format](https://github.com/tonglynn/Audit/blob/main/docs/formats.md) · [Verification evidence](https://github.com/tonglynn/Audit/blob/main/VERIFICATION.md) · [CI](https://github.com/tonglynn/Audit/actions/workflows/ci.yml)
