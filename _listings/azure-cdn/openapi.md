swagger: "2.0"
x-collection-name: Azure CDN
x-complete: 1
info:
  title: CdnManagementClient
  description: use-these-apis-to-manage-azure-cdn-resources-through-the-azure-resource-manager--you-must-make-sure-that-requests-made-to-these-resources-are-secure-
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Cdn/profiles/{profileName}/endpoints/{endpointName}/origins/{originName}
  : get:
      summary: Origins Get
      description: Gets an existing origin within an endpoint.
      operationId: Origins_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-cdnprofilesprofilenameendpointsendpointnameoriginsoriginname-get
      parameters:
      - in: path
        name: endpointName
        description: Name of the endpoint under the profile which is unique globally
      - in: query
        name: No Name
      - in: path
        name: originName
        description: Name of the origin which is unique within the endpoint
      - in: path
        name: profileName
        description: Name of the CDN profile which is unique within the resource group
      responses:
        200:
          description: OK
      tags:
      - CDN
      - Orgins
    patch:
      summary: Origins Update
      description: Updates an existing origin within an endpoint.
      operationId: Origins_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-cdnprofilesprofilenameendpointsendpointnameoriginsoriginname-patch
      parameters:
      - in: path
        name: endpointName
        description: Name of the endpoint under the profile which is unique globally
      - in: query
        name: No Name
      - in: path
        name: originName
        description: Name of the origin which is unique within the endpoint
      - in: body
        name: originUpdateProperties
        description: Origin properties
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileName
        description: Name of the CDN profile which is unique within the resource group
      responses:
        200:
          description: OK
      tags:
      - CDN
      - Orgins