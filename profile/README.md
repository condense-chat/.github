<a href="https://condense.chat/"><img src="https://raw.githubusercontent.com/condense-chat/.github/main/condense.svg" width="100%" alt="Condense. Less context. Same agent."></a>

Every time an agent calls a model, it sends earlier messages and tool results again. Condense compresses that history and keeps the stable prefix cached, so long sessions cost less to run on Anthropic and OpenAI.

**[Connect your agent →](https://condense.chat/docs/quickstart/)** · **[Install the CLI →](https://github.com/condense-chat/dense#install)**

### Try it in your terminal

After installing `dense`, run a coding session through Condense and check what it saved.

```sh
dense claude     # also supports codex and opencode
dense info       # see token and cost savings
```

Using Hermes Agent? [Add the Hermes plugin](https://github.com/condense-chat/hermes-condense) to route its Anthropic requests through Condense.

### Reproduce the numbers

In our published Claude Haiku 4.5 comparison, Condense cut cost by about **28%** on sessions truncated to 190k tokens. The benchmark includes recorded usage, so you can recompute the result offline without an API key.

[Explore the benchmark and reference runs →](https://github.com/condense-chat/minmax-bench#see-cached-results)
