🛡️ JWT Based SPA Authentication (React + Node.js)
 ----

A complete JWT Authentication System built using:

React Single Page Application (SPA)

Node.js + Express backend

Login / Logout flow

Protected routes

JWT token storage

Secure API authentication

🚀 Features
----


✔ Login with email & password

✔ JWT token generated on backend

✔ Token stored on frontend

✔ Protected routes (without login → access denied)

✔ Profile data only for logged-in users

✔ Logout clears token

✔ Clean UI (centered login card)

🛠️ Tech Stack
----

🖥️ Frontend
--

React

React Router

Axios

Context API

🛠 Backend
--

Node.js

Express

JWT (jsonwebtoken)

CORS
---
📂 Project Structure
JWT-SPA-AUTH
 ├── backend
 │    ├── server.js
 │    └── package.json
 │
 └── frontend
      ├── src
      │   ├── App.js
      │   ├── api.js
      │   ├── AuthContext.js
      │   ├── ProtectedRoute.js
      │   └── pages
      │        ├── Login.js
      │        └── Profile.js
---
⚙️ Installation & Setup
--

1️⃣ Clone repository
git clone <repo-url>

2️⃣ Install backend dependencies
cd backend
npm install

3️⃣ Run backend server
npm run dev


Backend runs at:

http://localhost:5000

4️⃣ Install frontend dependencies
cd frontend
npm install

5️⃣ Run frontend
npm start


Frontend runs at:

http://localhost:3000

🔑 Demo Login Credentials
email: test@example.com
password: 123456

🔌 API Endpoints
🔹 POST /login

Request Body

{
  "email": "test@example.com",
  "password": "123456"
}


Response

{
  "token": "jwt_token_here"
}

🔹 GET /profile (Protected)

Headers

Authorization: Bearer <token>


Response

{
  "email": "test@example.com"
}

----
🔒 Authentication Flow (How it works)
----


1️⃣ User enters email/password
2️⃣ Frontend sends /login request
3️⃣ Backend verifies credentials
4️⃣ Backend returns JWT token
5️⃣ Token stored in localStorage
6️⃣ Protected pages check token
7️⃣ Logout removes token

----


🛑 Protected Route Logic
if token exists → allow page
if no token → redirect to /login

🧠 Why JWT?

✔ Stateless authentication
✔ No server session storage
✔ Perfect for SPA
✔ Easy token verification
✔ Works with any frontend

📚 What I Learned from this Project

During this project I learned:

🔹 How JWT works in real apps

🔹 Authentication vs Authorization

🔹 Building backend API using Node + Express

🔹 Generating & verifying JWT tokens

🔹 Connecting React with backend API

🔹 Protecting routes using ProtectedRoute

🔹 Using localStorage for token storage

🔹 Sending token via Axios headers

🔹 Redirecting after login/logout

🔹 Managing auth state via Context API

🔹 Designing clean login UI


🔹 Importance of error handling & validation

