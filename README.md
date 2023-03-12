# todoapp-backend
Spring Boot RESTful API Controller for Task Management
This is a Spring Boot RESTful API Controller for managing tasks. It provides endpoints for reading, creating, updating, and deleting tasks. The controller uses the TaskService to interact with the data source.

Endpoints
The following endpoints are available:

Reading Tasks
-GET /api/v1/task/all - get all tasks
-GET /api/v1/task/id/{id} - get a task by id
-GET /api/v1/task/unfinished - get all unfinished tasks
-GET /api/v1/task/finished - get all finished tasks
-GET /api/v1/task/sort_by_id_ascending - sort tasks by id in ascending order
-GET /api/v1/task/sort_by_id_descending - sort tasks by id in descending order
-GET /api/v1/task/sort_by_priority_ascending - sort tasks by priority in ascending order
-GET /api/v1/task/sort_by_priority_descending - sort tasks by priority in descending order
-GET /api/v1/task/sort_by_difficulty_ascending - sort tasks by difficulty in ascending order
-GET /api/v1/task/sort_by_difficulty_descending - sort tasks by difficulty in descending order
-GET /api/v1/task/sort_by_created_ascending - sort tasks by creation time in ascending order
-GET /api/v1/task/sort_by_created_descending - sort tasks by creation time in descending order
-GET /api/v1/task/sort_by_estimate_ascending - sort tasks by estimate in ascending order
-GET /api/v1/task/sort_by_estimate_descending - sort tasks by estimate in descending order


Creating Tasks
-POST /api/v1/task - create a new task

Updating Tasks
-PUT /api/v1/task/update_to_finished/{id} - update a task to finished status
-PUT /api/v1/task/update_task_content/{id} - update a task's content

Deleting Tasks
-DELETE /api/v1/task/{id} - delete a task by id
-DELETE /api/v1/task/deleteAll - delete all tasks

Usage
-Prerequisites
-Java 8 or higher
-PostgreSQL installed and running
-Installation and Setup
-Clone the repository: git clone https://github.com/<username>/<reponame>.git
-Navigate to the project directory: cd <reponame>
-Create the PostgreSQL database and configure the application.properties file with the correct database credentials.
-Run the project: ./mvnw spring-boot:run
-The API should now be up and running on http://localhost:8080.

License
This project is licensed under the MIT License. See the LICENSE file for details.
