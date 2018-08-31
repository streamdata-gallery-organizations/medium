---
swagger: "2.0"
info:
  title: Medium.com
  description: Medium&rsquo;s unofficial API documentation using OpenAPI specification.#
    Official APIOfficial API document can also be viewed for most up to date API spec
    at [https://github.com/Medium/medium-api-docs](https://github.com/Medium/medium-api-docs).Developer
    Blog - [Welcome to the Medium API](https://medium.com/blog/welcome-to-the-medium-api-3418f956552)
  termsOfService: https://medium.com/@feerst/2b405a832a2f
  contact:
    name: Hossain Khan
    url: https://github.com/amardeshbd/medium-api-specification
  version: 1.0.0
host: api.medium.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /publications/{publicationId}/contributors:
    get:
      summary: Contributors of Publication
      description: This endpoint returns a list of contributors for a given publication
      operationId: publications.publicationId.contributors.get
      parameters:
      - in: path
        name: publicationId
        description: A unique identifier for the publication
      responses:
        200:
          description: OK
      tags:
      - publications
      - publication
      - contributors
definitions:
  Contibutor:
    properties:
      publicationId:
        description: This is a default description.
        type: get
      role:
        description: This is a default description.
        type: get
      userId:
        description: This is a default description.
        type: get
  ContibutorResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  Post:
    properties:
      canonicalUrl:
        description: This is a default description.
        type: get
      content:
        description: This is a default description.
        type: get
      contentFormat:
        description: This is a default description.
        type: get
      license:
        description: This is a default description.
        type: get
      publishStatus:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
  PostDetails:
    properties:
      authorId:
        description: This is a default description.
        type: get
      canonicalUrl:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      license:
        description: This is a default description.
        type: get
      licenseUrl:
        description: This is a default description.
        type: get
      publishStatus:
        description: This is a default description.
        type: get
      publishedAt:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
      url:
        description: This is a default description.
        type: get
  Publication:
    properties:
      description:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      imageUrl:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      url:
        description: This is a default description.
        type: get
  PublicationResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  User:
    properties:
      id:
        description: This is a default description.
        type: get
      imageUrl:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      url:
        description: This is a default description.
        type: get
      username:
        description: This is a default description.
        type: get
  UserResponse:
    properties: []
x-collection-name: Medium
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