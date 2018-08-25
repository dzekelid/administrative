---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/people/{id}/redact:
    post:
      summary: "Redact a Person by PersonId\r\nFirst request is just logged as an
        event \r\nSecond request must be by a branch admin and actually redacts the
        person"
      description: "Redact a person by personid\r\nfirst request is just logged as
        an event \r\nsecond request must be by a branch admin and actually redacts
        the person."
      operationId: People_RedactByidBynote
      x-api-path-slug: apipeopleidredact-post
      parameters:
      - in: path
        name: id
      - in: query
        name: note
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Redact
      - Person
      - By
      - "PersonId\r\nFirst"
      - Request
      - Is
      - Just
      - Logged
      - As
      - Event
      - Second
      - Request
      - Must
      - Be
      - By
      - Branch
      - Admin
      - Actually
      - Redacts
      - Person
---