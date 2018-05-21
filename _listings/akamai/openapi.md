---
swagger: "2.0"
x-collection-name: Akamai
x-complete: 1
info:
  title: Akamai API
  description: the-akamai-api-for-managing-your-akamai-service
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
    put:
      summary: Update a Cloudlets Origin Version
      description: Update a Cloudlets Origin Version
      operationId: cloudletsapiv2originsoriginidversionsversionvalidate
      x-api-path-slug: cloudletsapiv2originsoriginidversionsversion-put
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
  /cloudlets/api/v2/origins/currentActivations:
    get:
      summary: List Current Cloudlets Origin Activations
      description: List Current Cloudlets Origin Activations
      operationId: cloudletsapiv2originscurrentactivations
      x-api-path-slug: cloudletsapiv2originscurrentactivations-get
      responses:
        200:
          description: OK
      tags:
      - Cloudlets
      - Origins
      - Activations
  /cloudlets/api/v2/origins/{originId}/activations:
    get:
      summary: List Activations for a Cloudlets Origin
      description: List Activations for a Cloudlets Origin
      operationId: cloudletsapiv2originsoriginidactivations
      x-api-path-slug: cloudletsapiv2originsoriginidactivations-get
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
      - Activations
    post:
      summary: Activate a Cloudlets Origin Version
      description: Activate a Cloudlets Origin Version
      operationId: cloudletsapiv2originsoriginidactivations
      x-api-path-slug: cloudletsapiv2originsoriginidactivations-post
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
      - Activations
---