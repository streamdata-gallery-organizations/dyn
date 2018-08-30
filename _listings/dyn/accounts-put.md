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
  accounts:
    put:
      summary: 'Updating an Email Sub-Account '
      description: 'Updating an Email Sub-Account '
      operationId: putAccounts
      parameters:
      - in: query
        name: address
        description: Address
      - in: query
        name: apikey
        description: Required
      - in: query
        name: bounceurl
        description: Bounce Postback URL
      - in: query
        name: city
        description: City
      - in: query
        name: companyname
        description: Required
      - in: query
        name: country
        description: Two-letter English abbreviation, based on the ISO 3166 standard
      - in: query
        name: generatenewapikey
        description: Used to create a new API key for an existing account (1 or 0)
      - in: query
        name: password
        description: Required
      - in: query
        name: phone
        description: Required
      - in: query
        name: spamurl
        description: Spam Postback URL
      - in: query
        name: state
        description: State
      - in: query
        name: timezone
        description: The timezone of the account, in [+/-]h
      - in: query
        name: tracklinks
        description: Toggle click tracking (1 or 0)
      - in: query
        name: trackopens
        description: Toggle open tracking (1 or 0)
      - in: query
        name: trackunsubscribes
        description: Toggle automatic list-unsubscribe support
      - in: query
        name: unsubscribeurl
        description: Unsubscribe postback URL
      - in: query
        name: username
        description: Required
      - in: query
        name: zipcode
        description: Zip
      responses:
        200:
          description: OK
      tags:
      - updating.email
      - accounts
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