# practice-seth - Web App (v1)

**practice-seth** is a web-based learning platform designed to help users improve their skills through structured practice. The first iteration focuses on **coding practice**, with AI-powered feedback provided by the **Gemini API**.

This version includes a guided flow: select a topic → choose practice type → solve problems in an editor → get AI feedback.

---

## 🚀 Features (v1)

- Select a **topic** (e.g., Coding)
- Choose between **Theory** or **Code Practice**
- For Code Practice:
  - View coding problem
  - Solve it in an in-browser code editor
  - Choose difficulty level (shown in sidebar)
  - Click **Review Code** to get AI feedback
  - Click **Execute Code** (optional placeholder)

---

## 🧱 Tech Stack

| Layer     | Technology   |
|-----------|--------------|
| Frontend  | Next.js (deployed on Vercel) |
| Backend   | Spring Boot (REST APIs, deployed independently) |
| AI Assist | Gemini API |
| Database  | None (Static/dummy data used for now) |

---

## 🗂️ Project Structure

```
/frontend-practice-seth
├── pages/
├── components/
├── utils/
├── public/
/backend-practice-seth
└── src/
└── main/
├── java/
└── resources/
```

---

## 🔌 API Integration

- The backend integrates with **Gemini API** to provide:
  - Code reviews
  - Suggestions or improvements
- The frontend interacts with the backend through REST APIs.

---

## ⚙️ How to Run (Locally)

### Frontend (Next.js)
```bash
cd frontend-practice-seth
npm install
npm run dev
```

### Backend (Spring Boot)
```bash
cd backend-practice-seth
./mvnw spring-boot:run
```

## 🛠️ Planned Enhancements (Post v1)

    Code execution via Judge0 or similar service

    User authentication (email/password, OAuth)

    Additional content types: MCQs, Essay Writing, Math, etc.

    Admin panel for content management

    Persistent storage with MongoDB or PostgreSQL

    Microservices for language-specific backends (Java, Python, etc.)




