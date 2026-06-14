# Superblocks GraphQL API

Superblocks provides a GraphQL integration plugin that enables users to call any external or internal GraphQL API from within Superblocks Applications, Workflows, and Scheduled Jobs. The integration acts as a configured client connection: you supply the remote GraphQL endpoint URL, choose an authentication method, and optionally add custom request headers. Once configured, any API step inside Superblocks can issue GraphQL queries and mutations against that datasource — with results piped into your application's UI or downstream workflow steps.

The GraphQL plugin is one of more than 50 built-in integrations in Superblocks. Its configuration schema is defined in the open-source agent repository (`superblocksteam/agent`) using Protocol Buffers and is consumed by the Superblocks on-prem agent worker. Key configuration fields are the remote `path` (the GraphQL endpoint URL), a list of HTTP `headers` (key/value pairs for auth tokens, content-type overrides, etc.), the query `body` (the raw GraphQL query or mutation string), optional GraphQL `variables`, and two behavioral flags: `verboseHttpOutput` (to include raw HTTP response metadata) and `failOnGraphqlErrors` (to surface GraphQL `errors` arrays as execution failures rather than soft errors).

Superblocks' own management API (`api.superblocks.com/v1`) is a REST API, not a GraphQL API. It provides CRUD operations for Applications and Workflow listing, authenticated via an API key (`X-API-Key` header) or Bearer JWT. There is no publicly documented GraphQL endpoint at `api.superblocks.com` or `app.superblocks.com/graphql`. The GraphQL SDL schema below documents the Superblocks platform domain model — the resource types, enumerations, and relationships — derived from the open-source Protocol Buffer definitions in the `superblocksteam/agent` repository, expressed in GraphQL SDL for catalog use.

**Endpoint:** Not applicable — Superblocks does not expose a public GraphQL endpoint. The REST management API base URL is `https://api.superblocks.com/v1`.

**Documentation:** https://docs.superblocks.com/integrations/integrations-library/graphql

**References:**
- Documentation: https://docs.superblocks.com/integrations/integrations-library/graphql
- GettingStarted: https://docs.superblocks.com/getting-started/core-concepts
- APIReference: https://docs.superblocks.com/api-reference/openapi.json
- SourceRepository: https://github.com/superblocksteam/agent/tree/main/types/proto/plugins/graphql/v1/plugin.proto
- CommonTypes: https://github.com/superblocksteam/agent/tree/main/types/proto/common/v1
- IntegrationTypes: https://github.com/superblocksteam/agent/tree/main/types/proto/integration/v1
