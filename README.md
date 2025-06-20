# CodePractice - Web App (v1)

CodePractice is a web-based platform aimed at helping developers practice coding questions and improve their skills. The first iteration focuses solely on **code-based practice** with assistance powered by the **Gemini API**.

This project is structured with a **Next.js frontend** and a **Spring Boot backend**, designed to support a future transition into a microservice-based architecture.

---

## 🚀 Features (v1)

- Browse and select coding problems
- Submit code to get AI-generated feedback (via Gemini API)
- Simple, minimal UI (no login/signup required)
- API-first architecture to support future features

---

## 🧱 Tech Stack

| Layer     | Technology   |
|-----------|--------------|
| Frontend  | Next.js (React, deployed on Vercel) |
| Backend   | Spring Boot (REST APIs, deployed independently) |
| AI Assist | Gemini API |
| Database  | None (Static data/in-memory for now) |

---

## 🗂️ Project Structure

/frontend-codepractice  
  └── pages/  
  └── components/  
  └── utils/  
  └── public/  
  └── ...

/backend-codepractice  
  └── src/  
    └── main/  
      └── java/  
      └── resources/  
    └── ...

---

## 🔌 API Integration

- Backend integrates with **Gemini API** to provide:
 - Code hints  
 - Explanations  
 - Suggestions or bug help  
- Frontend communicates with backend via REST API endpoints.

---

## ⚙️ How to Run (Locally)

### Frontend (Next.js)
```
cd frontend-codepractice
npm install
npm run dev
```

### Backend (Spring Boot)

```
cd backend-codepractice
./mvnw spring-boot:run
```

---

## 🛠️ Planned Enhancements (Post v1)

- User authentication (email/password, OAuth)
- Code execution via Judge0 or similar APIs
- Support for MCQs, Math, Essay Writing
- Admin dashboard for adding/updating content
- MongoDB/PostgreSQL integration
- Microservices (Python/Java) for scalable backend

---

## 📌 Author & License