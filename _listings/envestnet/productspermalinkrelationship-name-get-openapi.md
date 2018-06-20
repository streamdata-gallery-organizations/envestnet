---
swagger: "2.0"
x-collection-name: Envestnet
x-complete: 0
info:
  title: Crunch Base Get Product Relationships
  description: Get Product Relationships
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
  /funds/:uuid/{relationship_name}:
    get:
      summary: Get Fund Relationships
      description: Get Fund Relationships
      operationId: fundRelationships
      x-api-path-slug: fundsuuidrelationship-name-get
      parameters:
      - in: query
        name: page
        description: The number of the page to retrieve
      - in: path
        name: relationship_name
        description: The name of the connection between the Fund and related Items
      - in: query
        name: sort_order
        description: The sort order
      - in: path
        name: uuid
        description: The 32-character identifier of the Fund
      responses:
        200:
          description: OK
      tags:
      - Funds
      - :uuid
      - Relationship
      - Name
  /funds/{uuid}:
    get:
      summary: Get Funds
      description: Get Funds
      operationId: funds
      x-api-path-slug: fundsuuid-get
      parameters:
      - in: path
        name: uuid
        description: The UUID of the Fund Raise
      responses:
        200:
          description: OK
      tags:
      - Funds
      - Uuid
  /ipos/{uuid}:
    get:
      summary: Get IPO
      description: Get IPO Using UUID
      operationId: ipo
      x-api-path-slug: iposuuid-get
      parameters:
      - in: query
        name: user_key
        description: 'Possible values are: 7a582a92032069b4f775a15b1acbe256'
      - in: path
        name: uuid
        description: The UUID of the IPO
      responses:
        200:
          description: OK
      tags:
      - Ipos
      - Uuid
  /ipos/{uuid}/{relationship_name}:
    get:
      summary: Get IPO Relationships
      description: Get IPO Relationships
      operationId: ipoRelationships
      x-api-path-slug: iposuuidrelationship-name-get
      parameters:
      - in: query
        name: order
        description: The sort order
      - in: path
        name: relationship_name
        description: The name of the relationship connecting Items
      - in: query
        name: The page number to retrieve
        description: The page number to retrieve
      - in: path
        name: uuid
        description: The 32-character identifier of the Ipo
      responses:
        200:
          description: OK
      tags:
      - Ipos
      - Uuid
      - Relationship
      - Name
  /locations:
    get:
      summary: Get Locations
      description: Get Locations
      operationId: locations
      x-api-path-slug: locations-get
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
      - Locations
  /organizations:
    get:
      summary: Organizations
      description: Get Organizations
      operationId: organizations
      x-api-path-slug: organizations-get
      parameters:
      - in: query
        name: categories
        description: Filter by categories (comma separated, ANDd together) e
      - in: query
        name: category_uuids
        description: Filter by one or more Categories
      - in: query
        name: domain_name
        description: Text search of an Organizations domain_name (e
      - in: query
        name: locations
        description: Filter by location names (comma separated, ANDd together) e
      - in: query
        name: name
        description: Full text search limited to name and aliases
      - in: query
        name: organization_types
        description: Filter by one or more types
      - in: query
        name: page
        description: Page number of the results to retrieve
      - in: query
        name: query
        description: Full text search of an Organizations name, aliases (i
      - in: query
        name: sort_order
        description: The sort order of the collection
      - in: query
        name: updated_since
        description: Timestamp When provided, restricts the result set to Organizations
          where updated_at >= the passed value
      - in: query
        name: user_key
        description: 'Possible values are: 7a582a92032069b4f775a15b1acbe256'
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /organizations/{permalink}:
    get:
      summary: Get Organizations
      description: Get Organization Using Permalink
      operationId: organizations
      x-api-path-slug: organizationspermalink-get
      parameters:
      - in: path
        name: permalink
        description: The permalink of the organization
      - in: query
        name: user_key
        description: 'Possible values are: 7a582a92032069b4f775a15b1acbe256'
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Permalink
  /organizations/{permalink}/{relationship_name}:
    get:
      summary: Get Organization Relationships
      description: Get Organizations Relationships Using Permlink
      operationId: organizationRelationships
      x-api-path-slug: organizationspermalinkrelationship-name-get
      parameters:
      - in: query
        name: page
        description: Page number to retrieve
      - in: path
        name: permalink
        description: The permalink of the organization
      - in: path
        name: relationship_name
        description: The name of the rleationship to attached items
      - in: query
        name: sort_order
        description: The sort order
      - in: query
        name: user_key
        description: 'Possible values are: 7a582a92032069b4f775a15b1acbe256'
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Permalink
      - Relationship
      - Name
  /people:
    get:
      summary: Get People
      description: Get People
      operationId: people
      x-api-path-slug: people-get
      parameters:
      - in: query
        name: locations
        description: Filter by location names (comma separated, ANDd together) e
      - in: query
        name: name
        description: A full-text query of name only
      - in: query
        name: page
        description: the 1-indexed page number to retrieve
      - in: query
        name: query
        description: A full-text query of name, title, and company
      - in: query
        name: socials
        description: Filter by social media identity (comma separated, ANDd together)
          e
      - in: query
        name: sort_order
        description: The sort order
      - in: query
        name: types
        description: Filter by type (currently, either this is empty, or is simply
          investor)
      - in: query
        name: updated_since
        description: When provided, restricts the result set to People where updated_at
          >= the passed value
      responses:
        200:
          description: OK
      tags:
      - People
  /people/{permalink}:
    get:
      summary: Get People
      description: Get People Using Permalink
      operationId: people
      x-api-path-slug: peoplepermalink-get
      parameters:
      - in: path
        name: permalink
        description: The permalink of the organization
      - in: query
        name: user_key
        description: 'Possible values are: 7a582a92032069b4f775a15b1acbe256'
      responses:
        200:
          description: OK
      tags:
      - People
      - Permalink
  /people/{permalink}/{relationship_name}:
    get:
      summary: Get People Relationships
      description: Get People Relationships
      operationId: peopleRelationships
      x-api-path-slug: peoplepermalinkrelationship-name-get
      parameters:
      - in: query
        name: page
        description: The page number to retrieve
      - in: path
        name: permalink
        description: The permalink of the Person
      - in: path
        name: relationship_name
        description: The name of the relationship to connected Items
      - in: query
        name: sort_order
        description: The sort order
      responses:
        200:
          description: OK
      tags:
      - People
      - Permalink
      - Relationship
      - Name
  /products:
    get:
      summary: Get Products
      description: Get Products
      operationId: products
      x-api-path-slug: products-get
      parameters:
      - in: query
        name: page
        description: the 1-indexed page number to retrieve
      - in: query
        name: sort_order
        description: The sort order for the collection
      - in: query
        name: updated_since
        description: When provided, restricts the result set to Products where updated_at
          >= the passed value
      responses:
        200:
          description: OK
      tags:
      - Products
  /products/{permalink}:
    get:
      summary: Get Products
      description: Get Products Using Permalink
      operationId: products
      x-api-path-slug: productspermalink-get
      parameters:
      - in: path
        name: permalink
        description: The permalink of the organization
      - in: query
        name: user_key
        description: 'Possible values are: 7a582a92032069b4f775a15b1acbe256'
      responses:
        200:
          description: OK
      tags:
      - Products
      - Permalink
  /products/{permalink}/{relationship_name}:
    get:
      summary: Get Product Relationships
      description: Get Product Relationships
      operationId: productRelationships
      x-api-path-slug: productspermalinkrelationship-name-get
      parameters:
      - in: query
        name: page
        description: The page number to retrieve
      - in: path
        name: permalink
        description: The permalink of the Product
      - in: path
        name: relationship_name
        description: The name of the relationship connecting Items
      - in: query
        name: sort_order
        description: The sort order
      responses:
        200:
          description: OK
      tags:
      - Products
      - Permalink
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