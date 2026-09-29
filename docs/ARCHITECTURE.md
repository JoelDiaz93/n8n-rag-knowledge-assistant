# RAG Knowledge Assistant — Architecture

## Purpose

Document knowledge assistant demonstrating an in-memory RAG baseline and a persistent PostgreSQL/PGVector architecture with document ingestion and change detection.

## Design principles

- Keep n8n focused on orchestration.
- Isolate external integrations behind explicit nodes/tools.
- Keep credentials outside exported workflows.
- Make mutations explicit and auditable.
- Prefer deterministic validation for authorization and business rules.
- Add retries, idempotency and observability before production use.
