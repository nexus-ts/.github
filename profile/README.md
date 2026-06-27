<p align="center">
  <img src="https://nexus-ts.github.io/nexusts/logo.svg" alt="NexusTS" width="400">
</p>

<h1 align="center">NexusTS</h1>

<p align="center">
  <strong>Bun-native fullstack framework</strong> — NestJS structure × Adonis productivity × Hono edge performance × TC39 standard ES decorators.
  31 modular packages under <code>@nexusts/*</code>.
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
bun create nexusts@latest my-app
cd my-app
bun install
bun run dev
```

## 📦 Architecture

```
@nexusts/core      → MVC + DI + routing + validation + view + standard decorators
@nexusts/cli       → `nx` CLI (scaffold, generate, seed, repl)
@nexusts/drizzle   → Default ORM (5 dialects: postgres/mysql/sqlite/d1)
@nexusts/kysely    → Typed SQL query builder + Lucid-style repository
@nexusts/auth      → better-auth integration
@nexusts/logger    → Pino-backed structured logging
@nexusts/graphql   → SDL-first + code-first (`autoSchema: true`)
@nexusts/resilience → Retry + Circuit Breaker + Bulkhead + HTTP admin
@nexusts/feature-flag → Canary deployments & A/B testing
@nexusts/cache     → Application cache (memory / Drizzle / Redis)
@nexusts/schedule  → Cron / Interval / Timeout (in-tree parser, zero deps)
@nexusts/grpc      → gRPC unary + server/client/bidi streaming
@nexusts/health    → Liveness / Readiness / Startup probes (K8s-ready)
@nexusts/limiter   → Rate limiting (sliding-window / fixed-window / token-bucket)
@nexusts/metrics   → Prometheus counters / gauges / histograms / summaries
@nexusts/openapi   → OpenAPI 3.1 spec + Scalar UI
@nexusts/tracing   → OpenTelemetry distributed tracing
@nexusts/upload    → Multipart file upload with validation
@nexusts/shield    → CSRF, CORS, HSTS, CSP security middleware
@nexusts/static    → Static file serving (ETag, Range, MIME)
@nexusts/session   → Cookie / Redis / Cloudflare KV session storage
@nexusts/sse       → Server-Sent Events
@nexusts/ws        → WebSocket gateway + rooms + broadcast
@nexusts/view      → Rendu / Edge / Eta template engines + Inertia.js v3
@nexusts/config    → Zod-validated configuration with layered loading
```

## ✨ Key features

| Feature | Status |
|---------|--------|
| **Bun-native runtime** (Bun + Cloudflare Workers only) | ✅ **v0.9.9** |
| **Test runner: vitest → bun test** | ✅ **v0.9.9** |
| **experimentalDecorators removed** from root tsconfig | ✅ **v0.9.9** |
| **emitDecoratorMetadata removed** from all configs | ✅ **v0.9.9** |
| **GraphQL dual-mode** (@Resolver/@Query/@Mutation standard + legacy) | ✅ **v0.9.9** |
| **All decorators dual-mode** (TC39 standard + legacy) | ✅ **v0.9.7** |
| **DI container — field injection** (`@Inject(Token) declare field`) | ✅ **v0.9.7** |
| 18 modules: @Cacheable, @OnEvent, @RateLimit, @Cron, @Trace, @GrpcMethod, etc. | ✅ **v0.9.7** |
| gRPC streaming (server/client/bidi) | ✅ **v0.9.7** |
| TC39 standard ES decorators (no experimentalDecorators, no reflect-metadata) | ✅ **v0.9.0** |
| HTTP + DI + Validation | ✅ Core |
| Exception Filters / Interceptors / Guards | ✅ v0.7.3 |
| Lifecycle Hooks (`OnModuleInit`, etc.) | ✅ v0.7.3 |
| Request-scoped DI | ✅ v0.4 |
| GraphQL (SDL + code-first) | ✅ v0.7.7 |
| WebSocket / SSE | ✅ v0.8.2 |
| Circuit Breaker + Retry + Bulkhead + HTTP admin | ✅ v0.8.0 |
| Cross-pod circuit breaker (Redis / Drizzle) | ✅ v0.8.1 |
| Feature flags (canary / A/B testing) | ✅ v0.8.0 |
| REPL with `.services` / `.routes` / `.modules` | ✅ v0.7.4 |
| OpenAPI 3.1 + Scalar UI | ✅ v0.4 |
| Prometheus metrics / OpenTelemetry tracing | ✅ v0.4 |
| Inertia.js v3 (React / Vue) adapter + SSR scaffold | ✅ v0.8.4 |
| Kysely typed SQL query builder | ✅ v0.9.5 |
| CLI Kysely scaffold | ✅ v0.9.5 |
| Inline Reflect Metadata polyfill (no npm package needed) | ✅ v0.9.6 |
| WebSocket / SSE decorators dual-mode | ✅ v0.9.6 |

## 📚 Docs & Links

- 🌐 **Website**: [nexus-ts.github.io/nexusts](https://nexus-ts.github.io/nexusts/)
- 📦 **Repository**: [nexus-ts/nexusts](https://github.com/nexus-ts/nexusts)
- [User Guide](https://github.com/nexus-ts/nexusts/tree/main/docs/user-guide)
- [NestJS Comparison](https://github.com/nexus-ts/nexusts/blob/main/docs/analysis/nestjs-comparison.md)
- [AdonisJS Comparison](https://github.com/nexus-ts/nexusts/blob/main/docs/analysis/adonisjs-comparison.md)
- [Changelog](https://github.com/nexus-ts/nexusts/blob/main/CHANGELOG.md)

## 🏗 Status

**v0.9.10** — Bun-Native Standardization Complete. Test runner migrated
from vitest to `bun test`. `experimentalDecorators` and
`emitDecoratorMetadata` removed from all configs. Runtime support
narrowed to Bun + Cloudflare Workers. GraphQL decorators support
standard mode. 862+ tests, 31 packages, all passing with `bun test`.

> **v1.0 target**: Production-ready LTS with semver guarantees.

## 🤝 Contributing

PRs welcome! See the [`AGENTS.md`](https://github.com/nexus-ts/nexusts/blob/main/AGENTS.md)
for module-author guidelines, standard decorator conventions, and the
7-step module addition workflow.

---

<p align="center">
  <sub>Built with Bun · TypeScript · Hono · Drizzle · TC39 standard decorators</sub>
</p>
