# Superblocks (superblocks)

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
