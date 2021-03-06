---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Delete a shipping zone
  description: Delete a shipping zone with predefined identifier string
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shipping-zones:
    get:
      summary: Retrieve a list of shipping zones
      description: Retrieve a list of shipping zones
      operationId: shipping_zones.get
      x-api-path-slug: shippingzones-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Shipping
      - Zones
    post:
      summary: Create a Shipping Zone
      description: Create a Shipping Zone
      operationId: shipping_zones.post
      x-api-path-slug: shippingzones-post
      parameters:
      - in: body
        name: body
        description: Shipping Zone resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Zone
  /shipping-zones/{id}:
    delete:
      summary: Delete a shipping zone
      description: Delete a shipping zone with predefined identifier string
      operationId: shipping_zones.id.delete
      x-api-path-slug: shippingzonesid-delete
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Zone
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