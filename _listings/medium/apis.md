---
name: Medium
x-slug: medium
description: Medium is an online publishing platform founded by Twitter co-founder
  Evan Williams in August 2012. The platform has evolved into a hybrid of non-professional
  contributions and professional, paid contributions, an example of social journalism.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/medium-logo.png
x-kinRank: "8"
x-alexaRank: ""
tags: Medium
created: "2018-05-22"
modified: "2018-05-22"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/medium/master/_listings/medium/apis.md
specificationVersion: "0.14"
apis:
- name: Medium User details
  x-api-slug: medium
  description: Returns details of the user who has granted permission to the application.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/medium-logo.png
  humanURL: https://medium.com/
  baseURL: https://api.medium.com//v1//me
  tags: Me
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/medium/master/_listings/medium/me-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/medium/master/_listings/medium/me-get-openapi.md
- name: Medium Contributors of Publication
  x-api-slug: medium
  description: This endpoint returns a list of contributors for a given publication.
    In other words, a list of Medium users who are allowed to publish under a publication,
    as well as a description of their exact role in the publication (for now, either
    an editor or a writer).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/medium-logo.png
  humanURL: https://medium.com/
  baseURL: https://api.medium.com//v1//publications/{publicationId}/contributors
  tags: Publications, Publication, Contributors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/medium/master/_listings/medium/publicationspublicationidcontributors-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/medium/master/_listings/medium/publicationspublicationidcontributors-get-openapi.md
- name: Medium Create Publication Post
  x-api-slug: medium
  description: |-
    creating a post and associating it with a publication on Medium. The request also shows this association, considering posts a collection of resources under a publication

    There are additional rules around publishing that each request to this API must respect:
      - If the authenticated user is an 'editor' for the publication, they can create posts with any publish status. Posts published as 'public' or 'unlisted' will appear in collection immediately, while posts created as 'draft' will remain in pending state under publication.
      - If the authenticated user is a 'writer' for the chosen publication, they can only create a post as a 'draft'. That post will remain in pending state under publication until an editor for the publication approves it.
      - If the authenticated user is neither a 'writer' nor an 'editor', they are not allowed to create any posts in a publication.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/medium-logo.png
  humanURL: https://medium.com/
  baseURL: https://api.medium.com//v1//publications/{publicationId}/posts
  tags: Publications, Publication, Posts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/medium/master/_listings/medium/publicationspublicationidposts-post-openapi.md
- name: Medium Create User Post
  x-api-slug: medium
  description: "Creates a post on the authenticated user\u2019s profile."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/medium-logo.png
  humanURL: https://medium.com/
  baseURL: https://api.medium.com//v1//users/{authorId}/posts
  tags: Users, Author, Posts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/medium/master/_listings/medium/usersauthoridposts-post-openapi.md
- name: Medium User's publications
  x-api-slug: medium
  description: Returns a full list of publications that the user is related to in
    some way. This includes all publications the user is subscribed to, writes to,
    or edits.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/medium-logo.png
  humanURL: https://medium.com/
  baseURL: https://api.medium.com//v1//users/{userId}/publications
  tags: Users, User, Publications
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/medium/master/_listings/medium/usersuseridpublications-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/medium/master/_listings/medium/usersuseridpublications-get-openapi.md
- name: Medium
  x-api-slug: medium
  description: Medium is an online publishing platform founded by Twitter co-founder
    Evan Williams in August 2012. The platform has evolved into a hybrid of non-professional
    contributions and professional, paid contributions, an example of social journalism.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/medium-logo.png
  humanURL: https://medium.com/
  baseURL: https://api.medium.com//v1
  tags: Medium
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/medium/master/_listings/medium/openapi.md
x-common:
- type: x-github
  url: https://github.com/Medium
- type: x-transparency-report
  url: https://medium.com/transparency-report
- type: x-twitter
  url: https://twitter.com/Medium
- type: x-website
  url: https://medium.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---