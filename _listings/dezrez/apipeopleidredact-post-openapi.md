---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: "Dezrez Redact a Person by PersonId\r\nFirst request is just logged as an
    event \r\nSecond request must be by a branch admin and actually redacts the person"
  version: 1.0.0
  description: "Redact a person by personid\r\nfirst request is just logged as an
    event \r\nsecond request must be by a branch admin and actually redacts the person."
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---