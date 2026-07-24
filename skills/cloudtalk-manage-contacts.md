---
name: Manage CloudTalk contacts
description: Create, find, update, tag, and annotate contacts in CloudTalk.
api: openapi/cloudtalk-openapi.json
operations:
- GET /contacts/index.json
- GET /contacts/show/{contactId}.json
- PUT /contacts/add.json
- POST /contacts/edit/{contactId}.json
- DELETE /contacts/delete/{contactId}.json
- PUT /contacts/addTags/{contactId}.json
- PUT /notes/add/{contactId}.json
---

# Manage CloudTalk contacts

Base URL: `https://my.cloudtalk.io/api`. All paths use a `.json` suffix and return JSON only.

## Auth
Send HTTP Basic Auth on every request: username = API Access Key ID, password = Access Key Secret.
`curl -u ACCESS_KEY_ID:ACCESS_KEY_SECRET https://my.cloudtalk.io/api/contacts/index.json`

## Steps
1. **Find a contact** — `GET /contacts/index.json` with filters (results come in the Collections
   Envelope: `responseData.data[]` plus `itemsCount`/`pageCount`/`pageNumber`/`limit`; page with
   `page` and `limit`). Retrieve one with `GET /contacts/show/{contactId}.json`.
2. **Create** — `PUT /contacts/add.json` (PUT creates in this API). A `201` is success; `406`
   means invalid input.
3. **Update** — `POST /contacts/edit/{contactId}.json` (POST updates). `404` if the id is unknown.
4. **Tag** — `PUT /contacts/addTags/{contactId}.json`; remove with `DELETE /contacts/removeTags/{contactId}.json`.
5. **Annotate** — `PUT /notes/add/{contactId}.json` to attach a note.
6. **Delete** — `DELETE /contacts/delete/{contactId}.json`.

## Rules
- Method semantics are non-standard: **PUT creates, POST updates**, GET reads, DELETE deletes.
- Send `Accept: application/json`; omitting it can yield `404`/`406`.
- Respect the 60 req/min-per-company limit; on `429` back off using `X-CloudTalkAPI-ResetTime`.
- There is **no idempotency key** — do not blindly retry a create; check first with an index query.
- Errors return `{ "responseData": { "status", "message" } }` (see errors/cloudtalk-problem-types.yml).
