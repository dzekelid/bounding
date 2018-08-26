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
  /api/poi/search/box:
    post:
      summary: Search for POI's inside a bounding box
      description: Search for poi's inside a bounding box.
      operationId: Poi_GeoBoxSearchByquery
      x-api-path-slug: apipoisearchbox-post
      parameters:
      - in: body
        name: query
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - SearchPOIs
      - Inside
      - Bounding
      - Box
---