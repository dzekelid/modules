---
swagger: "2.0"
x-collection-name: Azure Automation
x-complete: 0
info:
  title: Azure Automation API Module Get
  version: 1.0.0
  description: Retrieve the module identified by module name.
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/modules/{moduleName}
  : delete:
      summary: Module Delete
      description: Delete the module by name.
      operationId: Module_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamemodulesmodulename-delete
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: moduleName
        description: The module name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Module
    get:
      summary: Module Get
      description: Retrieve the module identified by module name.
      operationId: Module_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamemodulesmodulename-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: moduleName
        description: The module name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Module
    put:
      summary: Module Create Or Update
      description: Create or Update the module identified by module name.
      operationId: Module_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamemodulesmodulename-put
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: moduleName
        description: The name of module
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The create or update parameters for module
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Module
      - Or
    patch:
      summary: Module Update
      description: Update the module identified by module name.
      operationId: Module_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamemodulesmodulename-patch
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: moduleName
        description: The name of module
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The update parameters for module
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Module
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/modules
  : get:
      summary: Module List By Automation Account
      description: Retrieve a list of modules.
      operationId: Module_ListByAutomationAccount
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamemodules-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Module
      - List
      - Automation
      - Account
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