swagger: "2.0"
x-collection-name: Actility
x-complete: 1
info:
  title: ThingPark DX Maker API
  description: api-providing-features-for-device-makers-such-as-preprovisioning-on-standalone-join-servers-
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /maker/v011/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /moduleConfigs:
    get:
      summary: Module configurations retrieval
      description: Retrieves the list of existing module configurations.
      operationId: retrieves-the-list-of-existing-module-configurations
      x-api-path-slug: moduleconfigs-get
      responses:
        200:
          description: OK
      tags:
      - Module
      - Configurations
      - Retrieval
    post:
      summary: Module configuration creation
      description: Creates a new module configuration.
      operationId: creates-a-new-module-configuration
      x-api-path-slug: moduleconfigs-post
      parameters:
      - in: body
        name: moduleConfig
        description: Contents of the module configuration to create
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Module
      - Configuration
      - Creation
  /moduleConfigs/{moduleConfigRef}:
    get:
      summary: Module configuration retrieval
      description: Retrieves the module configuration corresponding to the provided
        ref.
      operationId: retrieves-the-module-configuration-corresponding-to-the-provided-ref
      x-api-path-slug: moduleconfigsmoduleconfigref-get
      parameters:
      - in: path
        name: moduleConfigRef
        description: Ref of the module configuration to retrieve
      responses:
        200:
          description: OK
      tags:
      - Module
      - Configuration
      - Retrieval
    put:
      summary: Module configuration update
      description: Updates the module configuration corresponding to the provided
        ref.
      operationId: updates-the-module-configuration-corresponding-to-the-provided-ref
      x-api-path-slug: moduleconfigsmoduleconfigref-put
      parameters:
      - in: body
        name: moduleConfig
        description: Contents of the module configuration to update
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: moduleConfigRef
        description: Ref of the module configuration to update
      responses:
        200:
          description: OK
      tags:
      - Module
      - Configuration
      - Update
    delete:
      summary: Module configuration deletion
      description: Deletes the module configuration corresponding to the provided
        ref.
      operationId: deletes-the-module-configuration-corresponding-to-the-provided-ref
      x-api-path-slug: moduleconfigsmoduleconfigref-delete
      parameters:
      - in: path
        name: moduleConfigRef
        description: Ref of the module configuration to delete
      responses:
        200:
          description: OK
      tags:
      - Module
      - Configuration
      - Deletion