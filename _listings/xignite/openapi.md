swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetExchangeHours:
    get:
      summary: Get Exchange Hours
      description: Get exchange hours.
      operationId: GetExchangeHours
      x-api-path-slug: getexchangehours-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Exchange
      - Hours
  /GetExchangeHoursRange:
    get:
      summary: Get Exchange Hours Range
      description: Get exchange hours range.
      operationId: GetExchangeHoursRange
      x-api-path-slug: getexchangehoursrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Exchange
      - Hours
      - Range