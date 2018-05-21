---
swagger: "2.0"
x-collection-name: Akamai
x-complete: 0
info:
  title: Akamai API Get a Cloudlets Origin Version
  description: Get a Cloudlets Origin Version
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cloudlets/api/v2/origins:
    get:
      summary: List Cloudlets Origins
      description: List Cloudlets Origins
      operationId: cloudletsapiv2originstype
      x-api-path-slug: cloudletsapiv2origins-get
      parameters:
      - in: query
        name: type
        description: Returns data for a specific type of origin as defined in Property
          Manager
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cloudlets
      - Origins
      - Type
  /cloudlets/api/v2/origins/{originId}:
    get:
      summary: Get a Cloudlets Origin
      description: Get a Cloudlets Origin
      operationId: cloudletsapiv2originsoriginid
      x-api-path-slug: cloudletsapiv2originsoriginid-get
      parameters:
      - in: query
        name: originId
        description: Unique identifier for the origin
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cloudlets
      - Origins
    put:
      summary: Update a Cloudlets Origin
      description: Update a Cloudlets Origin
      operationId: cloudletsapiv2originsoriginid
      x-api-path-slug: cloudletsapiv2originsoriginid-put
      parameters:
      - in: query
        name: originId
        description: Unique identifier for the origin
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cloudlets
      - Origins
  /cloudlets/api/v2/origins/{originId}/versions:
    get:
      summary: List Cloudlets Origin Versions
      description: List Cloudlets Origin Versions
      operationId: cloudletsapiv2originsoriginidversions
      x-api-path-slug: cloudletsapiv2originsoriginidversions-get
      parameters:
      - in: query
        name: originId
        description: Unique identifier for the origin
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cloudlets
      - Origins
      - Versions
    post:
      summary: Create a Cloudlets Origin Version
      description: Create a Cloudlets Origin Version
      operationId: cloudletsapiv2originsoriginidversions
      x-api-path-slug: cloudletsapiv2originsoriginidversions-post
      parameters:
      - in: query
        name: originId
        description: Unique identifier for the origin
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cloudlets
      - Origins
      - Versions
  /cloudlets/api/v2/origins/{originId}/versions/{version}:
    get:
      summary: Get a Cloudlets Origin Version
      description: Get a Cloudlets Origin Version
      operationId: cloudletsapiv2originsoriginidversionsversionvalidate
      x-api-path-slug: cloudletsapiv2originsoriginidversionsversion-get
      parameters:
      - in: query
        name: originId
        description: Unique identifier for the origin
        type: string
      - in: query
        name: validate
        description: For GET operations, verifies that the current settings for the
          selected originId and version are valid
        type: string
      - in: query
        name: version
        description: The origin version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cloudlets
      - Origins
      - Versions
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