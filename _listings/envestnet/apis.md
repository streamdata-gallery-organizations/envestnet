---
name: Envestnet
x-slug: envestnet
description: Build and transform financial apps and services with access to financial
  data through our APIs and digital solutions for banks, developers, and innovators.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
x-kinRank: "8"
x-alexaRank: "84912"
tags: Envestnet
created: "2018-06-19"
modified: "2018-06-19"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/apis.md
specificationVersion: "0.14"
apis:
- name: Crunch Base Acquistions
  x-api-slug: crunch-base
  description: Pull from Acquisition
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//acquisitions/{uuid}
  tags: Acquisitions,Uuid
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/acquisitionsuuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/acquisitionsuuid-get-openapi.md
- name: Crunch Base Get Acquisitions Relationships
  x-api-slug: crunch-base
  description: Get Acquisitions Relationships
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//acquisitions/{uuid}/{relationship_name}
  tags: Acquisitions,Uuid,Relationship,Name
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/acquisitionsuuidrelationship-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/acquisitionsuuidrelationship-name-get-openapi.md
- name: Crunch Base Get Categories
  x-api-slug: crunch-base
  description: Get Categories
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//categories
  tags: Categories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/categories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/categories-get-openapi.md
- name: Crunch Base Funding Rounds
  x-api-slug: crunch-base
  description: Gets funding rounds by UUID
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//funding-rounds/{uuid}
  tags: Funding,Rounds,Uuid
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/fundingroundsuuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/fundingroundsuuid-get-openapi.md
- name: Crunch Base Get Funding Rounds Relationships
  x-api-slug: crunch-base
  description: Get Funding Rounds Relationships
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//funding-rounds/{uuid}/{relationship_name}
  tags: Funding,Rounds,Uuid,Relationship,Name
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/fundingroundsuuidrelationship-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/fundingroundsuuidrelationship-name-get-openapi.md
- name: Crunch Base Get Fund Relationships
  x-api-slug: crunch-base
  description: Get Fund Relationships
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//funds/:uuid/{relationship_name}
  tags: Funds,:uuid,Relationship,Name
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/fundsuuidrelationship-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/fundsuuidrelationship-name-get-openapi.md
- name: Crunch Base Get Funds
  x-api-slug: crunch-base
  description: Get Funds
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//funds/{uuid}
  tags: Funds,Uuid
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/fundsuuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/fundsuuid-get-openapi.md
- name: Crunch Base Get IPO
  x-api-slug: crunch-base
  description: Get IPO Using UUID
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//ipos/{uuid}
  tags: Ipos,Uuid
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/iposuuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/iposuuid-get-openapi.md
- name: Crunch Base Get IPO Relationships
  x-api-slug: crunch-base
  description: Get IPO Relationships
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//ipos/{uuid}/{relationship_name}
  tags: Ipos,Uuid,Relationship,Name
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/iposuuidrelationship-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/iposuuidrelationship-name-get-openapi.md
- name: Crunch Base Get Locations
  x-api-slug: crunch-base
  description: Get Locations
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//locations
  tags: Locations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/locations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/locations-get-openapi.md
- name: Crunch Base Organizations
  x-api-slug: crunch-base
  description: Get Organizations
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//organizations
  tags: Organizations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/organizations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/organizations-get-openapi.md
- name: Crunch Base Get Organizations
  x-api-slug: crunch-base
  description: Get Organization Using Permalink
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//organizations/{permalink}
  tags: Organizations,Permalink
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/organizationspermalink-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/organizationspermalink-get-openapi.md
- name: Crunch Base Get Organization Relationships
  x-api-slug: crunch-base
  description: Get Organizations Relationships Using Permlink
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//organizations/{permalink}/{relationship_name}
  tags: Organizations,Permalink,Relationship,Name
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/organizationspermalinkrelationship-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/organizationspermalinkrelationship-name-get-openapi.md
- name: Crunch Base Get People
  x-api-slug: crunch-base
  description: Get People
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//people
  tags: People
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/people-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/people-get-openapi.md
- name: Crunch Base Get People
  x-api-slug: crunch-base
  description: Get People Using Permalink
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//people/{permalink}
  tags: People,Permalink
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/peoplepermalink-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/peoplepermalink-get-openapi.md
- name: Crunch Base Get People Relationships
  x-api-slug: crunch-base
  description: Get People Relationships
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//people/{permalink}/{relationship_name}
  tags: People,Permalink,Relationship,Name
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/peoplepermalinkrelationship-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/peoplepermalinkrelationship-name-get-openapi.md
- name: Crunch Base Get Products
  x-api-slug: crunch-base
  description: Get Products
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//products
  tags: Products
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/products-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/products-get-openapi.md
- name: Crunch Base Get Products
  x-api-slug: crunch-base
  description: Get Products Using Permalink
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//products/{permalink}
  tags: Products,Permalink
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/productspermalink-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/productspermalink-get-openapi.md
- name: Crunch Base Get Product Relationships
  x-api-slug: crunch-base
  description: Get Product Relationships
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//products/{permalink}/{relationship_name}
  tags: Products,Permalink,Relationship,Name
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/productspermalinkrelationship-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/productspermalinkrelationship-name-get-openapi.md
- name: Crunch Base
  x-api-slug: crunch-base
  description: Build and transform financial apps and services with access to financial
    data through our APIs and digital solutions for banks, developers, and innovators.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3
  tags: Envestnet
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/envestnet/master/_listings/envestnet/openapi.md
x-common:
- type: x-base
  url: https://rest.developer.yodlee.com/services/srest/
- type: x-blog
  url: http://www.yodlee.com/yodlee-moneycenter-blog/
- type: x-blog-rss
  url: http://www.yodlee.com/yodlee-moneycenter-blog/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/yodlee
- type: x-crunchbase
  url: https://crunchbase.com/organization/yodlee
- type: x-developer
  url: http://developer.yodlee.com/
- type: x-email
  url: Customercare@yodlee.com
- type: x-email
  url: customerservice@yodlee.com
- type: x-github
  url: https://github.com/Yodlee
- type: x-twitter
  url: https://twitter.com/Yodlee
- type: x-website
  url: http://www.yodlee.com/
- type: x-website
  url: http://crunchbase.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---