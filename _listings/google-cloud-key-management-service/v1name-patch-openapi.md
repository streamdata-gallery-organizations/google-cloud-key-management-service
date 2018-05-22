---
swagger: "2.0"
x-collection-name: Google Cloud Key Management Service
x-complete: 0
info:
  title: Google Cloud Key Management Service API Update Key
  description: |-
    Update a CryptoKeyVersion's metadata.

    state may be changed between
    ENABLED and
    DISABLED using this
    method. See DestroyCryptoKeyVersion and RestoreCryptoKeyVersion to
    move between other states.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: cloudkms.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{name}:
    get:
      summary: Get Key
      description: Returns metadata for a given CryptoKeyVersion.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.cryptoKeyVersions.get
      x-api-path-slug: v1name-get
      parameters:
      - in: path
        name: name
        description: The name of the CryptoKeyVersion to get
      responses:
        200:
          description: OK
      tags:
      - Key
    patch:
      summary: Update Key
      description: |-
        Update a CryptoKeyVersion's metadata.

        state may be changed between
        ENABLED and
        DISABLED using this
        method. See DestroyCryptoKeyVersion and RestoreCryptoKeyVersion to
        move between other states.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.cryptoKeyVersions.patch
      x-api-path-slug: v1name-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: Output only
      - in: query
        name: updateMask
        description: Required list of fields to be updated in this request
      responses:
        200:
          description: OK
      tags:
      - Key
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