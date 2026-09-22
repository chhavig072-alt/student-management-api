# student-management-api

A REST API built with Node.js and Express.js to manage student records using in-memory array/JSON data.

## Tech Stack

- Node.js
- Express.js
- Postman (for testing)

## Project Structure

```
student-management-api/
├── app.js
├── routes/
│   └── studentRoutes.js
├── middleware/
│   └── logger.js
├── data/
│   └── students.js
└── package.json
```

## Setup

```bash
npm install express
npm start
```

Server runs on `http://localhost:3000`

## API Endpoints

| Method | Endpoint       | Description             |
|--------|----------------|--------------------------|
| GET    | /students      | Get all students         |
| GET    | /students/:id  | Get a student by ID      |
| POST   | /students      | Create a new student     |
| PUT    | /students/:id  | Update a student         |
| DELETE | /students/:id  | Delete a student         |

## Sample Request Body (POST/PUT)

```json
{
  "name": "Sneha",
  "course": "BSc"
}
```

## Status Codes

| Code | Meaning       |
|------|---------------|
| 200  | Success       |
| 201  | Created       |
| 400  | Bad Request   |
| 404  | Not Found     |
