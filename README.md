## About 

A RESTful API with authentication and authorization plus role based access created using Node.js, express.js framework.

## Tech stack
Node.js: JavaScript runtime.
Express: Web framework for Node.js. 
Sequelize: Promise-based ORM for Node.js.
PostgreSQL: Relational database system.
jsonwebtoken: For JWT creation and verification.
bcryptjs: For hashing passwords.
 
---

## Project Structure
![Structure screenshot](./structure.png)
 

---

## Setup Instructions

1. **Clone the repository:**
 ```bash
 git clone https://github.com/ChepkemoiPeris/Node.js-Express-PostgreSQL-Authentication-with-JWT.git
 ```
2. **Install dependencies:**

```bash
npm install
```
  
3. **Create a database:**
 
Ensure PostgreSQL is running and the database testdb is created. Then, start the server:

Then update app/config/db.config.js to match your database credentials. You can also update app/config/auth.config.js with your JWT secret key
 
4. **Start the development server:**

```bash
node server.js
```

### API Access
- Base URL: http://127.0.0.1:8080/
 
### Endpoints 

Public:

- GET  http://localhost:8080/api/test/all

Auth:

- POST  http://localhost:8080/api/auth/signup

- POST  http://localhost:8080/api/auth/signin

Authenticated:

- GET http://localhost:8080/api/test/mod

- GET http://localhost:8080/api/test/user

- GET http://localhost:8080/api/test/admin
  