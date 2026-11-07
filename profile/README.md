<a href="https://condense.chat/"><img src="https://raw.githubusercontent.com/condense-chat/.github/main/profile/condense-banner.png" width="100%" alt="Condense. Less context. Same agent."></a>

Long-running agents resend earlier messages, file reads, and tool results on every turn. Condense compresses that history and keeps the stable prefix cached to reduce model costs on Anthropic and OpenAI.

**[Connect your agent](https://condense.chat/docs/quickstart/)** · **[Install the CLI](https://github.com/condense-chat/dense#install)**

### Try it in your terminal

Use [`dense`](https://github.com/condense-chat/dense) to run Claude Code, Codex, or OpenCode through Condense. After installing, launch the agent you already use:

```sh
dense claude     # or: dense codex, dense opencode
```

Type `/dense:info` inside the agent to see the input tokens and model cost for that session. Using Hermes Agent? [Add the Hermes plugin](https://github.com/condense-chat/hermes-condense) to route its Anthropic requests through Condense.

### Reproduce the benchmark

**63.8% lower estimated model cost** across 64 recorded coding sessions. In an offline replay of all 11,712 turns, estimated model cost fell from **$861.28 to $312.20**. The benchmark simulates prompt caching and prices token usage at Claude Opus 4.8 rates, excluding Condense fees.

[Watch the replay](https://github.com/condense-chat/dense#reproduce-the-benchmark) · [Inspect the run data](https://github.com/condense-chat/minmax-bench/tree/main/runs/run-5c61ab52-8eea-4fee-97a4-5c64ee5344af) · [Explore the quality evaluation](https://github.com/condense-chat/minmax-bench/blob/main/docs/quality.md)
