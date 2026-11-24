# 🏠 MERN Booking App

This is a full-stack **Booking Application** built with the **MERN stack** (**MongoDB**, **Express.js**, **React**, **Node.js**). The project demonstrates how to build a real-world booking platform with user authentication, RESTful API routes, and a modern, responsive frontend UI.

---

## 📌 Features

- **Full-Stack Architecture:** End-to-end application using MongoDB for data storage, Express.js and Node.js for the backend server, and React for the frontend.
- **User Authentication:** JSON Web Token (JWT)-based login and registration, with bcrypt-hashed passwords.
- **Booking Management:** Create, view, and manage bookings tied to user accounts.
- **Property Listings:** Add and display places with descriptions and images.
- **Responsive UI:** Built with React and Tailwind CSS for a clean, mobile-friendly design.
- **RESTful API:** Backend endpoints for CRUD operations and secure client–server communication.

---

## 🚀 Technologies Used

**Frontend:**
- React.js
- React Router
- Tailwind CSS
- Axios

**Backend:**
- Node.js
- Express.js
- Mongoose
- MongoDB
- JSON Web Tokens (JWT)
- Bcrypt.js (for password hashing)

---

## 🗃️ Database

- **MongoDB** for storing users, places, and booking data.
- **Mongoose** for schema design and database interaction.

---

## 🛠️ Run It Locally

1. Copy `api/.env.example` to `api/.env` and fill it in: a MongoDB connection string, a long random
   `JWT_SECRET` (the file shows a one-line command that generates one) and, for photo uploads, S3 keys.
2. Copy `client/.env.example` to `client/.env`.
3. Start the API and the client in two terminals:
   ```bash
   cd api && yarn install && node index.js        # http://127.0.0.1:4000
   cd client && yarn install && yarn dev          # http://127.0.0.1:5173
   ```

The API only accepts browser requests from `http://127.0.0.1:5173` (the CORS origin in `api/index.js`).
`.env` files are gitignored. On Vercel, set `MONGO_URL`, `JWT_SECRET`, the S3 keys and `VITE_API_BASE_URL=/api` as
project environment variables.
