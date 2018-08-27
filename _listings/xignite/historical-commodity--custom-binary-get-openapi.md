---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Futures Get Historical Commodity Chart Custom Binary
  description: Draw a custom historical chart for a future contract.
  version: 1.0.0
host: www.xignite.com
basePath: xFutures.json/XigniteFutures
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetHistoricalCommodityRange:
    get:
      summary: Get Historical Commodity Range
      description: Returns a range of historical quotes for a future contract.
      operationId: postGethistoricalcommodityrange
      x-api-path-slug: gethistoricalcommodityrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Commodity
      - Range
  /GetHistoricalCommodityMonthlyRange:
    get:
      summary: Get Historical Commodity Monthly Range
      description: Returns a range of historical quotes for a future contract.
      operationId: postGethistoricalcommoditymonthlyrange
      x-api-path-slug: gethistoricalcommoditymonthlyrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Commodity
      - Monthly
      - Range
  'Historical, Commodity, ':
    get:
      summary: Get Historical Commodity Chart
      description: Get a historical chart for a commodity.
      operationId: postGethistoricalcommoditychart
      x-api-path-slug: historical-commodity-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Commodity
      - Chart
  Historical, Commodity, , Binary:
    get:
      summary: Get Historical Commodity Chart Binary
      description: Get a historical chart for a commodity in binary format.
      operationId: postGethistoricalcommoditychartbinary
      x-api-path-slug: historical-commodity--binary-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Commodity
      - Chart
      - Binary
  Historical, Commodity, , Custom:
    get:
      summary: Get Historical Commodity Chart Custom
      description: Get a custom historical chart for a commodity in binary format.
      operationId: postGethistoricalcommoditychartcustom
      x-api-path-slug: historical-commodity--custom-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Commodity
      - Chart
      - Custom
  Historical, Commodity, , Custom, Binary:
    get:
      summary: Get Historical Commodity Chart Custom Binary
      description: Draw a custom historical chart for a future contract.
      operationId: postGethistoricalcommoditychartcustombinary
      x-api-path-slug: historical-commodity--custom-binary-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Commodity
      - Chart
      - Custom
      - Binary
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