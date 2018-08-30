---
swagger: "2.0"
info:
  title: Dyn
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  recipients/status:
    get:
      summary: Retrieve Recipient(s) Status
      description: Retrieve Recipient(s) Status
      operationId: getRecipientsStatus
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: emailaddress
        description: Required
      responses:
        200:
          description: OK
      tags:
      - retrieve
      - recipients
      - status
definitions: []
x-collection-name: Dyn
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