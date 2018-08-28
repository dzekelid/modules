---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API Delete module
  description: Delete module.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/modules:
    get:
      summary: List modules
      description: List modules.
      operationId: list-modules
      x-api-path-slug: coursescourse-idmodules-get
      parameters:
      - in: query
        name: include[]
        description: 'u201citemsu201d: Return module items inline if possible'
      - in: query
        name: search_term
        description: The partial name of the modules (and module items, if include
          is specified) to match and return
      - in: query
        name: student_id
        description: Returns module completion information for the student with this
          id
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
    post:
      summary: Create a module
      description: Create a module.
      operationId: create-a-module
      x-api-path-slug: coursescourse-idmodules-post
      parameters:
      - in: query
        name: module[name]
        description: The name of the module
      - in: query
        name: module[position]
        description: The position of this module in the course (1-based)
      - in: query
        name: module[prerequisite_module_ids][]
        description: IDs of Modules that must be completed before this one is unlocked
      - in: query
        name: module[publish_final_grade]
        description: Whether to publish the student&#39;s final grade for the course
          uponncompletion of this module
      - in: query
        name: module[require_sequential_progress]
        description: Whether module items must be unlocked in order
      - in: query
        name: module[unlock_at]
        description: The date the module will unlock
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
  /courses/{course_id}/modules/id:
    delete:
      summary: Delete module
      description: Delete module.
      operationId: delete-module
      x-api-path-slug: coursescourse-idmodulesid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
      - Id
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