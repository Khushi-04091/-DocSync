<div align="center">
  
# PRESCRIPTO 👨‍⚕️🏥🤒
</div>

Prescripto is a full-stack appointment booking system for clinics and hospitals, supporting three user roles: Patients, Doctors, and Admins. It streamlines healthcare appointment management, offering a seamless experience for users and robust controls for providers and administrators.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [System Architecture](#system-architecture)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Environment Variables](#environment-variables)
- [Running the Project](#running-the-project)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## Overview

Prescripto is a modern healthcare appointment platform that connects patients with doctors and provides an admin dashboard for clinic management. The system is designed for scalability, security, and ease of use, making it suitable for clinics, hospitals, and telemedicine providers.

---

## Features

### For Patients
- Register, login, and manage profile
- Browse doctors by specialty, availability, and location
- Book, view, and cancel appointments
- View appointment history

### For Doctors
- Secure login and profile management
- Manage availability and appointment slots
- View and manage upcoming appointments
- Track earnings and patient statistics

### For Admins
- Secure admin login
- Manage doctor profiles and availability
- View and manage all appointments
- Access dashboard analytics

---

## System Architecture

```
clientside/   # Patient-facing frontend (React + Vite)
admin/        # Admin & Doctor dashboard frontend (React + Vite)
backend/      # REST API backend (Node.js + Express + MongoDB)
```

- **Frontend:** Two separate React apps for patients and admin/doctor dashboards.
- **Backend:** Node.js REST API with JWT authentication, MongoDB for data storage, and Cloudinary for image uploads.
- **Deployment:** Ready for Vercel or similar platforms.

---

## Tech Stack

- **Frontend:** React, Vite, Tailwind CSS, Axios, React Router
- **Backend:** Node.js, Express, MongoDB, Mongoose, JWT, Cloudinary, Multer
- **DevOps:** Vercel (for frontend and backend), dotenv for environment management

---

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- npm or yarn
- MongoDB instance (local or cloud)
- Cloudinary account (for image uploads)

### Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/Khushi-04091/PrescriptoPanel.git
   cd PrescriptoPanel
   ```

2. **Install dependencies for each app:**
   ```sh
   cd backend && npm install
   cd ../admin && npm install
   cd ../clientside && npm install
   ```

---

### Environment Variables

Create a `.env` file in each directory as shown below:

#### `backend/.env`
```
PORT=4000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
ADMIN_EMAIL=admin@example.com
ADMIN_PASSWORD=your_admin_password
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```

#### `admin/.env` and `clientside/.env`
```
VITE_API_URL=http://localhost:4000/api
```
> For production, use your deployed backend URL.

---

## Running the Project

**Start the backend:**
```sh
cd backend
npm run dev
```

**Start the admin dashboard:**
```sh
cd admin
npm run dev
```

**Start the clientside (patient app):**
```sh
cd clientside
npm run dev
```

- Admin dashboard: [http://localhost:5174](http://localhost:5174)
- Patient app: [http://localhost:5173](http://localhost:5173)
- Backend API: [http://localhost:4000](http://localhost:4000)

---

## Deployment

- The project is ready for deployment on [Vercel](https://vercel.com/) or similar platforms.
- Use the provided `vercel.json` files for routing and build configuration.
- Set environment variables in your deployment dashboard as per the `.env` files.

---

## Contributing

We welcome contributions from everyone!

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

---

<div align="center">

# User Dashboard 👤:
![UI](https://github.com/user-attachments/assets/f953ae81-7cc8-4b6b-8101-c3aa47d0aada)

<br /><hr /><br />

# Doctor Panel 🧑‍⚕️:
![doctor-panel](https://github.com/user-attachments/assets/ed488e0a-a61a-4cb1-b95a-f19b9135f9b2)

<br /><hr /><br />

# Admin Panel 🎯:
![admin-panel](https://github.com/user-attachments/assets/5479b3c0-0663-41ec-9fe2-17434249155c)

</div>

---

## License 📝

This project is distributed under [MIT license](https://github.com/elyse502/prescripto/blob/main/LICENSE). Enjoy! 🎉

---

*For any questions, issues, or feature requests, please open an issue on GitHub.*
