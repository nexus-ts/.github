# NexusTS

**Bun-native fullstack framework** — 31 modular packages under `@nexusts/*`.
Ship only what you import. Zero overhead for what you don't.

---

## 🚀 Quick start

```bash
npm create nexusts@latest my-app
cd my-app
bun install
bun run dev
```

## 📦 Architecture

```
@nexusts/core      → MVC + DI + routing + validation + view
@nexusts/cli       → `nx` CLI (scaffold, generate, seed, repl)
@nexusts/drizzle   → Default ORM (5 dialects: postgres/mysql/sqlite/bun-sqlite/d1)
@nexusts/auth      → better-auth integration
@nexusts/logger    → Pino-backed structured logging
@nexusts/graphql   → SDL-first + code-first (`autoSchema: true`)
@nexusts/resilience → Retry + Circuit Breaker + Bulkhead
@nexusts/cache     → Application cache (memory / Drizzle / Redis)
@nexusts/schedule  → Cron / Interval / Timeout (in-tree parser, zero deps)
... and 22 more →
```

## ✨ Key features

| Feature | Status |
|---------|--------|
| HTTP + DI + Validation | ✅ Core |
| Exception Filters / Interceptors / Guards | ✅ v0.7.3 |
| Lifecycle Hooks (`OnModuleInit`, etc.) | ✅ v0.7.3 |
| Request-scoped DI | ✅ v0.4 |
| GraphQL (SDL + code-first) | ✅ v0.7.7 |
| WebSocket / SSE / gRPC | ✅ v0.5 |
| Circuit Breaker + Retry + Bulkhead | ✅ v0.7.0 |
| REPL with `.services` / `.routes` / `.modules` | ✅ v0.7.4 |
| OpenAPI 3.1 + Scalar UI | ✅ v0.4 |
| Prometheus metrics / OpenTelemetry tracing | ✅ v0.4 |
| Inertia.js v3 (React / Vue) adapter | ✅ v0.2 |

## 📚 Docs

- [User Guide](https://github.com/nexus-ts/nexusts/tree/main/docs/user-guide)
- [API Reference](https://github.com/nexus-ts/nexusts/blob/main/docs/api-reference.md)
- [NestJS Comparison](https://github.com/nexus-ts/nexusts/blob/main/docs/analysis/nestjs-comparison.md)
- [AdonisJS Comparison](https://github.com/nexus-ts/nexusts/blob/main/docs/analysis/adonisjs-comparison.md)

## 🏗 Status

**v0.7.8** — Active development. All Tier 1 & 2 gaps from NestJS/AdonisJS
closed. 31 packages, 67 smoke tests, 210+ unit tests.

> **v1.0 target**: Production-ready LTS with semver guarantees.

## 🤝 Contributing

PRs welcome! See the [`AGENTS.md`](https://github.com/nexus-ts/nexusts/blob/main/AGENTS.md)
for module-author guidelines, decorator conventions, and the 7-step
module addition workflow.

---

<p align="center">
  <sub>Built with Bun · TypeScript · Hono · Drizzle · reflect-metadata</sub>
</p>
