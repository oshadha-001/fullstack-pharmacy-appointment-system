---

# 💊 Appointment Booking System for Pharmacy

A full-stack web application built to help a **Senior Pharmacist** efficiently manage patient appointments. The system allows patients to book appointments online or physically, while providing an admin dashboard for managing bookings, approvals, and time slots.

---

## 🚀 Features

### 👤 Patient

* Register and login securely (JWT Authentication)
* Book **Online Appointments** (8:00 AM – 12:00 PM)
* Book **Physical Appointments** (12:00 PM – 6:00 PM)
* View appointment history and status

### 🧑‍⚕️ Pharmacist (Admin)

* Secure login with pre-created credentials
* Dashboard to view all appointments
* Filter appointments by **date** and **type**
* Approve or reject appointment requests
* Manage slot availability:

  * Enable/Disable slots
  * Set maximum number of patients per slot

---

## 🛠️ Tech Stack

### Frontend

* React (Vite)
* Tailwind CSS
* Axios
* React Router
* Lucide Icons

### Backend

* Node.js
* Express.js
* JWT (Authentication)
* Bcrypt (Password Hashing)

### Database

* MySQL

---

## 📁 Project Structure

```
project-root/
│
├── client/         # Frontend (React + Vite)
├── server/         # Backend (Node.js + Express)
├── schema.sql      # Database schema
└── README.md
```

---

## ⚙️ Setup Instructions

### 1️⃣ Database Setup

1. Open MySQL Workbench or CLI
2. Run the `schema.sql` file
3. Use the following configuration:

   * Host: `localhost`
   * User: `root`
   * Password: `12345`
   * Port: `3306`

---

### 2️⃣ Backend Setup

```bash
cd server
npm install
npm start
```

📌 Make sure `.env` file has correct database credentials:

```
DB_HOST=localhost
DB_USER=root
DB_PASS=12345
DB_NAME=appointment_system
JWT_SECRET=your_secret_key
```

---

### 3️⃣ Frontend Setup

```bash
cd client
npm install
npm run dev
```

---

## 🔐 Admin Credentials

| Field    | Value        |
| -------- | ------------ |
| NIC      | 000000000000 |
| Password | admin123     |

---

## 📌 API Overview (Basic)

### Auth Routes

* `POST /api/auth/register`
* `POST /api/auth/login`

### Appointment Routes

* `POST /api/appointments`
* `GET /api/appointments/user`
* `GET /api/appointments/admin`
* `PUT /api/appointments/:id/status`

---

## ✨ Key Highlights

* 🔐 Secure authentication with JWT
* 📅 Smart time-slot based booking system
* ⚡ Fast and responsive UI using Tailwind CSS
* 📊 Admin dashboard with filtering & controls
* 🧩 Modular and scalable architecture

---

## 🎯 Use Cases

* Pharmacy appointment management
* Clinic scheduling systems
* University full-stack projects
* Learning project for MERN-style architecture (with MySQL)

---

## 📷 Future Improvements

* Email/SMS notifications
* Payment integration
* Role-based access control
* Calendar view integration
* Docker deployment

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repo and submit a pull request.

---

## 📄 License

This project is licensed under the MIT License.

---
