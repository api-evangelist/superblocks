# Superblocks (superblocks)

Superblocks is a programmable internal tools platform that enables engineering and IT teams to build, govern, and deploy enterprise-grade internal applications, workflows, and scheduled jobs on top of databases, REST APIs, GraphQL APIs, and 50+ SaaS integrations. The platform exposes a REST management API at `api.superblocks.com/v1` for managing applications and workflows programmatically. Superblocks supports three deployment models—fully managed cloud, hybrid, and Cloud-Prem (private VPC on AWS, GCP, or Azure)—and is SOC 2 Type II certified and HIPAA compliant.

APIs.json: https://raw.githubusercontent.com/api-evangelist/superblocks/refs/heads/main/apis.yml

Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=superblocks-api-evangelist&utm_content=repo

## Tags

- internal tools
- low-code
- no-code
- applications
- workflows
- scheduled jobs
- integrations
- enterprise
- AI
- databases
- REST API
- developer tools

## APIs

| Name | Type | Description |
|------|------|-------------|
| Superblocks Management API | REST | REST API for managing Superblocks applications and workflows. CRUD operations for applications, workflow listing. Base URL: `https://api.superblocks.com/v1`. Auth via API key (`X-API-Key` header) or Bearer JWT. OpenAPI spec at `https://docs.superblocks.com/api-reference/openapi.json`. |

## Plans / Rate Limits / FinOps

| Plan | Type | Price | Notes |
|------|------|-------|-------|
| Free | free | $0 | Up to 5 users; 30s Application API, 1min Workflow/Scheduled Job execution; 5 MB step output |
| Teams | paid | $100-$125/Builder/month | Up to 15 Builders; 14-day trial; 5min App API, 10min Workflow, 30min Scheduled Job; 20 MB step output; 100 AI Credits/Builder/month |
| Enterprise | enterprise | Custom | Unlimited Builders; SSO/SAML/OIDC; VPC deployment; source control; audit logs; dedicated support |

**Rate Limits (steps per second):**

| Scope | Free/Trial | Pro/Enterprise |
|-------|-----------|----------------|
| Per user | 500 | 5,000 |
| Per organization | 5,000 | 50,000 |
| Per single API | 500 | 5,000 |

- Throttled requests return HTTP 429
- Full rate limit details: [rate-limits/superblocks-rate-limits.yml](rate-limits/superblocks-rate-limits.yml)
- Full plans details: [plans/superblocks-plans-pricing.yml](plans/superblocks-plans-pricing.yml)
- FinOps details: [finops/superblocks-finops.yml](finops/superblocks-finops.yml)

## Timestamps

- created: 2026-06-12
- modified: 2026-06-12

## Common Properties

| Type | URL |
|------|-----|
| Website | https://www.superblocks.com/ |
| Documentation | https://docs.superblocks.com/ |
| GitHub Organization | https://github.com/superblocksteam |
| LinkedIn | https://www.linkedin.com/company/superblockshq |
| X (Twitter) | https://x.com/superblocks |
| Blog | https://www.superblocks.com/blog |
| Pricing | https://www.superblocks.com/pricing |
| Status Page | https://status.superblocks.com/ |
| OpenAPI Spec | https://docs.superblocks.com/api-reference/openapi.json |

## Maintainers

- Kin Lane / kin@apievangelist.com
