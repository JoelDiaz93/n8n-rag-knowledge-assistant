# Security checklist

## Security

The workflows in this repository are sanitized portfolio versions. Credential bindings, pinned execution data, personal emails, account identifiers and embedded API keys were removed or replaced with placeholders.

Before importing:

1. Create credentials directly in n8n.
2. Rebind each credential-dependent node.
3. Replace `REPLACE_WITH_*` placeholders with your own resources.
4. Do not commit `.env` or exported credentials.
5. Validate webhook authentication, authorization and rate limits before exposing any endpoint publicly.

Additional production controls should include least-privilege credentials, request validation, idempotency, audit logging, secret rotation, retry/backoff policies and explicit authorization for state-changing operations.
