---
swagger: "2.0"
x-collection-name: Medium
x-complete: 0
info:
  title: Medium Contributors of Publication
  description: This endpoint returns a list of contributors for a given publication.
    In other words, a list of Medium users who are allowed to publish under a publication,
    as well as a description of their exact role in the publication (for now, either
    an editor or a writer).
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
  /me:
    get:
      summary: User details
      description: Returns details of the user who has granted permission to the application.
      operationId: me.get
      x-api-path-slug: me-get
      responses:
        200:
          description: OK
      tags:
      - Me
  /publications/{publicationId}/contributors:
    get:
      summary: Contributors of Publication
      description: This endpoint returns a list of contributors for a given publication.
        In other words, a list of Medium users who are allowed to publish under a
        publication, as well as a description of their exact role in the publication
        (for now, either an editor or a writer).
      operationId: publications.publicationId.contributors.get
      x-api-path-slug: publicationspublicationidcontributors-get
      parameters:
      - in: path
        name: publicationId
        description: A unique identifier for the publication
      responses:
        200:
          description: OK
      tags:
      - Publications
      - Publication
      - Contributors
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