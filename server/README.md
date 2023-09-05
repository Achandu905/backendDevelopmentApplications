````markdown
# To-Do List API

## Introduction

This is a simple RESTful API for managing tasks in a To-Do list. The API allows users to create, retrieve, update, and delete tasks.

## Technologies Used

- Node.js
- Express.js
- TypeScript
- SQLite (as a lightweight database)
- Postman (for API testing and documentation)

## Installation

1. Clone the repository:

   ```shell
   git clone <repository_url>
   cd <project_folder>
   ```
````

2. Install dependencies:

   ```shell
   npm install
   ```

3. Start the server:

   ```shell
   npm start
   ```

The server will run on `http://localhost:3000` by default.

## API Documentation

For detailed API documentation and examples, please refer to the [Postman Collection](https://web.postman.co/workspace/7cc30f39-0bd4-4d63-85e9-7346afc7f41d/collection/28441795-63379ffa-be3f-45da-a6c0-f4a13a2d098e?action=share&creator=28441795).

## Endpoints

- Create a task (POST): `/tasks`
- Get all tasks (GET): `/tasks`
- Get a task by ID (GET): `/tasks/:id`
- Update a task by ID (PUT): `/tasks/:id`
- Delete a task by ID (DELETE): `/tasks/:id`

## Error Handling

- If a request to create a task is missing the required `title` or `description`, the server will respond with a 400 Bad Request and an error message.
- If a requested task by ID does not exist, the server will respond with a 404 Not Found and an error message.
- If there are server errors during processing, the server will respond with a 500 Internal Server Error and an error message.
