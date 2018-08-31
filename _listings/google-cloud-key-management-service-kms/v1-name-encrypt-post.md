---
swagger: "2.0"
info:
  title: Google Cloud Key Management Service (KMS)
  description: Manages encryption for your cloud services the same way you do on-premise.
    You can generate, use, rotate, and destroy AES256 encryption keys.
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
  /v1/{name}:encrypt:
    post:
      summary: Encrypt Data
      description: Encrypt data, so that it can only be recovered by a call to Decrypt
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.encrypt
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: Required
      responses:
        200:
          description: OK
      tags:
      - encryption
definitions:
  AuditConfig:
    properties:
      auditLogConfigs:
        description: This is a default description.
        type: post
      exemptedMembers:
        description: This is a default description.
        type: post
      service:
        description: This is a default description.
        type: post
  AuditLogConfig:
    properties:
      exemptedMembers:
        description: This is a default description.
        type: post
      logType:
        description: This is a default description.
        type: post
  Binding:
    properties:
      members:
        description: This is a default description.
        type: post
      role:
        description: This is a default description.
        type: post
  CloudAuditOptions:
    properties: []
  Condition:
    properties:
      iam:
        description: This is a default description.
        type: post
      op:
        description: This is a default description.
        type: post
      svc:
        description: This is a default description.
        type: post
      sys:
        description: This is a default description.
        type: post
      value:
        description: This is a default description.
        type: post
      values:
        description: This is a default description.
        type: post
  CounterOptions:
    properties:
      field:
        description: This is a default description.
        type: post
      metric:
        description: This is a default description.
        type: post
  CryptoKey:
    properties:
      createTime:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      nextRotationTime:
        description: This is a default description.
        type: post
      purpose:
        description: This is a default description.
        type: post
      rotationPeriod:
        description: This is a default description.
        type: post
  CryptoKeyVersion:
    properties:
      createTime:
        description: This is a default description.
        type: post
      destroyEventTime:
        description: This is a default description.
        type: post
      destroyTime:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      state:
        description: This is a default description.
        type: post
  DataAccessOptions:
    properties: []
  DecryptRequest:
    properties:
      additionalAuthenticatedData:
        description: This is a default description.
        type: post
      ciphertext:
        description: This is a default description.
        type: post
  DecryptResponse:
    properties:
      plaintext:
        description: This is a default description.
        type: post
  DestroyCryptoKeyVersionRequest:
    properties: []
  EncryptRequest:
    properties:
      additionalAuthenticatedData:
        description: This is a default description.
        type: post
      plaintext:
        description: This is a default description.
        type: post
  EncryptResponse:
    properties:
      ciphertext:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  KeyRing:
    properties:
      createTime:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  ListCryptoKeyVersionsResponse:
    properties:
      cryptoKeyVersions:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
      totalSize:
        description: This is a default description.
        type: post
  ListCryptoKeysResponse:
    properties:
      cryptoKeys:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
      totalSize:
        description: This is a default description.
        type: post
  ListKeyRingsResponse:
    properties:
      keyRings:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
      totalSize:
        description: This is a default description.
        type: post
  ListLocationsResponse:
    properties:
      locations:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
  Location:
    properties:
      labels:
        description: This is a default description.
        type: post
      locationId:
        description: This is a default description.
        type: post
      metadata:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  LogConfig:
    properties: []
  Policy:
    properties:
      auditConfigs:
        description: This is a default description.
        type: post
      bindings:
        description: This is a default description.
        type: post
      etag:
        description: This is a default description.
        type: post
      iamOwned:
        description: This is a default description.
        type: post
      rules:
        description: This is a default description.
        type: post
      version:
        description: This is a default description.
        type: post
  RestoreCryptoKeyVersionRequest:
    properties: []
  Rule:
    properties:
      action:
        description: This is a default description.
        type: post
      conditions:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      in:
        description: This is a default description.
        type: post
      logConfig:
        description: This is a default description.
        type: post
      notIn:
        description: This is a default description.
        type: post
      permissions:
        description: This is a default description.
        type: post
  SetIamPolicyRequest:
    properties:
      updateMask:
        description: This is a default description.
        type: post
  TestIamPermissionsRequest:
    properties:
      permissions:
        description: This is a default description.
        type: post
  TestIamPermissionsResponse:
    properties:
      permissions:
        description: This is a default description.
        type: post
  UpdateCryptoKeyPrimaryVersionRequest:
    properties:
      cryptoKeyVersionId:
        description: This is a default description.
        type: post
x-collection-name: Google Cloud Key Management Service (KMS)
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