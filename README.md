# 🌍 PolyglotConnect Backend

PolyglotConnect is a culturally inspired language learning platform designed to help users learn and connect with Cameroonian indigenous languages. This repository hosts the backend API built with [NestJS](https://nestjs.com/), [Prisma](https://www.prisma.io/), and [PostgreSQL](https://www.postgresql.org/).

---

## 🚀 Features

- 🔐 JWT-based Authentication
- 🗣️ Language & Dialect Management
- 👨‍🏫 Tutor & Learner Profiles
- 🗓️ Booking and Scheduling System
- 🎥 Lesson & Media Content Management
- ⚙️ Admin Dashboard APIs
- 🌍 Internationalization (i18n) Support
- 🧩 Prisma ORM with PostgreSQL
- 🐳 Docker Support for Dev & Production
- 📘 Swagger-powered RESTful API Documentation

---

## 🛠️ Tech Stack

| Category         | Tech                            |
|------------------|----------------------------------|
| **Framework**    | NestJS (TypeScript)             |
| **ORM**          | Prisma                          |
| **Database**     | PostgreSQL (Hosted via Railway) |
| **Authentication** | JWT + Bcrypt                 |
| **API Docs**     | Swagger (OpenAPI)               |
| **DevOps**       | Docker, GitHub Actions (CI/CD)  |
| **Hosting**      | Heroku                          |

---

## 📁 Project Structure

src/

├── auth/ # Authentication (JWT, Guards, Strategies)

├── users/ # User module

├── languages/ # Languages and dialects

├── lessons/ # Lessons, media files, content

├── bookings/ # Bookings and scheduling

├── common/ # Shared utilities (guards, interceptors, etc.)

├── prisma/ # Prisma service and hooks

├── main.ts # App entry point

└── app.module.ts # Root module

---

## 📦 Getting Started

### 1. Clone the Repository


git clone https://github.com/polyglotconnect/backend.git
cd backend

### 2. Install Dependencies
npm install

### 3. Environment Setup
Create a .env file in the root directory and add the following environment variables:

#### Database
DATABASE_URL=postgresql://youruser:yourpassword@localhost:5432/polyglotconnect

#### JWT
JWT_SECRET=your_jwt_secret
JWT_EXPIRES_IN=3600s

#### Prisma
SHADOW_DATABASE_URL=postgresql://youruser:yourpassword@localhost:5432/polyglotconnect_shadow

#### App
PORT=3000

### 4. Prisma Setup
Generate the Prisma client:
npx prisma generate

Run database migrations:
npx prisma migrate dev --name init

### 5. Start Development Server
npm run start:dev
Your backend server will run at:
👉 http://your_server_ip:3000


🧪 Running Tests
npm run test          # Unit tests
npm run test:e2e      # End-to-end tests
npm run test:watch    # Watch mode


### 📄 License
This project is licensed under the MIT License.

### 🙌 Acknowledgments
PolyglotConnect is inspired by the need to preserve and promote African linguistic diversity through digital innovation. Special thanks to all contributors and cultural consultants.

### 🙋 Contributions
We are currently not accepting external contributions while the project is under active development. Thank you for your interest and understanding.

### 💬 Stay Connected
For updates or partnership opportunities, feel free to reach out via our official contact channels.
