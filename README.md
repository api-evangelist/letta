# Letta (letta)

Letta (formerly **MemGPT**) is a stateful AI agents platform built around long-term memory, tool execution, and multi-agent coordination. The Letta REST API exposes 239 endpoints across 36 public resource categories — agents, memory blocks, archival memory, sources (RAG), custom tools, MCP servers, multi-agent groups, identities, runs, scheduled messages, and a streaming voice-mode endpoint. The open-source server (Apache-2.0, 22.9k+ stars) is available on GitHub; **Letta Cloud** is the managed offering; the **Agent Development Environment (ADE)** is the web UI.

**APIs.json:** [apis.yml](apis.yml) · [raw on GitHub](https://raw.githubusercontent.com/api-evangelist/letta/refs/heads/main/apis.yml)

## Type
- **x-type:** company

## Tags
AI, Agents, Stateful Agents, Memory, MemGPT, Continual Learning, MCP, Multi-Agent, RAG, Open Source

## APIs

### 1. Letta Cloud API — `https://api.letta.com`
Managed REST API. 239 paths under `/v1/`. Bearer-token auth (`Authorization: Bearer $LETTA_API_KEY`). Covers:

- **Agents** (56 ops) — create, list, modify, export, message, stream.
- **Tools** (21 ops) — sandboxed Python, client-side, MCP-delegated.
- **Identities** (18 ops) — per-user agent/memory scoping.
- **Sources** (14 ops) — file/URL ingestion for archival memory.
- **Groups** (11 ops) — multi-agent (supervisor / round-robin / dynamic / sleep-time).
- **MCP Servers** (10 ops) — register external MCP servers (streamable_http / sse / stdio).
- **Runs** (10 ops) — inspect agent executions, steps, usage.
- **Blocks** (9 ops) — labeled in-context memory blocks, shareable across agents.
- **Messages** (8 ops) — send, list, search, batches.
- **Providers** (8 ops) — LLM provider credentials and routing.
- Plus: archives, passages, jobs, scheduled messages, voice (beta), models, sandboxes, folders, projects, templates, conversations, environments, and more.

### 2. Letta Self-Hosted Server — `http://localhost:8283`
Open-source Letta server (Apache-2.0). Same REST API surface as Letta Cloud. Pay only for hosting and your own LLM API usage. Agents move between self-hosted and cloud via the open `.af` agent file format.

### 3. Letta Code
"The memory-first coding agent that remembers and learns." CLI + desktop app + GitHub action, built on the Letta Code SDK.

## Common Properties

- [Website](https://www.letta.com/) · [Blog](https://www.letta.com/blog) · [LinkedIn](https://www.linkedin.com/company/letta-ai)
- [Documentation](https://docs.letta.com/) · [llms-full.txt](https://docs.letta.com/llms-full.txt) · [Pricing](https://docs.letta.com/guides/api/plans)
- [GitHub org: letta-ai](https://github.com/letta-ai) · [Python SDK](https://github.com/letta-ai/letta-python) · [TypeScript SDK](https://github.com/letta-ai/letta-node)
- [Sign in: app.letta.com](https://app.letta.com/) · [Agent File (.af) format](https://github.com/letta-ai/agent-file)

## Artifacts

| Artifact | Count | Folder |
|---|---|---|
| OpenAPI specs | 2 (JSON + YAML) | [`openapi/`](openapi/) |
| Spectral rulesets | 1 | [`rules/`](rules/) |
| Naftiko capabilities (one per public tag) | 36 | [`capabilities/`](capabilities/) |
| JSON Schemas (per entity) | 14 | [`json-schema/`](json-schema/) |
| JSON Structures | 14 | [`json-structure/`](json-structure/) |
| JSON-LD context | 1 | [`json-ld/`](json-ld/) |
| Examples (operations + payloads) | 28 | [`examples/`](examples/) |
| Vocabulary | 1 | [`vocabulary/`](vocabulary/) |
| Plans (pricing) | 1 | [`plans/`](plans/) |
| Rate limits | 1 | [`rate-limits/`](rate-limits/) |
| FinOps | 1 | [`finops/`](finops/) |

### OpenAPI

- [`openapi/letta-openapi.json`](openapi/letta-openapi.json) — Letta API v1.0.0, 239 paths, 347 component schemas, 36 public tags, bearer-token auth. Mirrored from [`letta-ai/letta/fern/openapi.json`](https://github.com/letta-ai/letta/blob/main/fern/openapi.json) with summaries Title-Cased and acronyms (MCP, LLM, API, ID, SSE) normalized.
- [`openapi/letta-openapi.yml`](openapi/letta-openapi.yml) — YAML rendering of the same spec.

### Naftiko Capabilities

One self-contained Naftiko capability file per public OpenAPI tag — each declares both a REST exposer and an MCP exposer routed through its inline `consumes` block. All 36 files in [`capabilities/`](capabilities/):

`letta-agents`, `letta-blocks`, `letta-archives`, `letta-passages`, `letta-sources`, `letta-tools`, `letta-mcp-servers`, `letta-groups`, `letta-identities`, `letta-runs`, `letta-jobs`, `letta-messages`, `letta-conversations`, `letta-scheduled-messages`, `letta-voice`, `letta-models`, `letta-llms`, `letta-embeddings`, `letta-providers`, `letta-folders`, `letta-projects`, `letta-templates`, `letta-sandboxes`, `letta-memory-files`, `letta-device-storage`, `letta-feeds`, `letta-environments`, `letta-client-side-access-tokens`, `letta-pipelines`, `letta-health`, `letta-telemetry`, `letta-steps`, `letta-tag`, `letta-metadata`, `letta-chat`, `letta-admin`.

### JSON Schemas

Per-entity Draft 2020-12 schemas: `agent`, `block`, `tool`, `source`, `run`, `group`, `identity`, `message`, `passage`, `archive`, `job`, `llm-config`, `embedding-config`, `provider`.

## Pricing Snapshot
- **Self-Hosted:** free (you pay infra + LLM).
- **API Plan (Cloud):** $20/mo base + $0.10/active agent/mo + $0.00015/sec tool execution + LLM pass-through at provider cost.
- **Enterprise:** custom (RBAC, SAML/OIDC SSO, increased quotas).

See [`plans/letta-plans-pricing.yml`](plans/letta-plans-pricing.yml), [`rate-limits/letta-rate-limits.yml`](rate-limits/letta-rate-limits.yml), [`finops/letta-finops.yml`](finops/letta-finops.yml).

## GitHub Org Highlights (`letta-ai`)

| Repo | Stars | Lang | Purpose |
|---|---|---|---|
| [letta](https://github.com/letta-ai/letta) | 22.9k | Python | OSS server, the platform itself (Apache-2.0) |
| [claude-subconscious](https://github.com/letta-ai/claude-subconscious) | 2.7k | TypeScript | Letta-based memory subconscious for Claude Code |
| [letta-code](https://github.com/letta-ai/letta-code) | 2.5k | TypeScript | Memory-first coding agent |
| [agent-file](https://github.com/letta-ai/agent-file) | 1.1k | TypeScript | Open `.af` file format for stateful agents |
| [sleep-time-compute](https://github.com/letta-ai/sleep-time-compute) | 132 | Python | Companion material to the sleep-time compute paper |
| [skills](https://github.com/letta-ai/skills) | 105 | Python | Shared skills (Letta Code / Claude Code / Codex) |
| [letta-chatbot-example](https://github.com/letta-ai/letta-chatbot-example) | 99 | TypeScript | Reference chatbot built on Letta |
| [context-constitution](https://github.com/letta-ai/context-constitution) | 74 | — | Letta primitive for memory governance |
| [letta-oss-ui](https://github.com/letta-ai/letta-oss-ui) | 73 | TypeScript | Open-source demo UI on the Letta Code SDK |
| [letta-obsidian](https://github.com/letta-ai/letta-obsidian) | 72 | TypeScript | Obsidian plugin running a Letta agent on your vault |
| [letta-evals](https://github.com/letta-ai/letta-evals) | 71 | Python | Evaluation kit for stateful agents |
| [letta-code-sdk](https://github.com/letta-ai/letta-code-sdk) | 68 | TypeScript | Letta Code SDK |
| [letta-python](https://github.com/letta-ai/letta-python) | 52 | Python | Python SDK |
| [letta-node](https://github.com/letta-ai/letta-node) | 48 | TypeScript | TypeScript SDK |
| [learning-sdk](https://github.com/letta-ai/learning-sdk) | 45 | Python | Drop-in continual learning SDK |
| [n8n-nodes-letta](https://github.com/letta-ai/n8n-nodes-letta) | 18 | TypeScript | Official n8n node |
| [vercel-ai-sdk-provider](https://github.com/letta-ai/vercel-ai-sdk-provider) | 20 | TypeScript | Official Vercel AI SDK provider |
| [letta-voice](https://github.com/letta-ai/letta-voice) | 25 | Python | Low-latency voice chat with Letta agents |
| [deep-research](https://github.com/letta-ai/deep-research) | 27 | Python | Open-source deep-research agent on Letta |

## Notable

- **MemGPT lineage** — Letta is the production framework that grew out of the 2023 MemGPT paper on virtual-context-management for LLM agents.
- **Sleep-time agents** — background agents that share memory with primary agents and asynchronously consolidate/rewrite it (`enable_sleeptime: true`).
- **Multi-agent groups** — supervisor / round-robin / dynamic / sleep-time manager configs; agents can share memory blocks across the group.
- **MCP as a first-class consumer** — Letta registers external MCP servers (streamable_http, sse, stdio) and exposes their tools to agents alongside sandboxed Python and client-side tools.
- **Agent Development Environment (ADE)** — "bridges the gap between development and deployment, providing complete transparency, state control, rapid prototyping, and robust debugging."
- **Agent File (.af)** — open format for serializing a full agent (memory + tools + config) for export, versioning, and migration.

## Maintainers

**FN:** Kin Lane · **Email:** kin@apievangelist.com
