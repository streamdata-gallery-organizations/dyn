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
  suppressions/count:
    get:
      summary: Retrieve Suppression Count
      description: Retrieving the count of Email addresses on the suppression list
      operationId: getSuppressionsCount
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: enddate
        description: End date/time range in full, ISO 8601 format
      - in: query
        name: startdate
        description: Start date/time range in full, ISO 8601 format
      responses:
        200:
          description: OK
      tags:
      - retrieve
      - suppression
      - count
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