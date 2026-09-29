# Ledger API

A backend REST API for a Ledger Management application, built with **Node.js, Express.js, and MongoDB**.

The project provides a structured backend for managing users, authentication, ledger-related data, and application services.

---

## 🚀 Tech Stack

| Technology        | Purpose                   |
| ----------------- | ------------------------- |
| **Node.js**       | Backend runtime           |
| **Express.js**    | REST API framework        |
| **MongoDB**       | Database                  |
| **Mongoose**      | MongoDB ODM               |
| **JWT**           | Authentication            |
| **bcrypt**        | Password hashing          |
| **Cookie Parser** | Cookie handling           |
| **Nodemailer**    | Email services            |
| **dotenv**        | Environment configuration |

---

## ✨ Features

* 🔐 User authentication
* 🔑 JWT-based authentication
* 🔒 Password hashing
* 🍪 Secure cookie handling
* 👤 User management
* 📒 Ledger management
* 🗄️ MongoDB database integration
* 📧 Email service integration
* 🛡️ Protected API routes
* ⚙️ Environment-based configuration
* 🧩 Modular backend architecture

---

## 🏗️ Architecture

The backend follows a modular structure to keep application logic organized and maintainable.

```text
ledger-api/
│
├── src/
│   ├── config/
│   │   └── db.js
│   │
│   ├── controllers/
│   │
│   ├── middleware/
│   │
│   ├── models/
│   │
│   ├── routes/
│   │
│   ├── services/
│   │
│   └── App.js
│
├── .env
├── .gitignore
├── package.json
├── package-lock.json
└── server.js
```

---

## 🔄 Application Flow

```text
Client Application
       │
       ▼
   REST API
       │
       ▼
 Express.js
       │
       ├── Authentication
       ├── Authorization
       ├── Validation
       ├── Business Logic
       │
       ▼
    Mongoose
       │
       ▼
    MongoDB
```

---

## 🔐 Authentication Flow

The application uses token-based authentication.

```text
User
 │
 ▼
Login / Register
 │
 ▼
Express API
 │
 ▼
Validate Credentials
 │
 ▼
bcrypt Password Verification
 │
 ▼
Generate JWT
 │
 ▼
Authentication Cookie
 │
 ▼
Protected API Requests
```

---

## 📡 API Design

The backend is designed around RESTful API principles.

Example API structure:

```text
/api/auth
/api/users
/api/ledger
```

Typical operations include:

```text
POST    /api/auth/register
POST    /api/auth/login
POST    /api/auth/logout

GET     /api/users
GET     /api/users/:id

GET     /api/ledger
POST    /api/ledger
GET     /api/ledger/:id
PUT     /api/ledger/:id
DELETE  /api/ledger/:id
```

> API routes may change as the application evolves.

---

## ⚙️ Environment Variables

Create a `.env` file in the project root.

```env
PORT=3000

MONGODB_URI=your_mongodb_connection_string

JWT_SECRET=your_jwt_secret

EMAIL_USER=your_email
EMAIL_PASSWORD=your_email_password
```

Never commit your `.env` file to GitHub.

---

## 🛠️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/rushi0612/ledger-api.git
```

### 2. Navigate to the project

```bash
cd ledger-api
```

### 3. Install dependencies

```bash
npm install
```

### 4. Configure environment variables

Create:

```text
.env
```

and add the required configuration.

### 5. Start development server

```bash
npm run dev
```

### 6. Start production server

```bash
npm start
```

The API will run on:

```text
http://localhost:3000
```

---

## 📦 Available Scripts

```bash
npm run dev
```

Starts the development server using Nodemon.

```bash
npm start
```

Starts the Node.js production server.

---

## 🧪 API Testing

You can test the API using:

* Postman
* Thunder Client
* Insomnia

Recommended testing flow:

```text
Register
   ↓
Login
   ↓
Receive Authentication
   ↓
Access Protected Routes
   ↓
Create Ledger Data
   ↓
Read Ledger Data
   ↓
Update Ledger Data
   ↓
Delete Ledger Data
```

---

## 🔒 Security

The project implements backend security practices including:

* Password hashing with bcrypt
* JWT-based authentication
* Protected routes
* Environment variables for secrets
* Cookie-based authentication handling
* Server-side validation

---

## 📈 Future Improvements

* [ ] Role-based access control
* [ ] Advanced request validation
* [ ] API documentation with Swagger
* [ ] Automated testing
* [ ] Rate limiting
* [ ] Request logging
* [ ] API versioning
* [ ] Docker support
* [ ] CI/CD pipeline
* [ ] Production deployment

---

## 🔗 Project Ecosystem

This backend can be connected with a React frontend to create a complete full-stack application.

```text
React.js
    │
    ▼
REST API
    │
    ▼
Node.js + Express.js
    │
    ▼
MongoDB
```

### Full-Stack Stack

**React.js → Node.js → Express.js → MongoDB**

---

## 👨‍💻 Author

**Rushikesh Patil**

Computer Science Engineer | Full-Stack Developer

Focused on building applications using:

**React.js · Node.js · Express.js · MongoDB**

GitHub:
https://github.com/rushi0612

---

## ⭐ If you find this project useful

Consider giving the repository a ⭐ on GitHub.
