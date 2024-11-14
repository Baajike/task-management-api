# Task Management API
## Overview
A RESTful API built using Node.js and MongoDB, designed to handle basic task management operations including task creation, updating, viewing, and deletion.

## Features
- User Authentication: Secure signup and login using JWT.
- Task Management: CRUD operations for managing tasks.
- Filtering & Sorting: Options to sort and filter tasks by completion status, date, etc.
## Installation
### Clone the repository:

bash
```
git clone [repository link]
cd task-management-api
```
## Install dependencies:

### bash
```
npm install
```
## Set up environment variables:

- Create a config folder in the root directory.

- Inside config, create a dev.env file with the following contents:

### plaintext
```
PORT=3000
MONGODB_URL=[Your MongoDB Connection URI]
JWT_SECRET=[Your Secret Key]
```
## Run the API:

### bash
````
npm run dev
API Endpoints
````
## User:

- POST /users - Register a new user
- POST /users/login - Login a user
- GET /users/me - Get profile of the logged-in user
- DELETE /users/me - Delete the logged-in user
## Tasks:

- POST /tasks - Create a new task
- GET /tasks - Get all tasks (filterable)
- PATCH /tasks/:id - Update a task by ID
- DELETE /tasks/:id - Delete a task by ID
### Dependencies
- Node.js and Express for the server
- MongoDB and Mongoose for data storage
- JWT for user authentication
- Nodemon for development
