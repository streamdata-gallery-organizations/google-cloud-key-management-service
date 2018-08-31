{
  "info": {
    "name": "Google Cloud Key Management Service API Get Key",
    "_postman_id": "31f91ce3-8bc4-4f17-b2d2-a9fbc3e6ed8c",
    "description": "Returns metadata for a given CryptoKeyVersion.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Key",
      "item": [
        {
          "id": "5cc6fdbf-40be-4c58-9548-520b2e0eae6d",
          "name": "cloudkms.projects.locations.keyRings.cryptoKeys.cryptoKeyVersions.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "cloudkms.googleapis.com",
              "path": [
                "v1/:name"
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metadata for a given CryptoKeyVersion."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4661bbc4-65a4-4869-a9b4-2d838725eea6"
            }
          ]
        }
      ]
    }
  ]
}