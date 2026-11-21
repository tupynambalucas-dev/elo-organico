# Changelog - tupynambalucas-dev/elo-organico

All notable changes to the `elo-organico` commercial SaaS platform will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

<!-- changelog-start -->

## [0.2.0] - 2026-11-20

### Features & Capabilities

- [feat(git): adopt Evil Martians Lefthook for parallel pre-commit and commitlint #11](https://github.com/tupynambalucas-dev/elo-organico/pull/11) ([@tupynambalucas](https://github.com/tupynambalucas))

### Documentation & Specifications

- [docs(governance): standardize github flow, workflows, and documentation #9](https://github.com/tupynambalucas-dev/elo-organico/pull/9) ([@tupynambalucas](https://github.com/tupynambalucas))
- [docs(changelog): upgrade to keep a changelog format #12](https://github.com/tupynambalucas-dev/elo-organico/pull/12) ([@tupynambalucas](https://github.com/tupynambalucas))

### Bug Fixes & Corrections

- [fix(deps): bump mongoose from 9.7.3 to 9.11.4 #8](https://github.com/tupynambalucas-dev/elo-organico/pull/8) ([@tupynambalucas](https://github.com/tupynambalucas))

---

## [0.1.0] - 2026-05-05

The foundational release of Elo Organico (`v0.1.0`) establishes the core monorepo architecture, workspace isolation boundaries, and domain foundations for the local community shop and global platform hub.

### Features & Capabilities

- [feat(instance): Fastify v5 API server leveraging strict layered architecture (49ae855)](https://github.com/tupynambalucas-dev/elo-organico/commit/49ae855) ([@tupynambalucas](https://github.com/tupynambalucas))
- [feat(instance): implement initial domains: auth (JWT session state), product, and cycle (531ad0d)](https://github.com/tupynambalucas-dev/elo-organico/commit/531ad0d) ([@tupynambalucas](https://github.com/tupynambalucas))
- [feat(web): frontend workspace using React 19 with CSS Modules, routing, and backend API integration (dbcba51)](https://github.com/tupynambalucas-dev/elo-organico/commit/dbcba51) ([@tupynambalucas](https://github.com/tupynambalucas))
- [feat(portal): global SaaS portal skeleton with auth domain (8a18075)](https://github.com/tupynambalucas-dev/elo-organico/commit/8a18075) ([@tupynambalucas](https://github.com/tupynambalucas))
- [feat(studio): design tokens standardized in assets and Penpot design ops integration (c4718a5)](https://github.com/tupynambalucas-dev/elo-organico/commit/c4718a5) ([@tupynambalucas](https://github.com/tupynambalucas))

### Refactoring & Internal Architecture

- [refactor(monorepo): pnpm workspaces v11 and Turborepo task pipeline for workspace segregation (1f9d2ef)](https://github.com/tupynambalucas-dev/elo-organico/commit/1f9d2ef) ([@tupynambalucas](https://github.com/tupynambalucas))
- [refactor(boundaries): strict bounded contexts between instance and portal codebases (3af302b)](https://github.com/tupynambalucas-dev/elo-organico/commit/3af302b) ([@tupynambalucas](https://github.com/tupynambalucas))
- [refactor(core): domain core first with packages/core as Single Source of Truth (9c99bf8)](https://github.com/tupynambalucas-dev/elo-organico/commit/9c99bf8) ([@tupynambalucas](https://github.com/tupynambalucas))

[0.2.0]: https://github.com/tupynambalucas-dev/elo-organico/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/tupynambalucas-dev/elo-organico/releases/tag/v0.1.0
