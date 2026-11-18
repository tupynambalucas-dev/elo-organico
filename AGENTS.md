<context-hierarchy>
  <parent src="../../AGENTS.md" type="meta-repository" />
  <system-instruction>
    AGENT: You are operating in the sovereign elo-organico commercial monorepo of tupynambalucas-dev. If you have not read ../../AGENTS.md in this session, read it for global ecosystem constraints.
  </system-instruction>
</context-hierarchy>

# Elo Orgânico Platform Agent Context

This document serves as the root context router (Layer 1) for AI agents operating within
the `tupynambalucas-dev/elo-organico` commercial software monorepo.

## Architectural Boundaries

- **Ecosystem Taxonomy**: Organic food distribution management, community marketplace cycles, and tenant SaaS portal.
- **Monorepo Engine**: Turborepo with strict pnpm catalogs (`catalogMode: 'strict'`).
- **Domain Separation**:
  - `instance/`: Community Shop operations, React SPA, Fastify API, BullMQ cycle worker, and MongoDB persistence.
  - `portal/`: Multi-tenant SaaS orchestration, platform landing page, global tenant gateway foundation.
  - `studio/`: Brand design tokens, SVG icon library, self-hosted Penpot services, and 3D assets.
  - `tools/`: Local MCP server adapters, Docker tooling, containerized agent runtime environments.
  - `docs/`: Docusaurus technical documentation portal (Handbook, Architecture, and Roadmaps).
  - `shared/`: Common tooling, ESLint configs, Prettier presets, and Husky git validation hooks.

## Workspace Navigation

- [README.md](./README.md): Primary platform documentation and operational runbook.
- [instance/README.md](./instance/README.md): Community instance application architecture.
- [instance/AGENTS.md](./instance/AGENTS.md): Local context router for community instance.
- [portal/README.md](./portal/README.md): SaaS platform portal architecture.
- [portal/AGENTS.md](./portal/AGENTS.md): Local context router for SaaS platform portal.
- [studio/README.md](./studio/README.md): Design tokens, SVG assets, and Penpot setup.
- [studio/AGENTS.md](./studio/AGENTS.md): Local context router for creative studio.
- [tools/README.md](./tools/README.md): MCP gateway and containerized agent tooling.
- [tools/AGENTS.md](./tools/AGENTS.md): Local context router for developer automation.
- [docs/README.md](./docs/README.md): Docusaurus engineering knowledge base documentation.
- [shared/README.md](./shared/README.md): Shared configuration presets and Git validation hooks.

## Governance Standards

- **Branching Model**: Single-Branch GitHub Flow on `main`. Short-lived branches MUST use Conventional Commit prefixes (`feat/`, `fix/`, `docs/`, `chore/`, `refactor/`, `ci/`, `perf/`, `test/`, `build/`, `style/`, `revert/`, `hotfix/`).
- **Cryptographic Signature**: All Git commits and annotated tags MUST be signed with SSH (`git commit -S -m "..."`).
- **Conventional Commits**: All commit messages must follow `<type>[optional (<scope>)][!]: <description>` (`<= 72` chars target, `<= 100` chars maximum).
- **Zero-Emoji Policy**: Emojis are strictly forbidden across all code, PRs, comments, documentation, and agent interactions.
- **Secret Hygiene**: Never commit plaintext tokens. Sourced via Infisical (`infisical run -- ...`) or local `.env` files.
- **Language Policy**: Code, comments, commit messages, and documentation must be written strictly in en-US.

## Architectural Plans & Artifact Dual-Storage Standard

Architectural blueprints, technical analyses, and master plans follow strict enterprise storage standards:

- **Storage Location**: Blueprints, analyses, and reports reside in `<target-repo>/.agents/plans/<artifact-slug>/` (or `<target-repo>/.agents/plans/<artifact-slug>.md`) within the respective repository for which the artifact is created. Creating a `plans/` directory at the root of any repository is strictly prohibited.
- **Topologies**: Topology 1 (Single-File Artifact) for atomic refactors, analyses, and reports; Topology 2 (Multi-Artifact Suite) for multi-domain frameworks with master `README.md` and numbered domain documents.
- **Dual-Storage Invariant**: Whenever an agent creates an architectural plan, analysis, or report artifact in the Antigravity conversation directory (`<appDataDir>/brain/<conversation-id>/`), an identical synchronized copy MUST ALWAYS be mirrored in `<target-repo>/.agents/plans/<artifact-slug>/` (or `<target-repo>/.agents/plans/<artifact-slug>.md`).
- **Ignore & Index Triad**: All repositories ignore `.agents/plans/` in `.gitignore`, while explicitly un-ignoring it in `.ignore` and `.rgignore` (`!.agents/plans/`, `!.agents/plans/**`) and setting `"search.useIgnoreFiles": false` in `.vscode/settings.json` so files can always be attached with `@`.

## Required Skills

Agents operating within this repository MUST autonomously engage the corresponding domain skills:

- **Atelier Plugin (`@tupynambalucas-dev/plugin-atelier`)**:
  - **`plan-architect`**: Designing, structuring, authoring, and auditing architectural plans, technical analyses, and governance reports following the dual-storage standard.
  - **`router-architect`**: Authoring, auditing, or updating hierarchical `AGENTS.md` context routers.
- **Repository Governance Plugin (`@tupynambalucas-dev/plugin-repo`)**:
  - **`monorepo-architect`**: Maintaining monorepo configurations, pnpm catalogs, package scopes, and Turborepo pipelines.
  - **`readme-architect` & `readme-auditor`**: Authoring or auditing `README.md` files and preserving recursive navigation.
  - **`community-health-architect`**: Auditing and aligning governance and health files.
- **GitHub Flow Plugin (`@tupynambalucas-dev/plugin-github-flow`)**:
  - **`github-flow-operator`**: Executing Git branching, SSH-signed Conventional Commits, and PR lifecycle workflows.
- **Secrets Plugin (`@tupynambalucas-dev/plugin-secrets`)**:
  - **`infisical-vault-operator`**: Managing secrets, environment variables, and Machine Identity tokens.
