# User Management REST API

A simple REST API built with Node.js, Express.js, and MySQL that performs CRUD operations on user data.

## Features

* Get all users
* Get a user by ID
* Create a new user
* Create multiple users at once
* Update a user (PUT)
* Partially update a user (PATCH)
* Delete a user
* MySQL database integration
* Input validation
* Error handling

## Tech Stack

* Node.js
* Express.js
* MySQL
* Postman

## Installation

1. Clone the repository

```bash
git clone <repository-url>
```

2. Install dependencies

```bash
npm install
```

3. Configure MySQL database

Create a database:

```sql
CREATE DATABASE userdb;
```

Create a users table:

```sql
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(100),
    age INT,
    city VARCHAR(100)
);
```

4. Update database credentials in `db.js`

5. Start the server

```bash
node app.js
```

Server runs on:

```text
http://localhost:8000
```

## API Endpoints

### Get All Users

```http
GET /users
```

### Get User By ID

```http
GET /users/:id
```

### Create User

```http
POST /users
```

### Create Multiple Users

```http
POST /users/bulk
```

### Update User

```http
PUT /users/:id
```

### Partially Update User

```http
PATCH /users/:id
```

### Delete User

```http
DELETE /users/:id
```

## Tested With

* Postman

## Author

Nilam Sutar
