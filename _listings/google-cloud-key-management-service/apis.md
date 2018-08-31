---
name: Google Cloud Key Management Service
x-slug: google-cloud-key-management-service
description: Cloud KMS is a cloud-hosted key management service that lets you manage
  encryption for your cloud services the same way you do on-premises. You can generate,
  use, rotate and destroy AES256 encryption keys. Cloud KMS is integrated with IAM
  and Cloud Audit Logging so that you can manage permissions on individual keys, and
  monitor how these are used. Use Cloud KMS to protect secrets and other sensitive
  data which you need to store in Google Cloud Platform.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Google Cloud Key Management Service
created: "2018-08-30"
modified: "2018-08-30"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/apis.md
specificationVersion: "0.14"
apis:
- name: Google Cloud Key Management Service (KMS) - Get Key
  x-api-slug: v1name-get
  description: Returns metadata for a given CryptoKeyVersion.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
  humanURL: https://cloud.google.com/kms/
  baseURL: ://cloudkms.googleapis.com//
  tags: Authentication, Management, Google APIs, Stack Network, Security, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1name-get-openapi.md
- name: Google Cloud Key Management Service (KMS) - Update Key
  x-api-slug: v1name-patch
  description: |-
    Update a CryptoKeyVersion's metadata.

    state may be changed between
    ENABLED and
    DISABLED using this
    method. See DestroyCryptoKeyVersion and RestoreCryptoKeyVersion to
    move between other states.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
  humanURL: https://cloud.google.com/kms/
  baseURL: ://cloudkms.googleapis.com//
  tags: Authentication, Management, Google APIs, Stack Network, Security, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1name-patch-openapi.md
- name: Google Cloud Key Management Service (KMS) - Get Locations
  x-api-slug: v1namelocations-get
  description: Lists information about the supported locations for this service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
  humanURL: https://cloud.google.com/kms/
  baseURL: ://cloudkms.googleapis.com//
  tags: Authentication, Management, Google APIs, Stack Network, Security, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1namelocations-get-openapi.md
- name: Google Cloud Key Management Service (KMS) - Decrypt Data
  x-api-slug: v1namedecrypt-post
  description: Decrypt data that was protected by Encrypt.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
  humanURL: https://cloud.google.com/kms/
  baseURL: ://cloudkms.googleapis.com//
  tags: Authentication, Management, Google APIs, Stack Network, Security, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1namedecrypt-post-openapi.md
- name: Google Cloud Key Management Service (KMS) - Destroy Key
  x-api-slug: v1namedestroy-post
  description: |-
    Schedule a CryptoKeyVersion for destruction.

    Upon calling this method, CryptoKeyVersion.state will be set to
    DESTROY_SCHEDULED
    and destroy_time will be set to a time 24
    hours in the future, at which point the state
    will be changed to
    DESTROYED, and the key
    material will be irrevocably destroyed.

    Before the destroy_time is reached,
    RestoreCryptoKeyVersion may be called to reverse the process.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
  humanURL: https://cloud.google.com/kms/
  baseURL: ://cloudkms.googleapis.com//
  tags: Authentication, Management, Google APIs, Stack Network, Security, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1namedestroy-post-openapi.md
- name: Google Cloud Key Management Service (KMS) - Encrypt Data
  x-api-slug: v1nameencrypt-post
  description: Encrypt data, so that it can only be recovered by a call to Decrypt.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
  humanURL: https://cloud.google.com/kms/
  baseURL: ://cloudkms.googleapis.com//
  tags: Authentication, Management, Google APIs, Stack Network, Security, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1nameencrypt-post-openapi.md
- name: Google Cloud Key Management Service (KMS) - Restore Key
  x-api-slug: v1namerestore-post
  description: |-
    Restore a CryptoKeyVersion in the
    DESTROY_SCHEDULED,
    state.

    Upon restoration of the CryptoKeyVersion, state
    will be set to DISABLED,
    and destroy_time will be cleared.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
  humanURL: https://cloud.google.com/kms/
  baseURL: ://cloudkms.googleapis.com//
  tags: Authentication, Management, Google APIs, Stack Network, Security, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1namerestore-post-openapi.md
- name: Google Cloud Key Management Service (KMS) - Update Version
  x-api-slug: v1nameupdateprimaryversion-post
  description: Update the version of a CryptoKey that will be used in Encrypt
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
  humanURL: https://cloud.google.com/kms/
  baseURL: ://cloudkms.googleapis.com//
  tags: Authentication, Management, Google APIs, Stack Network, Security, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1nameupdateprimaryversion-post-openapi.md
- name: Google Cloud Key Management Service (KMS) - List Key Versions
  x-api-slug: v1parentcryptokeyversions-get
  description: Lists CryptoKeyVersions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
  humanURL: https://cloud.google.com/kms/
  baseURL: ://cloudkms.googleapis.com//
  tags: Authentication, Management, Google APIs, Stack Network, Security, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1parentcryptokeyversions-get-openapi.md
