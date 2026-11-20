# Changelog

All notable changes to the `elo-organico` commercial SaaS platform will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

<!-- changelog-start -->

## [0.1.0] - 2026-05-05

The foundational release of Elo Organico (`v0.1.0`) establishes the core monorepo architecture, workspace isolation boundaries, and domain foundations for the local community shop and global platform hub.

### Features & Capabilities

- [FEAT] (instance): Fastify v5 API server (`@elo-instance/api`) leveraging strict layered architecture (`Controller -> Service -> Repository -> Model`).
- [FEAT] (instance): implement initial domains: `auth` (JWT session state), `product` (catalog & inventory), and `cycle` (cooperative cycles).
- [FEAT] (web): frontend workspace `@elo-instance/web` using React 19 with CSS Modules, routing, and backend API integration.
- [FEAT] (portal): global SaaS portal skeleton (`@elo-portal/api`, `@elo-portal/web`, and `@elo-portal/core`) with auth domain.
- [FEAT] (studio): design tokens standardized in `@elo-studio/assets` and Penpot design ops integration.
- [FEAT] (tooling): Model Context Protocol (MCP) SSE gateway for LLM client integration exposing GitHub, Context7, and Playwright interfaces.

### Refactoring & Internal Architecture

- [REFACTOR] (monorepo): pnpm workspaces v11 and Turborepo task pipeline for workspace segregation.
- [REFACTOR] (boundaries): strict bounded contexts between `instance` and `portal` codebases enforced via ESLint and TypeScript constraints.
- [REFACTOR] (core): domain core first with `packages/core` as Single Source of Truth (SSOT) for data models and schemas.

### Documentation & Specifications

- [DOCS] (knowledge-base): EloDocs Docusaurus developer portal for architectural references, guides, and style guides.

[0.1.0]: https://github.com/tupynambalucas-dev/elo-organico/releases/tag/v0.1.0
