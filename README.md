# PostgreSQL Express CRUD API (with .env)

## Setup Instructions

1. **Install Dependencies**
```
npm install express pg body-parser dotenv
```

2. **Configure Database**
- Install PostgreSQL and create a database.
- Run this SQL command to create the table:
```
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100),
  email VARCHAR(100),
  age INTEGER
);
```

3. **Create a `.env` file** (based on `.env.example`) and fill in your PostgreSQL credentials.

4. **Run the server**
```
node app.js
```

## API Endpoints

- GET `/users` – Retrieve all users
- GET `/users/:id` – Retrieve a specific user
- POST `/users` – Create a new user
- PUT `/users/:id` – Update a user
- DELETE `/users/:id` – Delete a user

Test using Postman or any REST client.