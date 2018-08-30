{
  "info": {
    "name": "Crunch Base Get Products",
    "_postman_id": "4a34f3ef-4f91-4498-a116-98221a90ad71",
    "description": "Get Products Using Permalink",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Acquisitions",
      "item": [
        {
          "id": "dd57fdfa-be5b-4b7c-9f84-a04ccdeb4250",
          "name": "acquistions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.crunchbase.com",
              "path": [
                "v",
                "3",
                "acquisitions/:uuid"
              ],
              "query": [
                {
                  "key": "user_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "uuid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Pull from Acquisition"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d85b008-9651-4788-aac7-efb919134dce"
            }
          ]
        },
        {
          "id": "4399c777-172a-4034-8f9e-f04906372ed4",
          "name": "acquisitionsRelationships",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.crunchbase.com",
              "path": [
                "v",
                "3",
                "acquisitions/:uuid/:relationship_name"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_order",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "relationship_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "uuid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Acquisitions Relationships"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1b8a269-27a2-4ef8-945b-1850ad8827e6"
            }
          ]
        }
      ]
    },
    {
      "name": "Categories",
      "item": [
        {
          "id": "680b12ca-c186-4a7e-85b4-fbd6a41774d1",
          "name": "categories",
          "request": {
            "url": "http://api.crunchbase.com/v/3/categories?page=%7B%7D&sort_order=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Categories"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84758f13-e699-4c05-9e3f-9ea371f8f38a"
            }
          ]
        }
      ]
    },
    {
      "name": "Funding",
      "item": [
        {
          "id": "afc374b6-215f-4545-8bf2-d4490f052906",
          "name": "fundingRounds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.crunchbase.com",
              "path": [
                "v",
                "3",
                "funding-rounds/:uuid"
              ],
              "query": [
                {
                  "key": "user_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "uuid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets funding rounds by UUID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c7b9412-9cd2-4de0-9cec-125a68c42d82"
            }
          ]
        },
        {
          "id": "cd593379-eec6-4052-baec-5f0b8f36778a",
          "name": "fundingRoundRelationships",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.crunchbase.com",
              "path": [
                "v",
                "3",
                "funding-rounds/:uuid/:relationship_name"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_order",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "relationship_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "uuid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Funding Rounds Relationships"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38bb9354-1035-4f63-8172-b31b12ddba14"
            }
          ]
        }
      ]
    },
    {
      "name": "Funds",
      "item": [
        {
          "id": "833f85be-8b54-4fdc-af0e-bbbc1a82c913",
          "name": "fundRelationships",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.crunchbase.com",
              "path": [
                "v",
                "3",
                "funds/:uuid/:relationship_name"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_order",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "uuid",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "relationship_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Fund Relationships"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bcdfd985-10f6-4902-a474-116bc922099b"
            }
          ]
        },
        {
          "id": "cd52c5f6-d6f5-44c9-92df-2f8098b9f7cb",
          "name": "funds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.crunchbase.com",
              "path": [
                "v",
                "3",
                "funds/:uuid"
              ],
              "variable": [
                {
                  "id": "uuid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Funds"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad52f738-7ba8-420b-b5e5-a669d0970d97"
            }
          ]
        }
      ]
    },
    {
      "name": "Ipos",
      "item": [
        {
          "id": "b3efa0b8-5ff1-4583-a7ef-ade951df60eb",
          "name": "ipo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.crunchbase.com",
              "path": [
                "v",
                "3",
                "ipos/:uuid"
              ],
              "query": [
                {
                  "key": "user_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "uuid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get IPO Using UUID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4674d2b9-20ca-40cb-a7bc-7e3b5d82ad00"
            }
          ]
        },
        {
          "id": "36f97a4e-6cc1-4dd4-9097-41a68d15e34f",
          "name": "ipoRelationships",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.crunchbase.com",
              "path": [
                "v",
                "3",
                "ipos/:uuid/:relationship_name"
              ],
              "query": [
                {
                  "key": "order",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "The page number to retrieve",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "relationship_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "uuid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get IPO Relationships"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "520ded94-b044-44db-add9-9f5e69d5bb0c"
            }
          ]
        }
      ]
    },
    {
      "name": "Locations",
      "item": [
        {
          "id": "31536d11-fba9-42a7-8213-47093ffbbd71",
          "name": "locations",
          "request": {
            "url": "http://api.crunchbase.com/v/3/locations?page=%7B%7D&sort_order=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Locations"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a18a5878-170e-45e8-bec2-e1ba585f58e9"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "1c392798-4e5a-4591-a546-99267ea66377",
          "name": "organizations",
          "request": {
            "url": "http://api.crunchbase.com/v/3/organizations?categories=%7B%7D&category_uuids=%7B%7D&domain_name=%7B%7D&locations=%7B%7D&name=%7B%7D&organization_types=%7B%7D&page=%7B%7D&query=%7B%7D&sort_order=%7B%7D&updated_since=%7B%7D&user_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Organizations"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "553c0e97-1970-4d50-99a8-fa4592590508"
            }
          ]
        },
        {
          "id": "5add63ed-a688-4510-bdf8-4dfab4bf089d",
          "name": "organizations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.crunchbase.com",
              "path": [
                "v",
                "3",
                "organizations/:permalink"
              ],
              "query": [
                {
                  "key": "user_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "permalink",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Organization Using Permalink"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ee53ab5-a26e-4603-9b78-00c8478ebab8"
            }
          ]
        },
        {
          "id": "b967d155-7d13-4844-af05-94b58156a7a4",
          "name": "organizationRelationships",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.crunchbase.com",
              "path": [
                "v",
                "3",
                "organizations/:permalink/:relationship_name"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_order",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "permalink",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "relationship_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Organizations Relationships Using Permlink"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6a520c3-4fb9-48e9-b0fc-0b523cc14d15"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "d5a20ac1-af4e-4f38-abe7-ea563aa874ec",
          "name": "people",
          "request": {
            "url": "http://api.crunchbase.com/v/3/people?locations=%7B%7D&name=%7B%7D&page=%7B%7D&query=%7B%7D&socials=%7B%7D&sort_order=%7B%7D&types=%7B%7D&updated_since=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get People"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6bba1b87-4317-4ea0-aafa-477d26aef3b4"
            }
          ]
        },
        {
          "id": "85f5eda9-df94-4a3c-bf02-8b4eed47a223",
          "name": "people",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.crunchbase.com",
              "path": [
                "v",
                "3",
                "people/:permalink"
              ],
              "query": [
                {
                  "key": "user_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "permalink",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get People Using Permalink"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af78aef0-bb75-4f97-a0d6-2d2daea98acc"
            }
          ]
        },
        {
          "id": "629dd180-e4c4-4b7f-9927-9a65381e3304",
          "name": "peopleRelationships",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.crunchbase.com",
              "path": [
                "v",
                "3",
                "people/:permalink/:relationship_name"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_order",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "permalink",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "relationship_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get People Relationships"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6aa39db0-2eae-4526-9a68-acba80d6bcdd"
            }
          ]
        }
      ]
    },
    {
      "name": "Products",
      "item": [
        {
          "id": "88a33945-23ce-4415-9087-53d94aad60d2",
          "name": "products",
          "request": {
            "url": "http://api.crunchbase.com/v/3/products?page=%7B%7D&sort_order=%7B%7D&updated_since=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Products"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79ba779c-ed6e-4977-96fb-16f2b33784a8"
            }
          ]
        },
        {
          "id": "751a4989-3750-4ec1-8296-3112179e5e7d",
          "name": "products",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.crunchbase.com",
              "path": [
                "v",
                "3",
                "products/:permalink"
              ],
              "query": [
                {
                  "key": "user_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "permalink",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Products Using Permalink"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e872efa-f4dd-4ce6-bfdf-f2896356a3c7"
            }
          ]
        }
      ]
    }
  ]
}