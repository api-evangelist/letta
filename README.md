# Letta

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Letta (formerly MemGPT) is a stateful AI agents platform built around long-term memory, tool execution, and multi-agent coordination. The Letta REST API exposes 239 endpoints across 36 public resource categories — agents, memory blocks, archival memory, sources (RAG), custom tools (sandboxed/client-side/MCP), MCP servers, multi-agent groups, identities, runs, scheduled messages, and a streaming voice-mode endpoint. Open-source server (Apache-2.0, 22.9k+ stars) is available on GitHub; Letta Cloud is the managed offering; the Agent Development Environment (ADE) provides a web UI for inspecting context windows, memory blocks, and run history. Python and TypeScript SDKs ship alongside the REST API, and the open `.af` agent file format lets agents migrate between deployments.

**Areas:** Artificial Intelligence · Agents · Stateful Agents · Memory · MemGPT · Continual Learning · MCP · Multi-Agent · RAG · Open Source · Real-Time

## Letta on APIs.io

Everything profiled for Letta is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/letta/](https://apis.io/providers/letta/)** — or go straight to one of the APIs or properties below.

### APIs (41)

- [Letta Code](https://apis.io/apis/letta/letta-code/) — Letta's memory-first coding agent — a CLI plus a desktop app (and an action for GitHub repos). "The memory-first coding agent that remembers and learns."…
- [Letta Admin API](https://apis.io/apis/letta/letta-admin-api/) — Administrative operations (org / billing / policy).
- [Letta Agents API](https://apis.io/apis/letta/letta-agents-api/) — Create, list, modify, export, and delete stateful agents with memory and tools.
- [Letta Archives API](https://apis.io/apis/letta/letta-archives-api/) — Manage archival memory archives and passages (RAG-style long-term store).
- [Letta Blocks API](https://apis.io/apis/letta/letta-blocks-api/) — Manage in-context memory blocks (core memory) shared across agents.
- [Letta Client-Side Access Tokens API](https://apis.io/apis/letta/letta-client-side-access-tokens-api/) — Mint short-lived client-side access tokens for browser/mobile use.
- [Letta Conversations API](https://apis.io/apis/letta/letta-conversations-api/) — Conversational session threads anchored to an agent.
- [Letta Device Storage API](https://apis.io/apis/letta/letta-device-storage-api/) — Per-device storage for the Letta Code SDK and ADE.
- [Letta Embeddings API](https://apis.io/apis/letta/letta-embeddings-api/) — List configured embedding models.
- [Letta Environments API](https://apis.io/apis/letta/letta-environments-api/) — Environment variables and configuration scoped to agents/tools.
- [Letta Feeds API](https://apis.io/apis/letta/letta-feeds-api/) — Subscribed feeds that drive agents.
- [Letta Folders API](https://apis.io/apis/letta/letta-folders-api/) — Organize agents and resources into folders.
- [Letta Groups API](https://apis.io/apis/letta/letta-groups-api/) — Coordinate multi-agent groups (supervisor/worker, round-robin, sleep-time).
- [Letta Health API](https://apis.io/apis/letta/letta-health-api/) — Service health/readiness endpoint.
- [Letta Identities API](https://apis.io/apis/letta/letta-identities-api/) — Map external user identities to agents and memory contexts.
- [Letta Internal Agents API](https://apis.io/apis/letta/letta-internal-agents-api/) — Internal Agents operations.
- [Letta Internal Blocks API](https://apis.io/apis/letta/letta-internal-blocks-api/) — Internal Blocks operations.
- [Letta Internal Runs API](https://apis.io/apis/letta/letta-internal-runs-api/) — Internal Runs operations.
- [Letta Internal Templates API](https://apis.io/apis/letta/letta-internal-templates-api/) — Internal Templates operations.
- [Letta Jobs API](https://apis.io/apis/letta/letta-jobs-api/) — Manage long-running background jobs (e.g., file ingestion).
- [Letta MCP Servers API](https://apis.io/apis/letta/letta-mcp-servers-api/) — Register external Model Context Protocol servers and expose their tools to agents.
- [Letta Memory Files API](https://apis.io/apis/letta/letta-memory-files-api/) — Memory-mapped file resources attached to agents.
- [Letta Messages API](https://apis.io/apis/letta/letta-messages-api/) — Send messages, list message history, search, and batch operations.
- [Letta Metadata API](https://apis.io/apis/letta/letta-metadata-api/) — Service/runtime metadata.
- [Letta Models API](https://apis.io/apis/letta/letta-models-api/) — List available chat and embedding models exposed by configured providers.
- [Letta Passages API](https://apis.io/apis/letta/letta-passages-api/) — Individual archival memory passages (chunked context).
- [Letta Pipelines API](https://apis.io/apis/letta/letta-pipelines-api/) — Composable agent pipelines.
- [Letta Projects API](https://apis.io/apis/letta/letta-projects-api/) — Project-level scoping for agents and resources.
- [Letta Providers API](https://apis.io/apis/letta/letta-providers-api/) — Configure LLM provider credentials (OpenAI, Anthropic, Azure, Ollama, etc.).
- [Letta Runs API](https://apis.io/apis/letta/letta-runs-api/) — Inspect and manage agent runs (executions of an agent in response to a message).
- [Letta Sandboxes API](https://apis.io/apis/letta/letta-sandboxes-api/) — Manage code-execution sandboxes used by sandbox tools.
- [Letta Scheduled Messages API](https://apis.io/apis/letta/letta-scheduled-messages-api/) — Schedule one-time or recurring messages to drive agents over time.
- [Letta Sources API](https://apis.io/apis/letta/letta-sources-api/) — Manage data sources (files, URLs) used to populate agent archival memory.
- [Letta Steps API](https://apis.io/apis/letta/letta-steps-api/) — Per-step traces of an agent run.
- [Letta Tag API](https://apis.io/apis/letta/letta-tag-api/) — Tag-based filtering metadata.
- [Letta Telemetry API](https://apis.io/apis/letta/letta-telemetry-api/) — Run-step traces and observability data.
- [Letta Templates API](https://apis.io/apis/letta/letta-templates-api/) — Reusable agent templates for instantiation.
- [Letta Tools API](https://apis.io/apis/letta/letta-tools-api/) — Register and execute custom tools (sandboxed Python, client-side, MCP).
- [Letta Voice API](https://apis.io/apis/letta/letta-voice-api/) — Voice (low-latency) chat completions endpoint for agents.
- [Letta LL Ms API](https://apis.io/apis/letta/letta-llms-api/) — List available LLM models and configurations.
- [Letta Chat Completions API](https://apis.io/apis/letta/letta-chat-completions-api/) — Chat operations.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Letta Agent Message Streaming (HTTP + SSE)](https://apis.io/asyncapis/letta/letta-asyncapi/)

#### Event channels (1)

Individual events and webhooks the provider emits.

- [/agents/{agent_id}/messages](https://apis.io/channels/letta/agents-agent-id-messages/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Letta Agentic Access](https://apis.io/agentic-access/letta/letta-agentic-access/)

#### JSON Schema (349)

The data models the API reads and writes.

- [AgentState](https://apis.io/schemas/letta/letta-agent/)
- [AgentEnvironmentVariable](https://apis.io/schemas/letta/letta-agentenvironmentvariable/)
- [AgentFileAttachment](https://apis.io/schemas/letta/letta-agentfileattachment/)
- [AgentFileSchema](https://apis.io/schemas/letta/letta-agentfileschema/)
- [AgentState](https://apis.io/schemas/letta/letta-agentstate/)
- [AgentType](https://apis.io/schemas/letta/letta-agenttype/)
- [Annotation](https://apis.io/schemas/letta/letta-annotation/)
- [AnnotationURLCitation](https://apis.io/schemas/letta/letta-annotationurlcitation/)
- [AnthropicModelSettings](https://apis.io/schemas/letta/letta-anthropicmodelsettings/)
- [AnthropicThinking](https://apis.io/schemas/letta/letta-anthropicthinking/)
- [ApprovalCreate](https://apis.io/schemas/letta/letta-approvalcreate/)
- [ApprovalRequestMessage](https://apis.io/schemas/letta/letta-approvalrequestmessage/)
- [ApprovalResponseMessage](https://apis.io/schemas/letta/letta-approvalresponsemessage/)
- [ApprovalReturn](https://apis.io/schemas/letta/letta-approvalreturn/)
- [ArchivalMemorySearchResponse](https://apis.io/schemas/letta/letta-archivalmemorysearchresponse/)
- [ArchivalMemorySearchResult](https://apis.io/schemas/letta/letta-archivalmemorysearchresult/)
- [Archive](https://apis.io/schemas/letta/letta-archive/)
- [ArchiveCreateRequest](https://apis.io/schemas/letta/letta-archivecreaterequest/)
- [ArchiveUpdateRequest](https://apis.io/schemas/letta/letta-archiveupdaterequest/)
- [AssistantMessage](https://apis.io/schemas/letta/letta-assistantmessage/)
- [AssistantMessageListResult](https://apis.io/schemas/letta/letta-assistantmessagelistresult/)
- [Audio](https://apis.io/schemas/letta/letta-audio/)
- [AuthRequest](https://apis.io/schemas/letta/letta-authrequest/)
- [AuthResponse](https://apis.io/schemas/letta/letta-authresponse/)
- [AzureModelSettings](https://apis.io/schemas/letta/letta-azuremodelsettings/)
- …and 324 more published on APIs.io

#### JSON Structure (15)

Data models expressed in JSON Structure.

- [Letta Agent Structure](https://apis.io/json-structure/letta/letta-agent-structure/)
- [Letta Archive Structure](https://apis.io/json-structure/letta/letta-archive-structure/)
- [Letta Block Structure](https://apis.io/json-structure/letta/letta-block-structure/)
- [Letta Embedding Config Structure](https://apis.io/json-structure/letta/letta-embedding-config-structure/)
- [Letta Group Structure](https://apis.io/json-structure/letta/letta-group-structure/)
- [Letta Identity Structure](https://apis.io/json-structure/letta/letta-identity-structure/)
- [Letta Job Structure](https://apis.io/json-structure/letta/letta-job-structure/)
- [Letta Llm Config Structure](https://apis.io/json-structure/letta/letta-llm-config-structure/)
- [Letta Message Structure](https://apis.io/json-structure/letta/letta-message-structure/)
- [Letta Passage Structure](https://apis.io/json-structure/letta/letta-passage-structure/)
- [Letta Provider Structure](https://apis.io/json-structure/letta/letta-provider-structure/)
- [Letta Run Structure](https://apis.io/json-structure/letta/letta-run-structure/)
- [Letta Source Structure](https://apis.io/json-structure/letta/letta-source-structure/)
- [Letta Structure](https://apis.io/json-structure/letta/letta-structure/)
- [Letta Tool Structure](https://apis.io/json-structure/letta/letta-tool-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Letta Context](https://apis.io/jsonld/letta/letta-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [letta-vocabulary](https://apis.io/vocabularies/letta/letta-vocabulary/)

#### Examples (29)

Example requests and responses.

- [Letta Agent Payload Example](https://apis.io/examples/letta/letta-agent-payload-example/)
- [Letta Block Payload Example](https://apis.io/examples/letta/letta-block-payload-example/)
- [Letta Create Agent Example](https://apis.io/examples/letta/letta-create-agent-example/)
- [Letta Create Identity Example](https://apis.io/examples/letta/letta-create-identity-example/)
- [Letta Create Memory Block Example](https://apis.io/examples/letta/letta-create-memory-block-example/)
- [Letta Create Multi Agent Group Example](https://apis.io/examples/letta/letta-create-multi-agent-group-example/)
- [Letta Create Source Example](https://apis.io/examples/letta/letta-create-source-example/)
- [Letta Create Tool Example](https://apis.io/examples/letta/letta-create-tool-example/)
- [Letta Create Voice Chat Completions Example](https://apis.io/examples/letta/letta-create-voice-chat-completions-example/)
- [Letta Group Payload Example](https://apis.io/examples/letta/letta-group-payload-example/)
- [Letta List Agents Example](https://apis.io/examples/letta/letta-list-agents-example/)
- [Letta List Chat Models Example](https://apis.io/examples/letta/letta-list-chat-models-example/)
- [Letta List Embedding Models Example](https://apis.io/examples/letta/letta-list-embedding-models-example/)
- [Letta List Mcp Servers Example](https://apis.io/examples/letta/letta-list-mcp-servers-example/)
- [Letta List Memory Blocks Example](https://apis.io/examples/letta/letta-list-memory-blocks-example/)
- [Letta List Runs Example](https://apis.io/examples/letta/letta-list-runs-example/)
- [Letta List Tools Example](https://apis.io/examples/letta/letta-list-tools-example/)
- [Letta Mcp Server Payload Example](https://apis.io/examples/letta/letta-mcp-server-payload-example/)
- [Letta Register Mcp Server Example](https://apis.io/examples/letta/letta-register-mcp-server-example/)
- [Letta Retrieve Agent Example](https://apis.io/examples/letta/letta-retrieve-agent-example/)
- [Letta Retrieve Run Example](https://apis.io/examples/letta/letta-retrieve-run-example/)
- [Letta Run Payload Example](https://apis.io/examples/letta/letta-run-payload-example/)
- [Letta Run Tool From Source Example](https://apis.io/examples/letta/letta-run-tool-from-source-example/)
- [Letta Send Agent Message Example](https://apis.io/examples/letta/letta-send-agent-message-example/)
- [Letta Source Payload Example](https://apis.io/examples/letta/letta-source-payload-example/)
- …and 4 more published on APIs.io

#### Collections (50)

Postman and Open Collection request collections.

- [Letta API](https://apis.io/collections/letta/open-letta/)
- [Letta Admin API](https://apis.io/collections/letta/open-letta-admin-api/)
- [Letta Agent Templates API](https://apis.io/collections/letta/open-letta-agent-templates-api/)
- [Letta Admin Agents API](https://apis.io/collections/letta/open-letta-agents-api/)
- [Letta API](https://apis.io/collections/letta/open-letta-ai/)
- [Letta Agent Templates Archival Memory API](https://apis.io/collections/letta/open-letta-archival-memory-api/)
- [Letta Admin Archives API](https://apis.io/collections/letta/open-letta-archives-api/)
- [Letta Admin Blocks API](https://apis.io/collections/letta/open-letta-blocks-api/)
- [Letta Admin Chat API](https://apis.io/collections/letta/open-letta-chat-api/)
- [Letta Agent Templates Chat Completions API](https://apis.io/collections/letta/open-letta-chat-completions-api/)
- [Letta Admin Client-Side Access Tokens API](https://apis.io/collections/letta/open-letta-client-side-access-tokens-api/)
- [Letta Admin Conversations API](https://apis.io/collections/letta/open-letta-conversations-api/)
- [Letta Admin Device Storage API](https://apis.io/collections/letta/open-letta-device-storage-api/)
- [Letta Admin Embeddings API](https://apis.io/collections/letta/open-letta-embeddings-api/)
- [Letta Admin Environments API](https://apis.io/collections/letta/open-letta-environments-api/)
- [Letta Admin Feeds API](https://apis.io/collections/letta/open-letta-feeds-api/)
- [Letta Admin Folders API](https://apis.io/collections/letta/open-letta-folders-api/)
- [Letta Admin Groups API](https://apis.io/collections/letta/open-letta-groups-api/)
- [Letta Admin Health API](https://apis.io/collections/letta/open-letta-health-api/)
- [Letta Admin Identities API](https://apis.io/collections/letta/open-letta-identities-api/)
- [Letta Admin Internal Agents API](https://apis.io/collections/letta/open-letta-internal-agents-api/)
- [Letta Admin Internal Blocks API](https://apis.io/collections/letta/open-letta-internal-blocks-api/)
- [Letta Admin Internal Runs API](https://apis.io/collections/letta/open-letta-internal-runs-api/)
- [Letta Admin Internal Templates API](https://apis.io/collections/letta/open-letta-internal-templates-api/)
- [Letta Admin Jobs API](https://apis.io/collections/letta/open-letta-jobs-api/)
- …and 25 more published on APIs.io

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Letta — asyncapi rules](https://apis.io/rules/letta/letta-asyncapi-spectral-rules/)
- [Letta — jsonschema rules](https://apis.io/rules/letta/letta-jsonschema-spectral-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Letta Authentication](https://apis.io/security/letta/letta-authentication/)
- [Letta Domain Security](https://apis.io/security/letta/letta-domain-security/)

#### Plans and pricing (2)

Published plans, tiers and prices.

- [Letta Plans Pricing](https://apis.io/plans/letta/letta-plans-pricing/)
- [Letta Price Estimates](https://apis.io/plans/letta/letta-price-estimates/)

#### Rate limits (1)

Published request limits.

- [Letta Rate Limits](https://apis.io/rate-limits/letta/letta-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Letta Finops](https://apis.io/finops/letta/letta-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.letta.com/)
- [Documentation](https://docs.letta.com/)
- [Pricing](https://docs.letta.com/guides/api/plans)
- [Blog](https://www.letta.com/blog)
- [GitHub](https://github.com/letta-ai)

## API Evangelist rating

**Kin Score 51.5** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 74.1 |
| Contract governance | 27.3 |
| Operational transparency | 18.4 |
| Developer ergonomics | 31.0 |
| Access clarity | 55.3 |

**Agent readiness 34.6** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | derived (partial credit) |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | yes |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | mostly (partial credit) |

**Regulatory alignment 15.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/letta/](https://apis.io/providers/letta/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Letta: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/letta/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
