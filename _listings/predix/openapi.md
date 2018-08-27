swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/collections/{collectionName}/spatial-query/bbox-interacts:
    get:
      summary: Return collection features in specified bounding box
      description: |-
        Returns all features in the specified collection that exist fully or
        partially within the specified bounding box. The bounding box is defined
        by two coordinates in the EPSG:4326 (WGS84) (for further details see
        http://epsg.io/4326):

        * left (longitude), bottom (latitude)

        * right (longitude), top (latitude)
      operationId: returns-all-features-in-the-specified-collection-that-exist-fully-orpartially-within-the-specified-b
      x-api-path-slug: v1collectionscollectionnamespatialquerybboxinteracts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Return
      - Collection
      - Features
      - In
      - Specified
      - Bounding
      - Box
  /v1/collections/{collectionName}/cluster:
    get:
      summary: Returns clustering data for collection features in specified bounding
        box
      description: |-
        Returns Clustering data for the specified collection that exist fully
         or partially within the specified bounding box. The bounding box is
         defined by two coordinates in the EPSG:4326 (WGS84)
         (for further details see http://epsg.io/4326):
         * left (longitude), bottom (latitude)
         * right (longitude), top (latitude)
      operationId: returns-clustering-data-for-the-specified-collection-that-exist-fully-or-partially-within-the-specif
      x-api-path-slug: v1collectionscollectionnamecluster-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Clustering
      - Datacollection
      - Features
      - In
      - Specified
      - Bounding
      - Box