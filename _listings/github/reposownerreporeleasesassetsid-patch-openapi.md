---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 0
info:
  title: Github Patch Repos Owner Repo Releases Assets
  description: |-
    Edit a release asset
    Users with push access to the repository can edit a release asset.
  termsOfService: https://help.github.com/articles/github-terms-of-service/#b-api-terms
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repos/{owner}/{repo}/releases/assets/{id}:
    delete:
      summary: Delete Repos Owner Repo Releases Assets
      description: Delete a release asset
      operationId: delete-a-release-asset
      x-api-path-slug: reposownerreporeleasesassetsid-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: id
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Releases
      - Assets
    get:
      summary: Get Repos Owner Repo Releases Assets
      description: Get a single release asset
      operationId: get-a-single-release-asset
      x-api-path-slug: reposownerreporeleasesassetsid-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: id
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Releases
      - Assets
    patch:
      summary: Patch Repos Owner Repo Releases Assets
      description: |-
        Edit a release asset
        Users with push access to the repository can edit a release asset.
      operationId: edit-a-release-assetusers-with-push-access-to-the-repository-can-edit-a-release-asset
      x-api-path-slug: reposownerreporeleasesassetsid-patch
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Releases
      - Assets
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