[Log Entry - Iteration 1: Flow Design and Tasks]

🗓️ Date: [Insert Today's Date]
🎯 Goal: Implement an interactive practice flow where the user chooses a topic → selects theory/code → sees a coding interface with AI-powered review and optional code execution.

---

✅ FUNCTIONALITY FOR THIS ITERATION

1. User selects a **topic** (e.g., "coding").
2. System asks: **Theory or Code Practice?**
3. If "Code" is selected:
    - Show question page with:
        - Coding problem at the top
        - Code editor (e.g., Monaco)
        - Side panel: Difficulty level
        - Buttons: "Review Code" (via Gemini), "Execute Code" (TBD)

---

🖥️ FRONTEND TASKS (Next.js)

- [ ] **Topic Selection Page**
    - Dropdown or list of topics (hardcoded or dummy JSON)
    - On selection, navigate to choice screen

- [ ] **Mode Selection Page**
    - Buttons or cards: [Theory] [Code Practice]

- [ ] **Code Practice Page**
    - Show question at the top
    - Embed code editor (Monaco or similar)
    - Side panel:
        - Selected difficulty (label or dropdown)
    - Buttons:
        - "Review Code" → sends request to backend
        - "Execute Code" → placeholder logic for now (can use dummy output)

- [ ] **UI/UX**
    - Use Tailwind or simple CSS
    - Responsive layout with editor + sidebar

---

⚙️ BACKEND TASKS (Spring Boot)

- [ ] Endpoint: `POST /api/review-code`
    - Input: code, questionId, difficulty
    - Process:
        - Generate prompt for Gemini
        - Call Gemini API
        - Return response
    - Output: feedback/suggestions from Gemini

- [ ] (Optional) Endpoint: `POST /api/execute-code`
    - For now, return dummy output (can integrate Judge0 later)

- [ ] Store questions in memory (as JSON list or service)
    - Fields: id, title, description, difficulty, tags

- [ ] Handle API key for Gemini via environment config

---

🧠 AI (Gemini) Integration

- [ ] Use Gemini to review the user’s code
    - Prompt = question context + code + instructions for feedback
- [ ] Return structured response (summary, improvements)

---

🚀 DEPLOYMENT PLAN

- Frontend → Vercel
- Backend → Render / Railway
- Configure environment-based URLs

---

📌 REMARKS

- No login/auth for now
- Focus on flow + core logic
- Keep placeholder for future code execution
- Ensure backend prompt logic is reusable and decoupled

[End of Log Entry]
s