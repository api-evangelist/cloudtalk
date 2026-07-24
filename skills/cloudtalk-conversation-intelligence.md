---
name: Get CloudTalk Conversation Intelligence for a call
description: Pull transcription, sentiment, topics, talk-listen ratio, and smart notes for a call.
api: openapi/cloudtalk-openapi.json
operations:
- GET /ai/calls/{callId}/transcription
- GET /ai/calls/{callId}/summary
- GET /ai/calls/{callId}/overall-sentiment
- GET /ai/calls/{callId}/talk-listen-ratio
- GET /ai/calls/{callId}/topics
- GET /ai/calls/{callId}/smart-notes
- GET /ai/calls/{callId}/details-link
---

# Get CloudTalk Conversation Intelligence for a call

Base URL: `https://my.cloudtalk.io/api`. HTTP Basic Auth (Access Key ID + Secret) on every request.

## Steps
Given a `callId` (from `GET /calls/index.json`), fetch any of:
1. `GET /ai/calls/{callId}/transcription` — full transcription.
2. `GET /ai/calls/{callId}/summary` — call summary.
3. `GET /ai/calls/{callId}/overall-sentiment` — sentiment score.
4. `GET /ai/calls/{callId}/talk-listen-ratio` — agent vs. caller talk ratio.
5. `GET /ai/calls/{callId}/topics` — detected topics with spans.
6. `GET /ai/calls/{callId}/smart-notes` — extracted notes / important dates.
7. `GET /ai/calls/{callId}/details-link` — deep link to the call details UI.

## Rules
- **Conversation Intelligence endpoints do NOT use the response envelopes** — the JSON body is the
  resource itself, not wrapped in `responseData`.
- Common errors: `400` (bad request), `401` (auth), `404` (no CI data for that call), `500`.
- These operations are read-only; Conversation Intelligence must be enabled on the account/plan.
- Honor the 60 req/min-per-company rate limit.
