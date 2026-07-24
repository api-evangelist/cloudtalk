---
name: Make an outbound CloudTalk call
description: Initiate an outbound call for an agent and follow up with call history and recording.
api: openapi/cloudtalk-openapi.json
operations:
- POST /calls/create.json
- GET /calls/index.json
- GET /calls/{callId}
- GET /calls/recording/{callId}.json
---

# Make an outbound CloudTalk call

Base URL: `https://my.cloudtalk.io/api`. HTTP Basic Auth (Access Key ID + Secret) on every request.

## Steps
1. **Place the call** — `POST /calls/create.json` with the agent and destination number. Watch for
   `409 Conflict` ("agent is already calling"), `403` (not permitted), `404` (agent/number unknown),
   `406` (invalid input).
2. **List call history** — `GET /calls/index.json` (Collections Envelope; filter by agent, number,
   date). Get a single record with `GET /calls/{callId}`.
3. **Recording** — `GET /calls/recording/{callId}.json` returns the recording (`audio/x-wav`);
   `410 Gone` means the recording has expired, `404` means none exists.

## Rules
- No idempotency key: a retried `POST /calls/create.json` may place a second call — confirm state first.
- HTTPS only; JSON only (except recording audio).
- Honor the 60 req/min-per-company rate limit and the `X-CloudTalkAPI-*` headers.
- For call analysis after the call, use the Conversation Intelligence skill.
