# parasxos/claude-plugins

Personal [Claude Code](https://docs.claude.com/en/docs/claude-code) plugin
marketplace.

## Plugins

### [`cpp26-adapter`](https://github.com/parasxos/cpp26-adapter)

Turn Claude into a C++26 specialist — reflection, contracts, senders, `#embed`, expansion statements, pack indexing, `std::inplace_vector`, hazard pointers, RCU, library hardening, and the rest of the ISO/IEC 14882:2026 surface — biased into Claude's defaults via skill + MCP + reviewer subagent + hooks.

**Recommendations follow the standard, not the toolchain.** If `clang 22` /
`gcc 16` don't yet implement a feature, the C++26 form is suggested
anyway; compiler errors are classified informationally as `compiler-lag`
vs `bug`.

Eval gate (held 39-task suite, bar ≥85%):

- v0.9.0 published refresh: **37/39 = 95%** ✓
- v0.9.1 published refresh: **35/39 = 90%** ✓

Current pin: **v0.9.2** (hooks.json schema fix; corpus and behaviour identical to v0.9.1). Full history in the [plugin repo](https://github.com/parasxos/cpp26-adapter), including the binding plan and architecture document.

```
/plugin install cpp26-adapter@parasxos/claude-plugins
```

## Installing this marketplace

```
/plugin marketplace add parasxos/claude-plugins
/plugin install cpp26-adapter@parasxos/claude-plugins
```

## License

Each plugin carries its own license; see the plugin directory. Marketplace
metadata (`marketplace.json`, this README) is CC0 — copy freely.
