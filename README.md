# Architecture Resources

A curated collection of resources for modern software architecture — covering architecture-as-code tooling, standards, patterns, and AI agent skills for the SDLC.

---

## Contents

- [Pattern Library](#pattern-library)
- [Architecture as Code](#architecture-as-code)
- [Architecture Standards](#architecture-standards)
- [Architecture Patterns](#architecture-patterns)
- [Agent Skills for the SDLC](#agent-skills-for-the-sdlc)

---

## Pattern Library

Architecture pattern reference files — each covering intent, structure, trade-offs, and implementation guidance.

| Pattern | Description |
| ------- | ----------- |
| [Layered Architecture](./layered-architecture.md) | Horizontal tiers (Presentation → Application → Domain → Infrastructure) with unidirectional dependencies. The standard starting point for most systems. |
| [Event-Driven Architecture](./event-driven-architecture.md) | Components communicate through immutable events via a broker. Decouples producers and consumers in time and logic. |
| [Microservices Architecture](./microservices-architecture.md) | Independently deployable services, each owning a single business capability and its data. |
| [CQRS & Event Sourcing](./cqrs-event-sourcing.md) | Separates read and write models; persists state as an append-only event log rather than current values. |
| [Domain-Driven Design](./domain-driven-design.md) | Centres design on the business domain using a shared language, bounded contexts, and rich domain objects. |
| [Hexagonal Architecture](./hexagonal-architecture.md) | Domain at the centre; all external systems connect through explicitly defined ports and adapters. |
| [Microkernel Architecture](./microkernel-architecture.md) | Minimal stable core extended by independently developed and deployed plugins. |
| [Space-Based Architecture](./space-based-architecture.md) | Distributed in-memory data grid across processing units eliminates the database as the scaling bottleneck. |
| [Serverless Architecture](./serverless-architecture.md) | Functions as the unit of deployment; cloud provider manages all infrastructure, scaling, and availability. |
| [Multi-Tenancy Patterns](./multi-tenancy-patterns.md) | Silo, Pool, and Bridge isolation models for hosting multiple customers on a shared platform. |
| [Saga Pattern](./saga-pattern.md) | Coordinates distributed workflows across services using local transactions paired with compensating actions. |

---

## Architecture as Code

Tools and frameworks for encoding architecture in machine-readable, version-controlled formats.

| Repo | Description |
|------|-------------|
| [Structurizr](https://github.com/structurizr) | Build multiple architecture diagrams from a single model using the C4 model. The canonical "diagrams as code" platform. |
| [C4InterFlow](https://github.com/SlavaVedernikov/C4InterFlow) | Architecture as Code framework — describe your architecture model once, generate many diagram and documentation outputs. |
| [swark](https://github.com/swark-io/swark) | Auto-generate architecture diagrams from code using LLMs (Mermaid output via GitHub Copilot / VS Code). |
| [HariSekhon/Diagrams-as-Code](https://github.com/HariSekhon/Diagrams-as-Code) | Cloud & DevOps architecture diagrams in Python, D2, and MermaidJS. |
| [terravision](https://github.com/patrickchugh/terravision) | Generate interactive HTML architecture diagrams from Terraform code. Supports AWS, GCP, and Azure. |
| [ai-sdlc](https://github.com/ai-sdlc-framework/ai-sdlc) | Declarative governance framework for AI-augmented software development lifecycles. |

**GitHub Topics to explore:**
- [github.com/topics/architecture-diagram](https://github.com/topics/architecture-diagram)
- [github.com/topics/diagrams-as-code](https://github.com/topics/diagrams-as-code)
- [github.com/topics/diagram-as-code](https://github.com/topics/diagram-as-code)

---

## Architecture Standards

Reference files, templates, and guidance for documenting software architecture consistently.

| Resource | Description |
|----------|-------------|
| [awesome-architecture-md](https://github.com/noahbald/awesome-architecture-md) | Curated list of exemplary `ARCHITECTURE.md` files from real open-source projects (Tauri, ESBuild, Redis, etc.). |
| [ARCHITECTURE.md (matklad)](https://matklad.github.io/2021/02/06/ARCHITECTURE.md.html) | Definitive blog post on what an `ARCHITECTURE.md` should contain — the canonical reference. |
| [adr/madr](https://github.com/adr/madr) | Markdown Architectural Decision Records (MADR) — a lean, standardised format for capturing decisions. |
| [joelparkerhenderson/architecture-decision-record](https://github.com/joelparkerhenderson/architecture-decision-record) | Comprehensive collection of ADR templates (Nygard, Y-Statement, MADR, and more). |
| [adr.github.io](https://adr.github.io/) | Home of the ADR community — templates, tools, and best practices. |
| [log4brains](https://github.com/thomvaill/log4brains) | ADR management and publication tool — stores ADRs next to source code in git. |
| [hojak/awesome-architecture](https://github.com/hojak/awesome-architecture) | Curated list of architecture resources, standards, and learning materials. |
| [Documenting Software Architecture in Code Repos (Medium)](https://medium.com/software-architecture-foundations/documenting-software-architecture-in-code-repository-74716412b0a2) | Practical guide on embedding architecture documentation inside a git repository. |

---

## Architecture Patterns

References and documentation for common software architecture patterns.

| Resource | Description |
|----------|-------------|
| [DovAmir/awesome-design-patterns](https://github.com/DovAmir/awesome-design-patterns) | Comprehensive curated list of software and architecture design patterns, including cloud, serverless, and multi-tenancy patterns. |
| [mehdihadeli/awesome-software-architecture](https://github.com/mehdihadeli/awesome-software-architecture) | Deep catalogue of articles, videos, and resources on architecture patterns — CQRS, Event Sourcing, DDD, microservices, and more. |
| [simskij/awesome-software-architecture](https://github.com/simskij/awesome-software-architecture) | Concise curated list covering CQRS, Event Sourcing, Feature Toggles, and architectural principles. |
| [jy-yi/Software-Architecture-Patterns](https://github.com/jy-yi/Software-Architecture-Patterns) | Focused reference on common patterns: Layered, Event-Driven, Microkernel, Microservices, Space-Based. |
| [Software Architecture Patterns Notes](https://github.com/ahmedhammad97/Software-Architecture-Patterns-Notes) | Reading notes following Mark Richards' *Software Architecture Patterns* O'Reilly report. |

**Patterns covered across these resources:**
- Layered / N-Tier
- Event-Driven Architecture
- Microservices
- CQRS & Event Sourcing
- Domain-Driven Design (DDD)
- Microkernel
- Space-Based Architecture
- Serverless
- Multi-Tenancy

---

## Agent Skills for the SDLC

Collections of Claude Code skills, subagents, and AI agent toolkits covering the full software development lifecycle.

| Resource | Description |
|----------|-------------|
| [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) | Claude Code skills and 1000+ agent skills from official dev teams (Anthropic, Vercel, Stripe, Cloudflare, and more). Compatible with Codex, Gemini CLI, and Cursor. |
| [hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) | Curated list of skills, hooks, slash-commands, agent orchestrators, and plugins for Claude Code. Includes the Superpowers bundle and Trail of Bits security skills. |
| [rohitg00/awesome-claude-code-toolkit](https://github.com/rohitg00/awesome-claude-code-toolkit) | Most comprehensive Claude Code toolkit — 135 agents, 35 skills, 42 commands, 176+ plugins, 20 hooks, 14 MCP configs, and more. |
| [VoltAgent/awesome-claude-code-subagents](https://github.com/VoltAgent/awesome-claude-code-subagents) | 100+ specialised Claude Code subagents for a wide range of development use cases. |
| [travisvn/awesome-claude-skills](https://github.com/travisvn/awesome-claude-skills) | Curated list of Claude Skills for customising AI workflows in Claude Code. |
| [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills) | 220+ Claude Code skills for Claude Code, Codex, Gemini CLI, Cursor, and 8 other coding agents. |
| [danielscholl/claude-sdlc](https://github.com/danielscholl/claude-sdlc) | SDLC tooling purpose-built for Claude Code — planning, review, testing, and delivery workflows. |
| [Piebald-AI/claude-code-system-prompts](https://github.com/Piebald-AI/claude-code-system-prompts) | All parts of Claude Code's system prompt, built-in tool descriptions, and sub-agent prompts — kept up to date per release. |
| [TheBushidoCollective/ai-dlc](https://github.com/TheBushidoCollective/ai-dlc) | AI-DLC 2026 methodology — iterative, AI-driven development with hat-based workflows. |
| [github/awesome-copilot](https://github.com/github/awesome-copilot/blob/main/docs/README.skills.md) | Official GitHub Copilot skills directory — useful cross-reference for agent skill patterns. |

### Further Reading

- [An AI-led SDLC — Microsoft Tech Community](https://techcommunity.microsoft.com/blog/appsonazureblog/an-ai-led-sdlc-building-an-end-to-end-agentic-software-development-lifecycle-wit/4491896) — Building an end-to-end agentic SDLC with Azure and GitHub.
- [AI Tools for Every SDLC Phase — MetaCTO](https://www.metacto.com/blogs/mapping-ai-tools-to-every-phase-of-your-sdlc) — Mapping specific AI tools to each phase of the SDLC.
- [Agentic SDLC in Practice — PwC](https://www.pwc.com/m1/en/publications/2026/docs/future-of-solutions-dev-and-delivery-in-the-rise-of-gen-ai.pdf) — The rise of autonomous software delivery.

---

## Curated Prompts

Repositories of curated AI prompts relevant to software architecture, technical design, and AI-assisted development workflows.

| Resource | Description |
| -------- | ----------- |
| [ai-architecture-prompts](https://github.com/Alexanderdunlop/ai-architecture-prompts) | Prompts designed to teach Claude/Cursor to architect replaceable, modular systems — based on Eskil Steenberg's architecture lecture. |
| [chatgpt-architecture-coach](https://github.com/mikaelvesavuori/chatgpt-architecture-coach) | Priming prompts for structured architectural discussions, design reviews, and technical trade-off analysis. |
| [awesome-ai-dev-prompts](https://github.com/piyushrajyadav/awesome-ai-dev-prompts) | 76 battle-tested system prompts encoding senior specialist knowledge across architecture, design reviews, and technical planning. |
| [awesome-claude-prompts](https://github.com/langgptai/awesome-claude-prompts) | Claude-specific prompt collection covering architecture planning, code review, and technical documentation generation. |
| [awesome-reviewers](https://github.com/baz-scm/awesome-reviewers) | 8,000+ specialised code review prompts distilled from real pull request comments — useful for architectural review and design validation. |
| [system-prompts-and-models-of-ai-tools](https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools) | Extracted system prompts from 25+ AI coding tools (Claude Code, Cursor, Devin, Replit, Windsurf) — a comparative reference across agent designs. |
| [awesome-system-prompts](https://github.com/EliFuzz/awesome-system-prompts) | System prompts and tool definitions from major AI coding agents — useful for understanding how different tools model development workflows. |

---

## Contributing

PRs welcome. Please follow the existing table format and include a brief description of what each resource covers and why it belongs here.
