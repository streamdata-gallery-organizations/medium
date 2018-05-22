{
  "info": {
    "name": "Medium User details",
    "_postman_id": "df98b86b-b3b7-4c11-b642-4a86bea578a9",
    "description": "Returns details of the user who has granted permission to the application.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Me",
      "item": [
        {
          "id": "9b786370-2e22-4bd6-9cf1-d9f0b0b58130",
          "name": "me.get",
          "request": {
            "url": "http://api.medium.com/v1/me",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns details of the user who has granted permission to the application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1a98096-fc24-44c0-a884-84a5b618de94"
            }
          ]
        }
      ]
    }
  ]
}