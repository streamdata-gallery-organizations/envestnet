---
swagger: "2.0"
x-collection-name: Envestnet
x-complete: 0
info:
  title: Crunch Base Get Funding Rounds Relationships
  description: Get Funding Rounds Relationships
  termsOfService: https://data.crunchbase.com/v3/page/accessing-the-dataset
  contact:
    name: Crunchbase
    url: https://groups.google.com/forum/#!forum/crunchbase-api
    email: data@crunchbase.com
  version: v3
host: api.crunchbase.com
basePath: /v/3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /acquisitions/{uuid}:
    get:
      summary: Acquistions
      description: Pull from Acquisition
      operationId: acquistions
      x-api-path-slug: acquisitionsuuid-get
      parameters:
      - in: query
        name: user_key
        description: This user_key is used to validate each developers access to the
          API and ensure that any rate limits or quotas are respected
      - in: path
        name: uuid
        description: The UUID of the acquisition
      responses:
        200:
          description: OK
      tags:
      - Acquisitions
      - Uuid
  /acquisitions/{uuid}/{relationship_name}:
    get:
      summary: Get Acquisitions Relationships
      description: Get Acquisitions Relationships
      operationId: acquisitionsRelationships
      x-api-path-slug: acquisitionsuuidrelationship-name-get
      parameters:
      - in: query
        name: page
        description: The number of the page to retrieve
      - in: path
        name: relationship_name
        description: The name of the relationship connecting Items
      - in: query
        name: sort_order
        description: The sort order
      - in: path
        name: uuid
        description: 32-character uuid of the Acquisition
      responses:
        200:
          description: OK
      tags:
      - Acquisitions
      - Uuid
      - Relationship
      - Name
  /categories:
    get:
      summary: Get Categories
      description: Get Categories
      operationId: categories
      x-api-path-slug: categories-get
      parameters:
      - in: query
        name: page
        description: Page number of the results to retrieve
      - in: query
        name: sort_order
        description: The sort order
      responses:
        200:
          description: OK
      tags:
      - Categories
  /funding-rounds/{uuid}:
    get:
      summary: Funding Rounds
      description: Gets funding rounds by UUID
      operationId: fundingRounds
      x-api-path-slug: fundingroundsuuid-get
      parameters:
      - in: query
        name: user_key
        description: 'Possible values are: 7a582a92032069b4f775a15b1acbe256'
      - in: path
        name: uuid
        description: The UUID of the Funding Round
      responses:
        200:
          description: OK
      tags:
      - Funding
      - Rounds
      - Uuid
  /funding-rounds/{uuid}/{relationship_name}:
    get:
      summary: Get Funding Rounds Relationships
      description: Get Funding Rounds Relationships
      operationId: fundingRoundRelationships
      x-api-path-slug: fundingroundsuuidrelationship-name-get
      parameters:
      - in: query
        name: page
        description: The page number to retrieve
      - in: path
        name: relationship_name
        description: The name of the relationship connecting Items
      - in: query
        name: sort_order
        description: The sort order
      - in: path
        name: uuid
        description: The 32-character uuid of the FundingRound
      responses:
        200:
          description: OK
      tags:
      - Funding
      - Rounds
      - Uuid
      - Relationship
      - Name
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