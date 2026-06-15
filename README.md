# Letta (letta)

Letta (formerly MemGPT) is a stateful AI agents platform built around long-term memory, tool execution, and multi-agent coordination. The Letta REST API exposes 239 endpoints across 36 public resource categories — agents, memory blocks, archival memory, sources (RAG), custom tools (sandboxed/client-side/MCP), MCP servers, multi-agent groups, identities, runs, scheduled messages, and a streaming voice-mode endpoint. Open-source server (Apache-2.0, 22.9k+ stars) is available on GitHub; Letta Cloud is the managed offering; the Agent Development Environment (ADE) provides a web UI for inspecting context windows, memory blocks, and run history. Python and TypeScript SDKs ship alongside the REST API, and the open `.af` agent file format lets agents migrate between deployments.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/letta/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/letta/refs/heads/main/apis.yml)

## Tags

- AI
- Agents
- Stateful Agents
- Memory
- MemGPT
- Continual Learning
- MCP
- Multi-Agent
- RAG
- Open Source

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-22

## APIs

### Letta Cloud API

REST API for managing stateful agents, memory blocks (in-context + archival/RAG), custom tools (sandboxed Python, client-side, MCP-delegated), sources, multi-agent groups (supervisor/round-robin/dynamic/sleep-time), MCP server registrations, runs, identities, scheduled messages, and a beta voice-mode streaming endpoint. 239 paths under `/v1/`. Bearer token auth (`Authorization: Bearer $LETTA_API_KEY`).

- **Human URL:** [https://docs.letta.com/](https://docs.letta.com/)
- **Base URL:** `https://api.letta.com`

#### Tags

- Agents
- Memory
- Tools
- Streaming
- RAG
- MCP
- Multi-Agent

#### Properties

- [Documentation](https://docs.letta.com/)
- [Sign Up](https://app.letta.com/)
- [Pricing](https://docs.letta.com/guides/api/plans)
- [Git Hub](https://github.com/letta-ai/letta)
- [L L Ms Txt](https://docs.letta.com/llms-full.txt)
- [Changelog](https://www.letta.com/blog)
- [OpenAPI](openapi/letta-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/letta.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/letta.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Open A P I Y A M L](openapi/letta-openapi.yml)
- [Spectral Ruleset](rules/letta-rules.yml)
- [JSON Schema](json-schema/letta-agent-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/letta-block-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/letta-tool-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/letta-source-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/letta-run-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/letta-group-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/letta-identity-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/letta-message-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/letta-passage-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/letta-archive-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/letta-job-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/letta-llm-config-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/letta-embedding-config-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/letta-provider-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Letta Self-Hosted Server

Open-source Letta server (Apache-2.0) for self-hosted agent deployments. Same REST API surface as Letta Cloud, free to run; pay only for hosting and underlying LLM API usage. Default base URL is http://localhost:8283. Agents can be migrated between self-hosted and cloud via the open .af agent file format.

- **Human URL:** [https://github.com/letta-ai/letta](https://github.com/letta-ai/letta)
- **Base URL:** `http://localhost:8283`

#### Tags

- Open Source
- Self-Hosted
- Agents
- Docker

#### Properties

- [Git Hub](https://github.com/letta-ai/letta)
- [Documentation](https://docs.letta.com/)
- [License](https://github.com/letta-ai/letta/blob/main/LICENSE)
- [Docker](https://github.com/letta-ai/letta/blob/main/Dockerfile)
- [Agent File Format](https://github.com/letta-ai/agent-file)
- [OpenAPI](openapi/letta-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/letta.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/letta.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Letta Code

Letta's memory-first coding agent — a CLI plus a desktop app (and an action for GitHub repos). "The memory-first coding agent that remembers and learns." Builds on the Letta Code SDK and the broader Letta platform; offered with personal plans (chat.letta.com) separate from the API Plan.

- **Human URL:** [https://github.com/letta-ai/letta-code](https://github.com/letta-ai/letta-code)
- **Base URL:** `https://chat.letta.com`

#### Tags

- Coding Agent
- CLI
- Desktop

#### Properties

- [Git Hub](https://github.com/letta-ai/letta-code)
- [SDK](https://github.com/letta-ai/letta-code-sdk)
- [Git Hub Action](https://github.com/letta-ai/letta-code-action)
- [Demo](https://github.com/letta-ai/letta-oss-ui)
- [Skills](https://github.com/letta-ai/skills)
- [Postman Collection](collections/letta.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/letta.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/letta-ai)
- [Website](https://www.letta.com/)
- [Blog](https://www.letta.com/blog)
- [Documentation](https://docs.letta.com/)
- [L L Ms Txt](https://docs.letta.com/llms-full.txt)
- [Git Hub](https://github.com/letta-ai)
- [Git Hub Org](https://github.com/letta-ai)
- [Python S D K](https://github.com/letta-ai/letta-python)
- [Type Script S D K](https://github.com/letta-ai/letta-node)
- [Sign In](https://app.letta.com/)
- [Pricing](https://docs.letta.com/guides/api/plans)
- [Plans](plans/letta-plans-pricing.yml)
- [Rate Limits](rate-limits/letta-rate-limits.yml)
- [Fin Ops](finops/letta-finops.yml)
- [Spectral Ruleset](rules/letta-rules.yml)
- [J S O N L D Context](json-ld/letta-context.jsonld)
- [Vocabulary](vocabulary/letta-vocabulary.yml)
- [Agent File Format](https://github.com/letta-ai/agent-file)
- [L L Ms Txt](https://docs.letta.com/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
