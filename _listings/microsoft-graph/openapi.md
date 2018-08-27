swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /workbook/names(&lt;name&gt;)/range/BoundingRect:
    post:
      summary: Range Bounding Rect
      description: 'Range: BoundingRect Gets the smallest range object that encompasses
        the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15"
        is "B2:E16".'
      operationId: Range:BoundingRect
      x-api-path-slug: workbooknamesltnamegtrangeboundingrect-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Range
      - Bounding
      - Rect
  /workbook/worksheets(&lt;id|name&gt;)/range(&lt;address&gt;)/BoundingRect:
    post:
      summary: Range Bounding Rect
      description: 'Range: BoundingRect Gets the smallest range object that encompasses
        the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15"
        is "B2:E16".'
      operationId: Range:BoundingRect
      x-api-path-slug: workbookworksheetsltidnamegtrangeltaddressgtboundingrect-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Range
      - Bounding
      - Rect
  /workbook/tables(&lt;id|name&gt;)/columns(&lt;id|name&gt;)/range/BoundingRect:
    post:
      summary: Range Bounding Rect
      description: 'Range: BoundingRect Gets the smallest range object that encompasses
        the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15"
        is "B2:E16".'
      operationId: Range:BoundingRect
      x-api-path-slug: workbooktablesltidnamegtcolumnsltidnamegtrangeboundingrect-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Range
      - Bounding
      - Rect