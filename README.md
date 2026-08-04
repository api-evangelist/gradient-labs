# Gradient Labs (gradient-labs)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
