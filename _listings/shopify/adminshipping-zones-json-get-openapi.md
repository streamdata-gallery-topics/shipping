---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Show list of shipping zones
  description: Show list of shipping zones.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/orders/4554953422/refunds/calculate.json:
    post:
      summary: Calculate a refund for a line item and shipping
      description: Calculate a refund for a line item and shipping.
      operationId: postAdminOrders4554953422RefundsCalculate.json
      x-api-path-slug: adminorders4554953422refundscalculate-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Calculate
      - Refunda
      - Line
      - Item
      - Shipping
  /admin/shipping_zones.json:
    get:
      summary: Show list of shipping zones
      description: Show list of shipping zones.
      operationId: getAdminShippingZones.json
      x-api-path-slug: adminshipping-zones-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Show
      - List
      - Shipping
      - Zones
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