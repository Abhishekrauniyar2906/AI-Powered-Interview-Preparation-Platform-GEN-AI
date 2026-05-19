# AI-Powered Interview Preparation Platform

An AI-driven interview preparation platform built using the MERN stack and the **Gemini-3-Flash-Preview Model** to help users prepare for technical interviews intelligently. The platform analyzes resumes, evaluates candidate-job compatibility, generates interview questions, identifies skill gaps, and creates personalized preparation roadmaps.

---

# Features

- JWT-based Authentication & Authorization
- Resume PDF Upload & Parsing
- AI-Powered Interview Question Generation
- Resume Match Score Evaluation
- Skill-Gap Analysis & Preparation Roadmap
- ATS-Friendly Resume PDF Generation
- Structured AI Responses using Zod Validation
- RESTful API Architecture
- Secure File Upload Handling using Multer

---

# Tech Stack

## Frontend
- React.js
- Tailwind CSS
- Context API
- Axios

## Backend
- Node.js
- Express.js
- MongoDB
- REST APIs
- JWT Authentication
- Multer

## Generative AI
- Gemini-3-Flash-Preview Model
- Structured AI Response Generation
- Resume Analysis

## Tools & Libraries
- Puppeteer
- Zod
- Postman
- Git & GitHub

---

# System Architecture

```txt
Frontend (React.js)
        ↓
REST API Requests
        ↓
Express.js Backend
        ↓
Authentication Middleware
        ↓
Resume PDF Parsing
        ↓
Gemini-3-Flash-Preview Model
        ↓
Structured AI Response
        ↓
MongoDB Storage
        ↓
Frontend Dashboard
```

---

# How It Works

1. User registers and logs into the platform.
2. User uploads resume PDF and enters job description.
3. Backend extracts resume content using PDF parsing.
4. Resume content and job description are sent to the Gemini AI model.
5. AI generates:
   - Interview Questions
   - Match Score
   - Skill-Gap Analysis
   - Preparation Roadmap
6. AI-generated ATS resume is converted into downloadable PDF using Puppeteer.
7. Generated reports are stored in MongoDB for future access.

---

# API Routes

## Authentication Routes

| Method | Route | Description |
|---|---|---|
| POST | `/api/auth/register` | Register new user |
| POST | `/api/auth/login` | Login user |
| GET | `/api/auth/profile` | Get user profile |

---

## Interview Routes

| Method | Route | Description |
|---|---|---|
| POST | `/api/interview/generate` | Generate AI interview report |
| GET | `/api/interview/reports` | Fetch all interview reports |
| GET | `/api/interview/:id` | Fetch single interview report |
| POST | `/api/interview/upload-resume` | Upload resume PDF |
| POST | `/api/interview/generate-resume` | Generate ATS-friendly resume PDF |

---

# Environment Variables

Create a `.env` file in the root directory and add:

```env
PORT=5000
MONGO_URI=your_mongodb_connection
JWT_SECRET=your_jwt_secret
GOOGLE_GENAI_API_KEY=your_gemini_api_key
```

---

# Installation & Setup

## Clone Repository

```bash
git clone https://github.com/your-username/project-name.git
```

## Install Dependencies

### Frontend

```bash
cd frontend
npm install
npm run dev
```

### Backend

```bash
cd backend
npm install
npm start
```

---

# Project Structure

```txt
project-root/
│
├── frontend/
│   ├── src/
│   ├── components/
│   ├── pages/
│   └── context/
│
├── backend/
│   ├── controllers/
│   ├── routes/
│   ├── middleware/
│   ├── models/
│   ├── services/
│   └── utils/
│
└── README.md
```

---

# Key Learning Outcomes

- Full-Stack Application Development
- REST API Design
- Authentication & Authorization
- File Upload Handling using Multer
- Generative AI Integration
- Structured AI Output Validation
- Dynamic PDF Generation
- Backend Architecture & Workflow Design

---

# Future Improvements

- AI Mock Interview System
- Voice-Based Interview Simulation
- Company-Specific Interview Preparation
- RAG-Based Contextual AI Responses
- AI Performance Analytics Dashboard



