# 🤖 SensAi – AI Career Coach Platform

**SensAi** is a full-stack AI-powered career coaching platform built with **Next.js 13+**, **Prisma**, **Clerk**, and Google’s **Gemini API**. It provides intelligent resume building, mock interview prep, real-time salary insights, and personalized cover letters — all within a sleek, modern interface using **Shad CN UI**.

> 🧠 Your AI-powered career assistant — from resume to recruitment.

---

## 🚀 Features

### 🧑‍💼 Career Dashboard
- Personalized insights based on industry, experience, and skills
- Weekly updated growth/salary trends via scheduled cron jobs (Inest)

### 📄 AI Resume Builder
- ATS-optimized content generated by Gemini
- Markdown editor + PDF export for professional output

### 🗣️ Mock Interviews
- Role-specific questions
- AI-generated feedback and improvement suggestions
- Performance tracking with charts

### ✍️ Cover Letter Generator
- Upload job description → receive tailored, polished letter

### 🔐 Seamless Authentication (Clerk)
- Google OAuth, secure sessions, and user profile management

### 🎨 Modern UI/UX with Shad CN
- Responsive design
- Light/Dark mode toggle
- Accessible form inputs, modals, buttons, etc.

---

## 🧰 Tech Stack

| Category      | Tech                             |
|---------------|----------------------------------|
| Frontend      | Next.js 13+, React, Tailwind CSS |
| UI Components | Shad CN UI                       |
| Backend       | API Routes, Prisma ORM           |
| Database      | PostgreSQL (Neon DB)             |
| Auth          | Clerk                            |
| AI API        | Google Gemini 1.5 Flash          |
| DevOps        | Vercel, Inest (for cron jobs)    |

---

## ⚙️ Getting Started

 1. Clone the Repo
    
git clone https://github.com/PalakKhem16/CareerCoach.git

 3. Install Dependencies
    
npm install

5. Create .env File
   
Rename .env.example to .env and update:

DATABASE_URL=postgresql://<user>:<password>@<host>/<db>
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=<your-clerk-key>
CLERK_SECRET_KEY=<your-clerk-secret>

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding

GEMINI_API_KEY=<your-gemini-api-key>

4. Set Up Prisma
   
npx prisma generate
npx prisma db push

6. Start Dev Server
   
npm run dev