- name: Google Cloud Key Management Service (KMS) - Create Key Version
  x-api-slug: v1parentcryptokeyversions-post
  description: |-
    Create a new CryptoKeyVersion in a CryptoKey.

    The server will assign the next sequential id. If unset,
    state will be set to
    ENABLED.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
  humanURL: https://cloud.google.com/kms/
  baseURL: ://cloudkms.googleapis.com//
  tags: Authentication, Management, Google APIs, Stack Network, Security, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1parentcryptokeyversions-post-openapi.md
- name: Google Cloud Key Management Service (KMS) - List Keys
  x-api-slug: v1parentcryptokeys-get
  description: Lists CryptoKeys.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
  humanURL: https://cloud.google.com/kms/
  baseURL: ://cloudkms.googleapis.com//
  tags: Authentication, Management, Google APIs, Stack Network, Security, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1parentcryptokeys-get-openapi.md
- name: Google Cloud Key Management Service (KMS) - Create Key
  x-api-slug: v1parentcryptokeys-post
  description: |-
    Create a new CryptoKey within a KeyRing.

    CryptoKey.purpose is required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
  humanURL: https://cloud.google.com/kms/
  baseURL: ://cloudkms.googleapis.com//
  tags: Authentication, Management, Google APIs, Stack Network, Security, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1parentcryptokeys-post-openapi.md
- name: Google Cloud Key Management Service (KMS) - List Key Rings
  x-api-slug: v1parentkeyrings-get
  description: Lists KeyRings.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
  humanURL: https://cloud.google.com/kms/
  baseURL: ://cloudkms.googleapis.com//
  tags: Authentication, Management, Google APIs, Stack Network, Security, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1parentkeyrings-get-openapi.md
- name: Google Cloud Key Management Service (KMS) - Create Key Ring
  x-api-slug: v1parentkeyrings-post
  description: Create a new KeyRing in a given Project and Location.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
  humanURL: https://cloud.google.com/kms/
  baseURL: ://cloudkms.googleapis.com//
  tags: Authentication, Management, Google APIs, Stack Network, Security, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1parentkeyrings-post-openapi.md
- name: Google Cloud Key Management Service (KMS) - Get IAM Policy
  x-api-slug: v1resourcegetiampolicy-get
  description: |-
    Gets the access control policy for a resource.
    Returns an empty policy if the resource exists and does not have a policy
    set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
  humanURL: https://cloud.google.com/kms/
  baseURL: ://cloudkms.googleapis.com//
  tags: Authentication, Management, Google APIs, Stack Network, Security, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1resourcegetiampolicy-get-openapi.md
- name: Google Cloud Key Management Service (KMS) - Set IAM Policy
  x-api-slug: v1resourcesetiampolicy-post
  description: |-
    Sets the access control policy on the specified resource. Replaces any
    existing policy.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
  humanURL: https://cloud.google.com/kms/
  baseURL: ://cloudkms.googleapis.com//
  tags: Authentication, Management, Google APIs, Stack Network, Security, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1resourcesetiampolicy-post-openapi.md
- name: Google Cloud Key Management Service (KMS) - Test IAM Permissions
  x-api-slug: v1resourcetestiampermissions-post
  description: |-
    Returns permissions that a caller has on the specified resource.
    If the resource does not exist, this will return an empty set of
    permissions, not a NOT_FOUND error.

    Note: This operation is designed to be used for building permission-aware
    UIs and command-line tools, not for authorization checking. This operation
    may "fail open" without warning.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kms-lead.png
  humanURL: https://cloud.google.com/kms/
  baseURL: ://cloudkms.googleapis.com//
  tags: Authentication, Management, Google APIs, Stack Network, Security, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-key-management-service/master/_listings/google-cloud-key-management-service/v1resourcetestiampermissions-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.cloud.identity.access.management.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.cloud.key.management.service.stack.network
- type: x-change-log
  url: https://cloud.google.com/kms/docs/release-notes
- type: x-code
  url: https://cloud.google.com/kms/docs/reference/libraries
- type: x-concepts
  url: https://cloud.google.com/kms/docs/concepts
- type: x-getting-started
  url: https://cloud.google.com/kms/docs/quickstart
- type: x-how-to-guides
  url: https://cloud.google.com/kms/docs/how-tos
- type: x-issues
  url: https://cloud.google.com/kms/known-issues
- type: x-pricing
  url: https://cloud.google.com/kms/pricing
- type: x-rate-limits
  url: https://cloud.google.com/kms/quota
- type: x-service-level-agreement
  url: https://cloud.google.com/kms/sla
- type: x-support
  url: https://cloud.google.com/kms/docs/support
- type: x-website
  url: https://cloud.google.com/kms/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---