# 📊 Xeno Mini CRM Platform – SDE Internship Assignment 2025

Welcome to the Mini CRM Platform, built as part of the Xeno SDE Internship Assignment – 2025. This platform enables audience segmentation, personalized campaign delivery, and **AI-powered insights**, reflecting real-world CRM functionalities with a scalable architecture.

---

## 🚀 Features Overview

### 1. 🔁 Data Ingestion APIs
- Secure RESTful APIs to ingest customer and order data.
- Includes request validation and Swagger/Postman documentation.
- (Optional) Pub-sub pattern designed (mocked for scope).

### 2. 🎯 Campaign Creation UI
- Audience segmentation with dynamic rule builder (AND/OR logic).
- UI allows real-time audience size preview.
- Campaign history with delivery stats, sorted by most recent.

### 3. ✉️ Campaign Delivery & Logging
- Simulates message sending via dummy vendor API.
- 90% delivery success, 10% failure (randomized).
- Receives delivery receipts and updates communication log.

### 4. 🔐 Authentication
- Secure Google OAuth 2.0 integration.
- Only authenticated users can access CRM dashboard and create/view campaigns.

### 5. 🧠 AI Integration
- AI-powered message suggestions using OpenAI API.
- (Optional scope) Campaign performance summarization mock included.

---

## 🛠️ Tech Stack

| Layer         | Technology          |
|---------------|---------------------|
| Frontend      | React.js (Vite)     |
| Backend       | Node.js + Express   |
| Database      | MongoDB             |
| Authentication| Google OAuth 2.0    |
| AI Integration| OpenAI API          |
| Documentation | Postman + Swagger   |
| Dev Tools     | Vercel (optional), Render (optional) |

---

## 🧪 AI Features Breakdown

| Feature                              | Status    |
|--------------------------------------|-----------|
| AI-powered message suggestions       | ✅ Done    |
| Campaign performance summarization   | ✅ Partial |
| Natural language to segment rules    | ❌ Not implemented |
| Smart scheduling / Lookalike Gen.    | ❌ Not implemented |

You can simulate some advanced AI features with rule-based logic as shown in the code.

---

## 🔐 Authentication Flow

- Utilizes Google OAuth 2.0 via Firebase Auth.
- Session is stored securely; routes are protected using middleware.
- Logout option provided in the UI.

---

## 📐 Architecture Overview

```

Frontend (React)
↓
Backend (Express API)
↓
MongoDB (Data Storage)
↓
Dummy Vendor API ⇄ Delivery Receipt API
↓
Communication Log

* Optional AI Services (OpenAI) used on Campaign Creation UI

```

---

## 📦 Project Structure

```

XenoTechSolution/
│
├── backend/
│   ├── routes/
│   ├── controllers/
│   ├── models/
│   ├── utils/
│   └── index.js
│
├── frontend/
│   ├── components/
│   ├── pages/
│   ├── services/
│   └── App.jsx
│
├── .env.example
├── README.md
├── demo.mp4
└── postman\_collection.json


## 🚀 Deployment (Optional)

> This project is ready for deployment using:
- 🔷 [Render](https://render.com)
- 🔷 [Vercel](https://vercel.com)
- 🔷 [Railway](https://railway.app)

💡 To deploy:
```bash
# Backend
cd backend && npm install && npm start

# Frontend
cd frontend && npm install && npm run dev
````

---

## ⚙️ Local Setup Instructions

1. Clone the repository

```bash
git clone https://github.com/yourusername/xeno-crm-assignment.git
cd xeno-crm-assignment
```

2. Install dependencies

```bash
cd backend && npm install
cd ../frontend && npm install
```

3. Setup `.env` files
   Create a `.env` in both `frontend/` and `backend/` directories using `.env.example` as a reference.

4. Run the application

```bash
# Run backend
cd backend
npm run dev

# Run frontend
cd ../frontend
npm run dev
```

---

## ✅ Known Limitations

* Kafka/pub-sub architecture is not implemented; async simulation used instead.
* Only one AI use case fully implemented due to time constraints.
* Campaign delivery updates are handled individually (no batch consumer).
* No lookalike audience or auto-tagging logic yet.

---

## 📬 Submission Checklist

* [x] ✅ Public GitHub Repository
* [x] ✅ Demo Video (with explanation)
* [x] ✅ README with setup, architecture, tech & AI tools
* [x] ✅ Complete Codebase
* [ ] 🔄 Optional: Deployment Link (Add if hosted)

🙋‍♂️ Author
👨‍💻 Anwar Ansari
CSE Student, Chandigarh University
Email: [anwaransari46708@gmail.com]
