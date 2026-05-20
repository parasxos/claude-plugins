# parasxos/claude-plugins

Personal [Claude Code](https://docs.claude.com/en/docs/claude-code) plugin
marketplace.

## Plugins

### [`cpp26-adapter`](./cpp26-adapter) — v0.9.0

Turn Claude into a C++26 specialist. Reflection, contracts, std::execution
senders, expansion statements, pack indexing, #embed, std::inplace_vector,
hazard pointers, RCU, library hardening, and the rest of the C++26 surface
— biased into Claude's defaults via skill + MCP + reviewer subagent.

**Recommendations follow the standard, not the toolchain.** If `clang 22` /
`gcc 16` don't yet implement a feature, the C++26 form is suggested
anyway; compiler errors are classified informationally as `compiler-lag`
vs `bug`.

Eval gate (held 39-task suite): **37/39 = 95%** standard-compliance.

```
/plugin install cpp26-adapter@parasxos/claude-plugins
```

See the plugin repo at [`parasxos/cpp26-adapter`](https://github.com/parasxos/cpp26-adapter)
— it carries the full 15-commit build history, the binding plan, and
the architecture document.

## Installing this marketplace

```
/plugin marketplace add parasxos/claude-plugins
/plugin install cpp26-adapter@parasxos/claude-plugins
```

## License

Each plugin carries its own license; see the plugin directory. Marketplace
metadata (`marketplace.json`, this README) is CC0 — copy freely.
