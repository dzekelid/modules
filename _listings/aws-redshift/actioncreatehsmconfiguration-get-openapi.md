---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Create Hsm Configuration
  version: 1.0.0
  description: |-
    Creates an HSM configuration that contains the information required by an Amazon Redshift
                cluster to store and use database encryption keys in a Hardware Security Module (HSM).
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateHsmConfiguration:
    get:
      summary: Create Hsm Configuration
      description: |-
        Creates an HSM configuration that contains the information required by an Amazon Redshift
                    cluster to store and use database encryption keys in a Hardware Security Module (HSM).
      operationId: createHsmConfiguration
      x-api-path-slug: actioncreatehsmconfiguration-get
      parameters:
      - in: query
        name: Description
        description: A text description of the HSM configuration to be created
        type: string
      - in: query
        name: HsmConfigurationIdentifier
        description: The identifier to be assigned to the new Amazon Redshift HSM
          configuration
        type: string
      - in: query
        name: HsmIpAddress
        description: The IP address that the Amazon Redshift cluster must use to access
          the HSM
        type: string
      - in: query
        name: HsmPartitionName
        description: The name of the partition in the HSM where the Amazon Redshift
          clusters will store their            database encryption keys
        type: string
      - in: query
        name: HsmPartitionPassword
        description: The password required to access the HSM partition
        type: string
      - in: query
        name: HsmServerPublicCertificate
        description: The HSMs public certificate file
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Configurations
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