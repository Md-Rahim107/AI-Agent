## SAAS

GadgetGrid eliminates every manual step in running an online store. Orders flow via webhook into Google Sheets instantly. A RAG chatbot (Qdrant + Gemini) handles customer queries; when humans are needed, it collects contacts and pings the team on Telegram. A Telegram AI agent manages delivery status with plain-language commands. A dedicated error workflow logs failures with full stack traces for silent monitoring.

---

### 1. Message Processing Workflow

Filters whether the incoming message is a **file** or **text**:

- **If file** → Uploaded to Qdrant as knowledge for the chatbot  
- **If text** → Treated as a command for the Telegram bot  

![Message Processing Workflow](https://github.com/user-attachments/assets/807628f9-3002-48d2-a50e-7858a3f85845)

---

### 2. RAG System

Handles intelligent responses using retrieval-augmented generation.

![RAG System](https://github.com/user-attachments/assets/be4c39f5-e071-464a-b29d-96bbdab9efae)

---

### 3. Order Automation Workflow

Automatically adds orders from the website into Google Sheets.

![Order Workflow](https://github.com/user-attachments/assets/6a0dc8de-0d11-4438-b1e5-5c8d11148736)

---

### 4. Error Workflow

Logs failures with full stack traces for monitoring and debugging.

![Error Workflow](https://github.com/user-attachments/assets/4b6c5699-1d20-4443-bf0a-cbb1fa1f3312)
