# RAG Knowledge Assistant

Document knowledge assistant demonstrating an in-memory RAG baseline and a persistent PostgreSQL/PGVector architecture with document ingestion and change detection.

> Portfolio-ready, sanitized n8n workflows. Credentials and personal/course-specific data are intentionally excluded.

## Workflows

- `rag-in-memory.json` — Sistema RAG estándar
- `rag-postgresql-pgvector.json` — Sistema RAG estándar PostgreSQL

## Architecture

The repository separates orchestration from credentials and external service configuration. n8n coordinates triggers, validation, integrations, AI/tool execution and persistence while external systems remain independently replaceable.

## Getting started

1. Run or connect to an n8n instance.
2. Import the JSON files from `workflows/`.
3. Create the required credentials inside n8n and bind them to the imported nodes.
4. Replace every `REPLACE_WITH_*` placeholder.
5. Execute with test data before activating schedules or public webhooks.

## Security

The workflows in this repository are sanitized portfolio versions. Credential bindings, pinned execution data, personal emails, account identifiers and embedded API keys were removed or replaced with placeholders.

Before importing:

1. Create credentials directly in n8n.
2. Rebind each credential-dependent node.
3. Replace `REPLACE_WITH_*` placeholders with your own resources.
4. Do not commit `.env` or exported credentials.
5. Validate webhook authentication, authorization and rate limits before exposing any endpoint publicly.

## Portfolio context

This repository refactors training workflows into a clean engineering showcase. It is intended to demonstrate orchestration, integrations, AI automation and production-minded patterns rather than publish third-party credentials or course-specific account data.

## License

MIT. Review the terms of every external API/service before production use.
