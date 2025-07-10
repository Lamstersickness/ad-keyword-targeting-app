# 🎯 Ad Keyword Targeting App – Full Stack Project

A full-stack web application that allows users to create and search advertisements based on keywords, complete with image uploads. Built using **Spring Boot** for the backend and **React.js + Tailwind CSS** for the frontend.

---

## 🔗 Live Demo

- 🔵 **Frontend**: [https://your-vercel-app.vercel.app](https://your-vercel-app.vercel.app](https://ad-frontend-mu.vercel.app/)
- 🟢 **Backend API**: [https://adapi-backend.onrender.com/api](https://adapi-backend.onrender.com/api)

---

## 🧰 Tech Stack

| Frontend            | Backend             | Database          | Hosting           |
|---------------------|---------------------|-------------------|-------------------|
| React.js            | Java 17 + Spring Boot | MySQL (Railway)   | Vercel (FE), Render (BE) |
| Axios + Tailwind CSS| Spring Data JPA     | Cloud Hosted      | Railway + GitHub  |

---

## ✨ Features

- 📤 **Create ads** with title, description, keywords, and image upload
- 🔍 **Search ads** by keyword (exact or partial matches)
- 📷 **Upload images** with real-time preview
- 🔗 **RESTful API** integration between frontend and backend
- 🌐 Deployed and live with full CORS and environment variable support

---

## 📸 Screenshots

> _(Add your screenshots here in a `screenshots/` folder)_

- ![Create Ad](screenshots/create-ad.png)
- ![Search Results](screenshots/search-results.png)

---

## 🚀 Getting Started

### 🔧 Backend Setup (Spring Boot)

1. Clone the backend:
   ```bash
   git clone https://github.com/yourusername/adapi-backend.git
   cd adapi-backend

    Add application.properties:

spring.datasource.url=jdbc:mysql://your-railway-db-url
spring.datasource.username=your-db-user
spring.datasource.password=your-db-password
spring.jpa.hibernate.ddl-auto=update

Run the app:

    ./mvnw spring-boot:run

📍 Base URL: https://adapi-backend.onrender.com/api
💻 Frontend Setup (React)

    Clone the frontend:

git clone https://github.com/yourusername/ad-frontend.git
cd ad-frontend

Add .env file:

REACT_APP_BACKEND_URL=https://adapi-backend.onrender.com/api

Install and run:

    npm install
    npm start

📍 Frontend URL: https://your-vercel-app.vercel.app
📬 API Endpoints
Method	Endpoint	Description
POST	/api/ads	Create new ad
GET	/api/ads/search?keyword=xyz	Search ads by keyword

Note: Accepts multipart/form-data for image uploads.
🛡️ CORS Configuration

Backend allows CORS for:

    http://localhost:3000

    https://your-vercel-app.vercel.app

    Configured via WebConfig.java using CorsRegistry.

🧠 Project Structure
```bash

ad-keyword-targeting-app/
├── adapi-backend/         → Spring Boot backend
└── ad-frontend/           → React frontend
```
🧑‍💻 Author

Archit Kumar

    GitHub: @Lamstersickness

    LinkedIn: Archit Kumar

📌 Notes

    Backend hosted on Render (free tier)

    MySQL DB hosted via Railway

    Frontend hosted on Vercel

    Includes .env support and full separation of concerns

📄 License

MIT License — use it, fork it, build on it!
