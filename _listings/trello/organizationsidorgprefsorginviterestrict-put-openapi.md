---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Put Organizations Preferences Orginviterestrict
  description: Put organizations preferences orginviterestrict.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/{idOrg}/prefs/orgInviteRestrict:
    delete:
      summary: Delete Organizations Preferences Orginviterestrict
      description: Delete organizations preferences orginviterestrict.
      operationId: deleteOrganizationsPrefsOrgInviteRestrictByIdOrg
      x-api-path-slug: organizationsidorgprefsorginviterestrict-delete
      parameters:
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      - in: query
        name: value
        description: An email address with optional expansion tokens
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Preferences
      - Orginviterestrict
    put:
      summary: Put Organizations Preferences Orginviterestrict
      description: Put organizations preferences orginviterestrict.
      operationId: updateOrganizationsPrefsOrgInviteRestrictByIdOrg
      x-api-path-slug: organizationsidorgprefsorginviterestrict-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Org Invite Restrict to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Preferences
      - Orginviterestrict
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