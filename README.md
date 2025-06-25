# Ad Keyword Targeting App

A Java full stack project with spring boot framework and MySQL dB for backend and react and tailwindcss for frontend. It's a ad creation and searching application where you can Post ads and also Get ads based on your search. All the posted ads are stored in a MySQL database which can be retrieved at any time. 

## Backend
- Java 17
- Spring Boot
- MySQL
- REST API

## Frontend
- React.js
- Tailwind CSS
- Consumes REST API

## 📦 Local Setup

### 1. MySQL Setup
Create a database called `ad_db`. Update credentials in: backend/src/main/resources/application.properties

## How to Run (Local)

### Backend:
```bash
cd backend
./mvnw spring-boot:run
```

### Frontend:
```bash
cd frontend
npm install
npm start
```

HOSTED LINKS:
Frontend:
Backend: https://adapi-backend.onrender.com/

✅ Folder Structure
```bash
ad-keyword-targeting-app/
├── backend/
│   ├── src/
│   ├── pom.xml
│   ├── application.properties
│   └── render.yaml         ✅ (Render deploy config)
├── frontend/
│   ├── src/
│   ├── package.json
│   ├── tailwind.config.js
│   └── netlify.toml        ✅ (Netlify deploy config)
├── .gitignore              ✅
└── README.md
            ✅
```

🧪 API Usage
➕ Add Ad
```bash
POST /ads
```
🔍 Search Ads
```bash
GET /ads/search?keyword=laptop
```
