---
swagger: "2.0"
x-collection-name: Neblio
x-complete: 0
info:
  title: Neblio Builds a transaction that sends an NTP1 Token
  description: Builds an unsigned raw transaction that sends an NTP1 token on the
    Neblio blockchain.
  version: 1.0.0
host: ntp1node.nebl.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ntp1/issue:
    post:
      summary: Builds a transaction that issues a new NTP1 Token
      description: Builds an unsigned raw transaction that issues a new NTP1 token
        on the Neblio blockchain.
      operationId: issueToken
      x-api-path-slug: ntp1issue-post
      parameters:
      - in: body
        name: body
        description: Object representing the token to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Builds
      - Transaction
      - That
      - Issues
      - New
      - NTP1
      - Token
  /ntp1/sendtoken:
    post:
      summary: Builds a transaction that sends an NTP1 Token
      description: Builds an unsigned raw transaction that sends an NTP1 token on
        the Neblio blockchain.
      operationId: sendToken
      x-api-path-slug: ntp1sendtoken-post
      parameters:
      - in: body
        name: body
        description: Object representing the token to be sent
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Builds
      - Transaction
      - That
      - Sends
      - NTP1
      - Token
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