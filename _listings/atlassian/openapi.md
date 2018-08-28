swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:actionTarget:
    get:
      summary: Get a list of chat:actionTarget modules
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatActionTargetGetAllHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatactiontarget-get
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: query
        name: limit
        description: A maximum number of modules to return per call
      - in: query
        name: start
        description: Offset for the query
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Chat:actionTarget
      - Modules
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:bot:
    get:
      summary: Get a list of chat:bot modules
      description: Authentication required, with scope participate:conversation
      operationId: AppWebhookChatBotGetAllHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatbot-get
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: query
        name: limit
        description: A maximum number of modules to return per call
      - in: query
        name: start
        description: Offset for the query
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Chat:bot
      - Modules
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:bot:messages:
    get:
      summary: Get a list of chat:bot:messages modules
      description: Authentication required, with scope participate:conversation
      operationId: AppWebhookChatBotMessageGetAllHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatbotmessages-get
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: query
        name: limit
        description: A maximum number of modules to return per call
      - in: query
        name: start
        description: Offset for the query
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Chat:bot:messages
      - Modules
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:dialog:
    get:
      summary: Get a list of chat:dialog modules
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatDialogGetAllHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatdialog-get
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: query
        name: limit
        description: A maximum number of modules to return per call
      - in: query
        name: start
        description: Offset for the query
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Chat:dialog
      - Modules
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:externalPage:
    get:
      summary: Get a list of chat:externalPage modules
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatExternalPageGetAllHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatexternalpage-get
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: query
        name: limit
        description: A maximum number of modules to return per call
      - in: query
        name: start
        description: Offset for the query
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Chat:externalPage
      - Modules
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:glance:
    get:
      summary: Get a list of chat:glance modules
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatGlanceGetAllHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatglance-get
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: query
        name: limit
        description: A maximum number of modules to return per call
      - in: query
        name: start
        description: Offset for the query
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Chat:glance
      - Modules
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:sidebar:
    get:
      summary: Get a list of chat:sidebar modules
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatSidebarGetAllHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatsidebar-get
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: query
        name: limit
        description: A maximum number of modules to return per call
      - in: query
        name: start
        description: Offset for the query
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Chat:sidebar
      - Modules
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:webhook:
    get:
      summary: Get a list of chat:webhook modules
      description: Authentication required, with scope participate:conversation
      operationId: AppWebhookChatWebhookGetAllHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatwebhook-get
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: query
        name: limit
        description: A maximum number of modules to return per call
      - in: query
        name: start
        description: Offset for the query
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Chat:webhook
      - Modules
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:actionTarget/{key}:
    put:
      summary: Create or update a chat:actionTarget module
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatActionTargetPutHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatactiontargetkey-put
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: The key to identify the resource
      responses:
        200:
          description: OK
      tags:
      - Update
      - Chat:actionTarget
      - Module
    delete:
      summary: Delete a chat:actionTarget module
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatActionTargetDeleteHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatactiontargetkey-delete
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: The key to identify the resource
      responses:
        200:
          description: OK
      tags:
      - Chat:actionTarget
      - Module
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:bot/{key}:
    put:
      summary: Create or update a chat:bot module
      description: Authentication required, with scope participate:conversation
      operationId: AppWebhookChatBotPutHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatbotkey-put
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: The key to identify the resource
      responses:
        200:
          description: OK
      tags:
      - Update
      - Chat:bot
      - Module
    delete:
      summary: Delete a chat:bot module
      description: Authentication required, with scope participate:conversation
      operationId: AppWebhookChatBotDeleteHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatbotkey-delete
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: The key to identify the resource
      responses:
        200:
          description: OK
      tags:
      - Chat:bot
      - Module
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:bot:messages/{key}:
    put:
      summary: Create or update a chat:bot:messages module
      description: Authentication required, with scope participate:conversation
      operationId: AppWebhookChatBotMessagePutHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatbotmessageskey-put
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: The key to identify the resource
      responses:
        200:
          description: OK
      tags:
      - Update
      - Chat:bot:messages
      - Module
    delete:
      summary: Delete a chat:bot:messages module
      description: Authentication required, with scope participate:conversation
      operationId: AppWebhookChatBotMessageDeleteHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatbotmessageskey-delete
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: The key to identify the resource
      responses:
        200:
          description: OK
      tags:
      - Chat:bot:messages
      - Module
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:dialog/{key}:
    put:
      summary: Create or update a chat:dialog module
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatDialogPutHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatdialogkey-put
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: The key to identify the resource
      responses:
        200:
          description: OK
      tags:
      - Update
      - Chat:dialog
      - Module
    delete:
      summary: Delete a chat:dialog module
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatDialogDeleteHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatdialogkey-delete
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: The key to identify the resource
      responses:
        200:
          description: OK
      tags:
      - Chat:dialog
      - Module
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:externalPage/{key}:
    put:
      summary: Create or update a chat:externalPage module
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatExternalPagePutHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatexternalpagekey-put
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: The key to identify the resource
      responses:
        200:
          description: OK
      tags:
      - Update
      - Chat:externalPage
      - Module
    delete:
      summary: Delete a chat:externalPage module
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatExternalPageDeleteHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatexternalpagekey-delete
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: The key to identify the resource
      responses:
        200:
          description: OK
      tags:
      - Chat:externalPage
      - Module
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:glance/{key}:
    put:
      summary: Create or update a chat:glance module
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatGlancePutHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatglancekey-put
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: The key to identify the resource
      responses:
        200:
          description: OK
      tags:
      - Update
      - Chat:glance
      - Module
    delete:
      summary: Delete a chat:glance module
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatGlanceDeleteHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatglancekey-delete
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: The key to identify the resource
      responses:
        200:
          description: OK
      tags:
      - Chat:glance
      - Module
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:sidebar/{key}:
    put:
      summary: Create or update a chat:sidebar module
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatSidebarPutHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatsidebarkey-put
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: The key to identify the resource
      responses:
        200:
          description: OK
      tags:
      - Update
      - Chat:sidebar
      - Module
    delete:
      summary: Delete a chat:sidebar module
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatSidebarDeleteHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatsidebarkey-delete
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: The key to identify the resource
      responses:
        200:
          description: OK
      tags:
      - Chat:sidebar
      - Module
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:webhook/{key}:
    put:
      summary: Create or update a chat:webhook module
      description: Authentication required, with scope participate:conversation
      operationId: AppWebhookChatWebhookPutHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatwebhookkey-put
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: The key to identify the resource
      responses:
        200:
          description: OK
      tags:
      - Update
      - Chat:webhook
      - Module
    delete:
      summary: Delete a chat:webhook module
      description: Authentication required, with scope participate:conversation
      operationId: AppWebhookChatWebhookDeleteHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatwebhookkey-delete
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: The key to identify the resource
      responses:
        200:
          description: OK
      tags:
      - Chat:webhook
      - Module