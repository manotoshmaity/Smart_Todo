📝 Smart ToDo API

A RESTful backend application for managing tasks efficiently with secure user authentication and CRUD operations.
Built using modern backend technologies following best practices.

🚀 Project Overview

The Smart ToDo API is a backend system that allows users to:

Register and authenticate securely

Create, read, update, and delete personal tasks

Store user and task data persistently in a NoSQL database

Interact with the API using RESTful endpoints

This project demonstrates backend architecture, API design, authentication, and database integration.

🧩 Core Features
🔐 User Authentication

User registration & login

JWT-based authentication

Protected routes for task operations

📌 Task Management

Create new tasks

Fetch all user-specific tasks

Update task details

Delete tasks

🗄 Database Integration

NoSQL database for storing users and tasks

Secure data handling with schema validation

🛠 Tech Stack
Backend

Node.js with Express.js
(or Python with FastAPI/Flask — based on implementation)

Database

MongoDB (NoSQL)

Authentication

JSON Web Tokens (JWT)

API Documentation

Swagger UI / Postman Collection

📂 Project Structure
smart-todo-api/
│
├── controllers/
│   ├── authController.js
│   └── taskController.js
│
├── models/
│   ├── User.js
│   └── Task.js
│
├── routes/
│   ├── authRoutes.js
│   └── taskRoutes.js
│
├── middleware/
│   └── authMiddleware.js
│
├── config/
│   └── db.js
│
├── app.js
├── package.json
├── .env
└── README.md

🔗 API Endpoints
Authentication
Method	Endpoint	Description
POST	/auth/register	Register a new user
POST	/auth/login	Login user & generate JWT
Tasks (Protected Routes)
Method	Endpoint	Description
POST	/tasks	Create a new task
GET	/tasks	Get all tasks
PUT	/tasks/:id	Update a task
DELETE	/tasks/:id	Delete a task
🔑 Authentication Flow

User logs in and receives a JWT token

Token must be sent in headers:

Authorization: Bearer <token>


Access granted to protected routes

🧪 API Documentation

📬 Postman Collection: (attached in repository)
OR

📘 Swagger Documentation:

http://localhost:PORT/docs

⚙️ Environment Variables

Create a .env file in the root directory:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key

▶️ Installation & Setup
# Clone repository
git clone https://github.com/your-username/smart-todo-api.git

# Navigate to project
cd smart-todo-api

# Install dependencies
npm install

# Start server
npm run dev


Server will run on:

http://localhost:5000

🎯 Learning Outcomes

RESTful API design

JWT authentication

MongoDB schema modeling

Middleware implementation

Secure backend architecture

👨‍💻 Author

Arun Maity
CSE Student | MERN Stack Developer
📌 Backend Project – Smart ToDo API

