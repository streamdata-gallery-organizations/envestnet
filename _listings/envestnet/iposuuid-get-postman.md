{
  "info": {
    "name": "Crunch Base Get IPO",
    "_postman_id": "d8647d4c-7a2f-405b-8d56-64dad3490822",
    "description": "Get IPO Using UUID",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Acquisitions",
      "item": [
        {
          "id": "90011984-b27b-4571-8662-fed6fc415424",
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
              "id": "a358a900-c05e-4a65-9b4c-de0fbf1c5157"
            }
          ]
        },
        {
          "id": "fb8abd07-cf3f-4bec-ba42-7f8d14d8df9f",
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
              "id": "c99b32e5-92ae-4113-a060-261465a3a0a0"
            }
          ]
        }
      ]
    },
    {
      "name": "Categories",
      "item": [
        {
          "id": "07818ef3-1111-4b31-8402-effac28b8c88",
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
              "id": "7960a00b-0fa1-4101-a85b-31554f851b18"
            }
          ]
        }
      ]
    },
    {
      "name": "Funding",
      "item": [
        {
          "id": "75122dbc-a8f3-45b7-b6f2-456b31e03608",
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
              "id": "b480704c-43af-4729-8555-da5240c216a4"
            }
          ]
        },
        {
          "id": "7946f392-fa04-4710-af27-e0f3679f1dca",
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
              "id": "ab8af0ed-9543-4e06-881e-fc77bec1d6ee"
            }
          ]
        }
      ]
    },
    {
      "name": "Funds",
      "item": [
        {
          "id": "6d0490df-f510-4600-8eec-578663a8a404",
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
              "id": "d9d4584b-f58c-4401-a61c-9d5474533f07"
            }
          ]
        },
        {
          "id": "3fca66f4-c3ec-4c18-bcfe-947f398a83a7",
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
              "id": "00bcc0f6-1c72-42be-9de8-6cd3b5eebf3d"
            }
          ]
        }
      ]
    },
    {
      "name": "Ipos",
      "item": [
        {
          "id": "3e262271-791b-488b-ac3c-0907e55aa2a5",
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
              "id": "d4fcdfac-9739-4252-97df-fed70d8e508b"
            }
          ]
        }
      ]
    }
  ]
}