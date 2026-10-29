# CloudTalk

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

CloudTalk is an AI-powered cloud call center and business phone system (CCaaS) for sales and customer support teams, backed by Point Nine. Its public REST API (served at https://my.cloudtalk.io/api, published as OpenAPI 3.0.1 version 1.7) lets developers automate calls, contacts, agents, groups, phone numbers, campaigns, tags, SMS, blacklists and notes, and read Conversation Intelligence data — transcription, sentiment, topics, talk-listen ratio and smart notes — plus initiate VoiceAgent calls. Authentication is HTTPS-only HTTP Basic Auth using an API Access Key ID and Secret; responses are JSON, paginated with a Collections Envelope, and rate limited to 60 requests per minute per company. Events are delivered through Workflow Automation triggers (native and virtual webhooks) rather than the REST API.

**Areas:** Company · Communications · Voice · VoIP · Call Center · Contact Center · CCaaS · Telephony · SMS · Conversation Intelligence

## CloudTalk on APIs.io

Everything profiled for CloudTalk is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/cloudtalk/](https://apis.io/providers/cloudtalk/)** — or go straight to one of the APIs or properties below.

### APIs (13)

- [CloudTalk Agents API](https://apis.io/apis/cloudtalk/cloudtalk-agents-api/) — All data you can get about your agents.
- [CloudTalk Bulks API](https://apis.io/apis/cloudtalk/cloudtalk-bulks-api/) — Bulk actions.
- [CloudTalk Calls API](https://apis.io/apis/cloudtalk/cloudtalk-calls-api/) — All data you can get about your calls.
- [CloudTalk Campaigns API](https://apis.io/apis/cloudtalk/cloudtalk-campaigns-api/) — All data you can get about your campaigns.
- [CloudTalk Contacts API](https://apis.io/apis/cloudtalk/cloudtalk-contacts-api/) — All data you can get about your contacts.
- [CloudTalk Conversation Intelligence API](https://apis.io/apis/cloudtalk/cloudtalk-conversation-intelligence-api/) — Conversation Intelligence data about your calls.
- [CloudTalk CueCard API](https://apis.io/apis/cloudtalk/cloudtalk-cuecard-api/) — CueCards API ver. 1.0.2
- [CloudTalk Groups API](https://apis.io/apis/cloudtalk/cloudtalk-groups-api/) — The Groups API from CloudTalk — 3 operation(s) for groups.
- [CloudTalk Numbers API](https://apis.io/apis/cloudtalk/cloudtalk-numbers-api/) — All data you can get about your numbers.
- [CloudTalk Other API](https://apis.io/apis/cloudtalk/cloudtalk-other-api/) — All other helper endpoints.
- [CloudTalk Sms API](https://apis.io/apis/cloudtalk/cloudtalk-sms-api/) — Sms handling.
- [CloudTalk Tags API](https://apis.io/apis/cloudtalk/cloudtalk-tags-api/) — All data you can get about your tags.
- [CloudTalk VoiceAgent API](https://apis.io/apis/cloudtalk/cloudtalk-voiceagent-api/) — VoiceAgent API ver. 1.0.0

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Cloudtalk Webhooks](https://apis.io/asyncapis/cloudtalk/cloudtalk-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [cloudtalk](https://apis.io/servers/cloudtalk/cloudtalk/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Cloudtalk Agentic Access](https://apis.io/agentic-access/cloudtalk/cloudtalk-agentic-access/)

#### Collections (13)

Postman and Open Collection request collections.

- [CloudTalk Agents API](https://apis.io/collections/cloudtalk/open-cloudtalk-agents-api/)
- [CloudTalk Agents Bulks API](https://apis.io/collections/cloudtalk/open-cloudtalk-bulks-api/)
- [CloudTalk Agents Calls API](https://apis.io/collections/cloudtalk/open-cloudtalk-calls-api/)
- [CloudTalk Agents Campaigns API](https://apis.io/collections/cloudtalk/open-cloudtalk-campaigns-api/)
- [CloudTalk Agents Contacts API](https://apis.io/collections/cloudtalk/open-cloudtalk-contacts-api/)
- [CloudTalk Agents Conversation Intelligence API](https://apis.io/collections/cloudtalk/open-cloudtalk-conversation-intelligence-api/)
- [CloudTalk Agents CueCard API](https://apis.io/collections/cloudtalk/open-cloudtalk-cuecard-api/)
- [CloudTalk Agents Groups API](https://apis.io/collections/cloudtalk/open-cloudtalk-groups-api/)
- [CloudTalk Agents Numbers API](https://apis.io/collections/cloudtalk/open-cloudtalk-numbers-api/)
- [CloudTalk Agents Other API](https://apis.io/collections/cloudtalk/open-cloudtalk-other-api/)
- [CloudTalk Agents Sms API](https://apis.io/collections/cloudtalk/open-cloudtalk-sms-api/)
- [CloudTalk Agents Tags API](https://apis.io/collections/cloudtalk/open-cloudtalk-tags-api/)
- [CloudTalk Agents VoiceAgent API](https://apis.io/collections/cloudtalk/open-cloudtalk-voiceagent-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Cloudtalk Openapi Overlay](https://apis.io/overlays/cloudtalk/cloudtalk-openapi-overlay/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Cloudtalk Authentication](https://apis.io/security/cloudtalk/cloudtalk-authentication/)
- [Cloudtalk Domain Security](https://apis.io/security/cloudtalk/cloudtalk-domain-security/)
- [Cloudtalk Trust Center](https://apis.io/security/cloudtalk/cloudtalk-trust-center/)
- [Cloudtalk Vulnerability Disclosure](https://apis.io/security/cloudtalk/cloudtalk-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Cloudtalk Plans Pricing](https://apis.io/plans/cloudtalk/cloudtalk-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Cloudtalk Rate Limits](https://apis.io/rate-limits/cloudtalk/cloudtalk-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.cloudtalk.io)
- [Documentation](https://developers.cloudtalk.io/)
- [Getting started](https://help.cloudtalk.io/en/collections/441737-getting-started-with-cloudtalk)
- [API reference](https://developers.cloudtalk.io/)
- [Pricing](https://www.cloudtalk.io/pricing/)
- [Sign up](https://www.cloudtalk.io/signup/)
- [Support](https://help.cloudtalk.io/en/)
- [Blog](https://www.cloudtalk.io/blog/)
- [Security](https://trust.cloudtalk.io/)
- [Compliance](https://trust.cloudtalk.io/)
- [Terms of service](https://www.cloudtalk.io/terms-and-conditions/)
- [Privacy policy](https://www.cloudtalk.io/privacy-notice/)
- [GitHub](https://github.com/CloudTalk-io)
- [Status](https://status.cloudtalk.io/)

## API Evangelist rating

**Kin Score 58.2** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 60.9 |
| Contract governance | 4.5 |
| Operational transparency | 68.4 |
| Developer ergonomics | 32.7 |
| Access clarity | 84.2 |

**Agent readiness 46.1** — agent-native

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | verified |
| Error Semantics | verified |
| OpenAPI Examples | verified |
| Rate Limit Signal | verified |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | distinct |

**Regulatory alignment 25.8** — Telecommunications

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/cloudtalk/](https://apis.io/providers/cloudtalk/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for CloudTalk: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/cloudtalk/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
