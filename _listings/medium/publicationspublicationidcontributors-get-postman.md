{
  "info": {
    "name": "Medium Contributors of Publication",
    "_postman_id": "11ffa1a0-9247-4185-81ea-5a7a57ef95a3",
    "description": "This endpoint returns a list of contributors for a given publication. In other words, a list of Medium users who are allowed to publish under a publication, as well as a description of their exact role in the publication (for now, either an editor or a writer).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "publications",
      "item": [
        {
          "id": "36c9be16-e6f0-448b-b8bd-6d560aa75f27",
          "name": "publications.publicationId.contributors.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.medium.com",
              "path": [
                "v1",
                "publications/:publicationId/contributors"
              ],
              "variable": [
                {
                  "id": "publicationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint returns a list of contributors for a given publication"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b80ddab0-c5d1-47a7-82d4-795f9465fbac"
            }
          ]
        }
      ]
    }
  ]
}