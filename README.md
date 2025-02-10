# Job Search API - Backend

This is the backend for the Job Search application, built using **Node.js**, **Express**, and **MongoDB**.

## Features
- User authentication (Register/Login with JWT)
- Swagger documentation

---

## Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/RaznoOleg/job-search-server.git
cd job-search-server
```

### 2️⃣ Install Dependencies
```bash
npm install
```

### 3️⃣ Create `.env` File
Create a `.env` file in the root directory and add the following:
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

### 4️⃣ Start the Server
#### Development Mode
```bash
npm run dev
```
#### Production Mode
```bash
npm start
```

---

## API Documentation (Swagger)
After running the server, visit:
```
http://localhost:5000/api-docs
```
This will open the Swagger UI with full API documentation.

---

## API Endpoints

### **Auth Routes**
| Method | Endpoint         | Description          |
|--------|----------------|----------------------|
| POST   | `/api/auth/register` | Register new user  |
| POST   | `/api/auth/login`    | Login user & get JWT |

---
## Deployment
### **1️⃣ Connect MongoDB (Atlas)**
- Go to [MongoDB Atlas](https://www.mongodb.com/atlas/database).
- Create a new cluster and get the connection string.
- Add the connection string to `.env` as `MONGO_URI`.
  
### **2️⃣ Deploy Backend to Render**
- Push your code to GitHub.
- Go to [Render](https://render.com/), create a new Web Service.
- Select your GitHub repository and set up environment variables.
- Deploy the service.
---

## Technologies Used
- **Node.js** + **Express.js** - Backend framework
- **MongoDB** + **Mongoose** - Database
- **JWT** - Authentication
- **Swagger** - API documentation
- **Render** - Deployment

---

## License
This project is open-source and available under the [MIT License](LICENSE).

