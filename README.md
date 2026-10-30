# Tong Lin

AI agent engineering · Python · Context engineering · Evaluation harnesses

I build coding-agent tools with a focus on reliable execution, useful context, controllable permissions, and verifiable outcomes.

## Featured project

### [MiniClaudeCode](https://github.com/tonglynn/MiniClaudeCode)

A local coding-agent CLI built with Python, AsyncIO, Rich, and SQLite, with OpenAI-compatible and Anthropic-compatible backends.

- **Agent runtime:** streaming tool calls, 13 tools with deferred activation, concurrent reads, and resumable sessions.
- **Context and memory:** four-stage compression, persistent notes, semantic side queries, and asynchronous recall.
- **Execution controls:** five permission modes, declarative rules, dangerous-command checks, and validated edits.
- **Audit harness:** independent verification, execution traces, failure classification, and strategy ablations.

Release checks: **122 local tests passed**, **26 offline contract/verifier checks passed**, and **one live coding task independently verified**. These are separate checks; the offline results are not a model completion benchmark.

[Source and setup](https://github.com/tonglynn/MiniClaudeCode) · [Runtime design](https://github.com/tonglynn/MiniClaudeCode/blob/main/docs/design.md) · [Verification evidence](https://github.com/tonglynn/MiniClaudeCode/blob/main/VERIFICATION.md) · [中文说明](https://github.com/tonglynn/MiniClaudeCode/blob/main/docs/README.zh-CN.md)
