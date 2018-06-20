{
  "info": {
    "name": "Crunch Base Get Products",
    "_postman_id": "24b910f2-5ef6-4d6c-9630-aa939260f53c",
    "description": "Get Products",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Acquisitions",
      "item": [
        {
          "id": "bfc25109-f57f-44d6-a8a8-f8b5493f760c",
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
              "id": "437ce807-04e5-4511-8f7f-f3b508d54718"
            }
          ]
        },
        {
          "id": "1256b54b-92c7-4e72-bd43-d1b4e03f6cab",
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
              "id": "cda5534b-9d8d-4882-9fb2-7152ceed8e68"
            }
          ]
        }
      ]
    },
    {
      "name": "Categories",
      "item": [
        {
          "id": "bcadb5be-2968-4185-a8da-54f4a7dd6436",
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
              "id": "e727acad-4b67-402b-8c23-82ae68ce5ec4"
            }
          ]
        }
      ]
    },
    {
      "name": "Funding",
      "item": [
        {
          "id": "ef12201e-2333-41ca-9e03-320479f141a3",
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
              "id": "2c25953d-6c93-42c7-89ac-8a3c38d49cc0"
            }
          ]
        },
        {
          "id": "61f1e3fa-670c-4cbb-8039-917d51b5f053",
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
              "id": "5538b309-eb74-42c9-991d-979af4aeab18"
            }
          ]
        }
      ]
    },
    {
      "name": "Funds",
      "item": [
        {
          "id": "72ee51d5-eaf2-4944-b09a-63e1503e2b79",
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
              "id": "137c4cc5-7ecb-4928-8e1c-7b3e9b5b3aac"
            }
          ]
        },
        {
          "id": "565dcd96-24a1-4c78-af93-4d97c9a8a69a",
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
              "id": "31f2c1de-e85a-40cb-85c3-ebfffa74a4f5"
            }
          ]
        }
      ]
    },
    {
      "name": "Ipos",
      "item": [
        {
          "id": "df49aa37-42f3-495a-b008-6c7b068e9854",
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
              "id": "160ed5f9-2b67-40e4-9464-aedb579e119f"
            }
          ]
        },
        {
          "id": "4652d2ff-366a-4c82-9d10-e8089fbe540e",
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
              "id": "760a7c03-23a2-4a13-9292-3cc2f1fafc34"
            }
          ]
        }
      ]
    },
    {
      "name": "Locations",
      "item": [
        {
          "id": "2c2168aa-5866-407b-8234-91bada45d0b1",
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
              "id": "a58a00a4-357e-45f3-b5f4-c48d9a16e0e6"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "49e85d3b-3360-40e2-a7eb-9da956e3af06",
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
              "id": "8efdd84f-1874-4945-81c7-85d0e4dfcb3a"
            }
          ]
        },
        {
          "id": "a392185d-3b40-4640-b618-9222c3abd436",
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
              "id": "f0136642-263c-4b79-a7a6-dac3dcbf6dbb"
            }
          ]
        },
        {
          "id": "ecce18ea-e0a1-4efc-a6d9-30008f5f2238",
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
              "id": "3e1b742f-6685-4595-a701-098bd889144b"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "607d4ee3-0c01-4e95-a030-7a7f4c1b77d0",
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
              "id": "cca2cc28-4f5a-4b29-9189-531a196854d1"
            }
          ]
        },
        {
          "id": "f6fa711b-51cc-4ba7-b563-59c507df6adb",
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
              "id": "59fdacf2-a96b-458d-aa39-4221119ed83a"
            }
          ]
        },
        {
          "id": "790ac6f7-920a-460f-b09e-4d4211acf2be",
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
              "id": "306f88c9-101a-489d-a434-26f229f7ee4e"
            }
          ]
        }
      ]
    },
    {
      "name": "Products",
      "item": [
        {
          "id": "a8b59e49-a961-4bcd-ad7a-966b9303dad7",
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
              "id": "643f08b2-ba04-4202-aade-5946e5b0a0e2"
            }
          ]
        }
      ]
    }
  ]
}