# Uniphore

Uniphore — "The Business AI Company" — is an enterprise AI vendor founded in 2008 and
headquartered in Palo Alto, California. Its flagship platform, the **Business AI Cloud
(BAIC)**, is a sovereign, composable and secure AI platform organised into a Data Layer,
Knowledge Layer, Model Layer and Agentic Layer, with products spanning Marketing AI
(CDP Agent), Sales AI, People AI and Customer Service AI.

- Website: https://www.uniphore.com/
- Docs: https://uniphore.github.io/baic-docs/ (BAIC Installation Guide)
- Support: https://www.uniphore.com/support/ · https://support.uniphore.com/
- Trust Center: https://trust.uniphore.com/
- GitHub: https://github.com/uniphore

## API surface

Uniphore **publishes no OpenAPI, AsyncAPI, GraphQL schema, MCP server or A2A agent
card** on any public host. The machine-readable contract hunt (2026-08-02) probed
`api.uniphore.com` (a live Kong gateway that answers `no Route matched with those
values` on every path), `www.uniphore.com`, `support.uniphore.com`,
`uniphore.github.io` and `uniphore.us.auth0.com` for `/openapi.json`, `/openapi.yaml`,
`/swagger.json`, `/v1/openapi.json`, `/api-docs`, `/docs`, `/redoc`, `/graphql`,
`/mcp` and both `/.well-known/agent-card.json` and `/.well-known/agent.json` — all
miss. There is no public Postman workspace.

What **is** public and captured here:

| Surface | Where |
|---|---|
| BAIC platform API (`/auth/m2m-token`, `POST /v1/question-answer/ask`, OpenAI-compatible `/openai/v1`) | https://uniphore.github.io/baic-docs/ |
| OIDC / RFC 8414 discovery for Uniphore's Auth0 tenant | `well-known/` |
| `llms.txt` (published by Uniphore, saved verbatim) | `llms/uniphore-llms.txt` |
| Trust Center certifications (SOC 2 Type 2, ISO 27001/27017/27018/27701, PCI DSS v4.0.1, HIPAA, GDPR, FIPS 140, CASA Tier 2, NIST CSF, EU AI Act) | `security/` |
| SLA — 99.5% monthly uptime, severity response targets, per-region maintenance windows, 6-month version support window | `lifecycle/` |
| First-party npm client/UI libraries + Chronos desktop releases | `packages/`, `changelog/` |

No published vulnerability disclosure programme, status page, public pricing page,
CLI, sandbox or roadmap was found.
