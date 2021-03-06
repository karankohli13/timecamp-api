Tasks
======

GET /tasks
----------

Return all tasks If you want to get only one specific task you can provide a task_id in get parametr.

Get Variable Array Fields:
* (optional) exclude_archived: 1 or 0 (default - we give both archived and not archived tasks)

Example:
`https://www.timecamp.com/third_party/api/tasks/api_token/a36cabi96bba83f826`
`https://www.timecamp.com/third_party/api/tasks/api_token/a36cabi96bba83f826/task_id/1234`

POST /tasks
----------

Add a new task. To add a task you should have proper permissions.

Example:
`https://www.timecamp.com/third_party/api/tasks/api_token/a36cabi96bba83f826`

Post Variable Array Fields:
* name: “Task name”
* keywords: “Keword 1, Keyword 2”
* parent_id: 0
* user_ids: ‘123,563,125’ (optional, comma separated)
* role: 1 (optional, by default 1, 1=manager, 3=regular user)
* external_task_id: "string" (optional)
* external_parent_id: "string" (optional)
* budget_unit: "string" (optional, hours/fee)

PUT /tasks
----------

Modify existing task. To modify a task you should have proper permissions.

Example:
`https://www.timecamp.com/third_party/api/tasks/api_token/a36cabi96bba83f826`

Put Variable Array Fields:
* task_id: 123
* name: “Task name” (optional)
* keywords: “Keword 1, Keyword 2” (optional)
* parent_id: 0 (optional)
* external_task_id: "string" (optional)
* external_parent_id: "string" (optional)
* budgeted: 2 (optional, in hours)
* note: "string" (optional)
* archived: 0 (optional, 0=no, 1=yes)
* billable: 0 (optional, 0=no, 1=yes)
* budget_unit: "string" (optional, hours/fee)
* user_ids: ‘123,563,125’ (optional, comma separated)
* role: 1 (optional, by default 1, 1=manager, 3=regular user)
