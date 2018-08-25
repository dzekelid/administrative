{
  "info": {
    "name": "GIGANDCROWD Post Admin Event Approve Eventid",
    "_postman_id": "537c6271-ac5b-4ce8-9658-f973e38e92c1",
    "description": "Post admin event approve eventid.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Art",
      "item": [
        {
          "id": "f0e69aec-76e4-4aa7-8817-ae884e7571eb",
          "name": "getApiV1ArtEventsPast",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/art/:id/events/past"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get art events past."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d7c0722-3815-4de2-910e-810ac977ca39"
            }
          ]
        }
      ]
    },
    {
      "name": "City",
      "item": [
        {
          "id": "3cb399a7-4314-49b1-9afc-de1061bd92ba",
          "name": "getApiV1CityEvents",
          "request": {
            "url": "http://gigandcrowd.com/api/v1/city/events",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get city events."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8664444c-4f17-4d3e-995c-6a7d9373c2d5"
            }
          ]
        }
      ]
    },
    {
      "name": "Gigme",
      "item": [
        {
          "id": "01550ab2-8cd1-4b87-b3bb-ba86e1c8fdd8",
          "name": "getApiV1GigmeArtistEventsPast",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/gigme/artist/:id/events/past"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get gigme artist events past."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ca011e5-3759-4712-8e53-a897113de214"
            }
          ]
        },
        {
          "id": "d695c310-85c1-4b3a-b022-595f06560a01",
          "name": "getApiV1GigmeArtistEventsFuture",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/gigme/artist/:id/events/future"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get gigme artist events future."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c29f2e44-e423-4bf0-8976-f71148b446d7"
            }
          ]
        },
        {
          "id": "a389a1e8-021b-4541-a8bb-43ce8dfa65cb",
          "name": "getApiV1GigmeCityEvents",
          "request": {
            "url": "http://gigandcrowd.com/api/v1/gigme/city/events",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get gigme city events."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d63d0049-84bb-4874-b73a-d4b29dfb8fb5"
            }
          ]
        }
      ]
    },
    {
      "name": "Admin",
      "item": [
        {
          "id": "ee09c585-27a6-4641-a9cf-8808f81a53de",
          "name": "postApiV1AdminEventApproveEvent",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/admin/event/approve/:eventId"
              ],
              "variable": [
                {
                  "id": "eventId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Post admin event approve eventid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce354072-dbec-4d13-9039-273d3969bff7"
            }
          ]
        }
      ]
    }
  ]
}