# Gradient Labs (gradient-labs)

Gradient Labs builds "Otto", an AI customer support agent that autonomously handles complex, end-to-end support conversations for regulated and financial services businesses. The API lets you start and drive conversations, stream customer messages, hand off to human agents, execute business actions/tools, and manage the knowledge base the agent reasons over, with signed webhooks delivering the agent's outbound messages and events.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/apis.yml)

> Accuracy note: Gradient Labs' public API reference at https://api-docs.gradient-labs.ai/ is behind an access code. The endpoints, base URL (`https://api.gradient-labs.ai`), Bearer auth, and webhook event types cataloged here were reconstructed from the vendor's official open-source SDKs (primarily [gradientlabs-go](https://github.com/gradientlabs-ai/gradientlabs-go)). Request/response schemas are modeled and should be verified against the gated reference. See `review.yml` for what is confirmed vs. modeled.

## Tags

- AI
- Customer Support
- AI Agent
- Conversations
- Financial Services
- Regulated

## Timestamps

- **Created:** 2026-07-01
- **Modified:** 2026-07-01

## APIs

### Gradient Labs Conversations API

Start a conversation, assign it to the Gradient Labs AI agent, read its current state, and manage its lifecycle (finish, cancel, resume). The AI agent autonomously works the conversation and emits outbound messages and events via webhooks.

- **Human URL:** [https://api-docs.gradient-labs.ai/](https://api-docs.gradient-labs.ai/)
- **Base URL:** `https://api.gradient-labs.ai`

#### Tags

- Conversations
- AI Agent
- Support

#### Properties

- [Documentation](https://api-docs.gradient-labs.ai/)
- [OpenAPI](openapi/gradient-labs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gradient-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gradient-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Gradient Labs Messages API

Add inbound customer and human-agent messages (with optional email subject and attachments) to an existing conversation for the AI agent to process.

- **Human URL:** [https://api-docs.gradient-labs.ai/](https://api-docs.gradient-labs.ai/)
- **Base URL:** `https://api.gradient-labs.ai`

#### Tags

- Messages
- Conversations
- Attachments

#### Properties

- [Documentation](https://api-docs.gradient-labs.ai/)
- [OpenAPI](openapi/gradient-labs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gradient-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gradient-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Gradient Labs Hand-off & Assignment API

Assign or reassign a conversation between the AI agent and human participants, and capture the conversation.hand_off webhook the agent emits when it decides to escalate to a human, including reason code and routing target.

- **Human URL:** [https://api-docs.gradient-labs.ai/](https://api-docs.gradient-labs.ai/)
- **Base URL:** `https://api.gradient-labs.ai`

#### Tags

- Hand-off
- Assignment
- Human Agent

#### Properties

- [Documentation](https://api-docs.gradient-labs.ai/)
- [OpenAPI](openapi/gradient-labs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gradient-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gradient-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Gradient Labs Actions & Tools API

Define the business tools the AI agent can call and execute them. Tools can be run via the API or delivered to your endpoint through the action.execute webhook so the agent can take real actions in your systems.

- **Human URL:** [https://api-docs.gradient-labs.ai/](https://api-docs.gradient-labs.ai/)
- **Base URL:** `https://api.gradient-labs.ai`

#### Tags

- Actions
- Tools
- Function Calling

#### Properties

- [Documentation](https://api-docs.gradient-labs.ai/)
- [OpenAPI](openapi/gradient-labs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gradient-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gradient-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Gradient Labs Knowledge API

Upsert and delete knowledge-base articles (title, description, body, visibility, topic, status) that ground the AI agent's answers, organized by topic.

- **Human URL:** [https://api-docs.gradient-labs.ai/](https://api-docs.gradient-labs.ai/)
- **Base URL:** `https://api.gradient-labs.ai`

#### Tags

- Knowledge
- Articles
- Content

#### Properties

- [Documentation](https://api-docs.gradient-labs.ai/)
- [OpenAPI](openapi/gradient-labs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gradient-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gradient-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Gradient Labs Webhooks API

Signed, ordered webhook events the AI agent delivers to your endpoint — agent.message, conversation.hand_off, conversation.finished, action.execute, and resource.pull — each carrying an incrementing sequence_number so you can establish a total order of events per conversation.

- **Human URL:** [https://api-docs.gradient-labs.ai/](https://api-docs.gradient-labs.ai/)
- **Base URL:** `https://api.gradient-labs.ai`

#### Tags

- Webhooks
- Events
- Signing

#### Properties

- [Documentation](https://api-docs.gradient-labs.ai/)
- [OpenAPI](openapi/gradient-labs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/gradient-labs-ai)
- [Website](https://www.gradient-labs.ai)
- [Documentation](https://api-docs.gradient-labs.ai/)
- [GitHub Organization](https://github.com/gradientlabs-ai)
- [Plans](plans/gradient-labs-plans-pricing.yml)
- [Rate Limits](rate-limits/gradient-labs-rate-limits.yml)
- [Fin Ops](finops/gradient-labs-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
