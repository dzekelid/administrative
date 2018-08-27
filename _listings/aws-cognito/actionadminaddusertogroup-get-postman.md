{
  "info": {
    "name": "AWS Cognito API Admin Add User To Group",
    "_postman_id": "d86d8563-1bcd-4243-a602-6783b7351232",
    "description": "Adds the specified user to the specified group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attributes",
      "item": [
        {
          "id": "623d6bc6-c800-403e-bec6-0f34ef85a20c",
          "name": "addCustomAttributes",
          "request": {
            "url": "http://example.com/api/?Action=AddCustomAttributes?CustomAttributes=CustomAttributes&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds additional user attributes to the user pool schema."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d39002e1-f055-4353-9f45-d3fe0ec55725"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "7ba1366b-a883-4dfd-b554-68d383bc621a",
          "name": "adminAddUserToGroup",
          "request": {
            "url": "http://example.com/api/?Action=AdminAddUserToGroup?GroupName=GroupName&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds the specified user to the specified group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "976cb292-6b9f-45d7-bf4d-189b2b18cd49"
            }
          ]
        }
      ]
    }
  ]
}