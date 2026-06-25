<p align="center">
  <img src="https://nexus-ts.github.io/nexusts/logo.svg" alt="NexusTS" width="400">
</p>

<h1 align="center">NexusTS</h1>

<p align="center">
  <strong>Bun-native fullstack framework</strong> — NestJS structure × Adonis productivity × Hono edge performance × TC39 standard ES decorators.
  32 modular packages under <code>@nexusts/*</code>.
  Ship only what you import. Zero overhead for what you don't.
</p>

<p align="center">
  <a href="https://nexus-ts.github.io/nexusts/">🌐 Website</a>
  ·
  <a href="https://github.com/nexus-ts/nexusts">📦 Repository</a>
  ·
  <a href="https://github.com/nexus-ts/nexusts/blob/main/docs/user-guide">📚 Documentation</a>
  ·
  <a href="https://github.com/nexus-ts/nexusts/blob/main/CHANGELOG.md">📝 Changelog</a>
</p>

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
@nexusts/core      → MVC + DI + routing + validation + view + standard decorators
@nexusts/cli       → `nx` CLI (scaffold, generate, seed, repl)
@nexusts/drizzle   → Default ORM (5 dialects: postgres/mysql/sqlite/bun-sqlite/d1)
@nexusts/auth      → better-auth integration
@nexusts/logger    → Pino-backed structured logging
@nexusts/graphql   → SDL-first + code-first (`autoSchema: true`)
@nexusts/resilience → Retry + Circuit Breaker + Bulkhead + HTTP admin
@nexusts/feature-flag → Canary deployments & A/B testing
@nexusts/cache     → Application cache (memory / Drizzle / Redis)
@nexusts/schedule  → Cron / Interval / Timeout (in-tree parser, zero deps)
... and 23 more →
```

## ✨ Key features

| Feature | Status |
|---------|--------|
| **TC39 standard ES decorators** (no experimentalDecorators, no reflect-metadata) | ✅ **v0.9.0** |
| Field injection (`@Inject(Token) declare field: Type`) | ✅ **v0.9.0** |
| HTTP + DI + Validation | ✅ Core |
| Exception Filters / Interceptors / Guards | ✅ v0.7.3 |
| Lifecycle Hooks (`OnModuleInit`, etc.) | ✅ v0.7.3 |
| Request-scoped DI | ✅ v0.4 |
| GraphQL (SDL + code-first) | ✅ v0.7.7 |
| WebSocket / SSE / gRPC (incl. streaming) | ✅ v0.8.2 |
| Circuit Breaker + Retry + Bulkhead + HTTP admin | ✅ v0.8.0 |
| Cross-pod circuit breaker (Redis / Drizzle) | ✅ v0.8.1 |
| Feature flags (canary / A/B testing) | ✅ v0.8.0 |
| REPL with `.services` / `.routes` / `.modules` | ✅ v0.7.4 |
| OpenAPI 3.1 + Scalar UI | ✅ v0.4 |
| Prometheus metrics / OpenTelemetry tracing | ✅ v0.4 |
| Inertia.js v3 (React / Vue) adapter + SSR scaffold | ✅ v0.8.4 |

## 📚 Docs & Links

- 🌐 **Website**: [nexus-ts.github.io/nexusts](https://nexus-ts.github.io/nexusts/)
- 📦 **Repository**: [nexus-ts/nexusts](https://github.com/nexus-ts/nexusts)
- [User Guide](https://github.com/nexus-ts/nexusts/tree/main/docs/user-guide)
- [Standard Decorator Migration Guide](https://github.com/nexus-ts/nexusts/blob/main/docs/design/standard-decorators-migration.md)
- [NestJS Comparison](https://github.com/nexus-ts/nexusts/blob/main/docs/analysis/nestjs-comparison.md)
- [AdonisJS Comparison](https://github.com/nexus-ts/nexusts/blob/main/docs/analysis/adonisjs-comparison.md)
- [Changelog](https://github.com/nexus-ts/nexusts/blob/main/CHANGELOG.md)

## 🏗 Status

**v0.9.0** — Standard decorator migration complete. TC39 standard ES
decorators, no reflect-metadata required. 32 packages, 323+ tests,
dual-mode backward compatibility with legacy decorators.

> **v1.0 target**: Production-ready LTS with semver guarantees.

## 🤝 Contributing

PRs welcome! See the [`AGENTS.md`](https://github.com/nexus-ts/nexusts/blob/main/AGENTS.md)
for module-author guidelines, standard decorator conventions, and the
7-step module addition workflow.

---

<p align="center">
  <sub>Built with Bun · TypeScript · Hono · Drizzle · TC39 standard decorators</sub>
</p>
