# Negari (ነጋሪ) - Civic Engagement Platform

[![Next.js](https://img.shields.io/badge/Next.js-13.0+-000000?logo=nextdotjs)](https://nextjs.org/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16+-4169E1?logo=postgresql)](https://www.postgresql.org/)
[![Vercel](https://img.shields.io/badge/Deployed_on-Vercel-000000?logo=vercel)](https://vercel.com/)
[![Gemini API](https://img.shields.io/badge/AI-Gemini_API-4285F4?logo=google)](https://ai.google.dev/)

<img src="https://github.com/kirubelatk/Negari/blob/main/Negari.png" alt="Negari Platform Interface" width="800">

## Overview
Negari is a full-stack civic engagement platform connecting Ethiopian citizens with local governments. The platform enables anonymous feedback submission, AI-powered sentiment analysis of community input, and real-time dashboards for government officials to improve service transparency and accountability.

**Live Demo**: [https://negari.vercel.app/](https://negari.vercel.app/)

## Key Features

### 👥 Citizen Experience
- 🔍 Search local government offices (Kebele/Woreda)
- 📝 Submit feedback & ratings (anonymous option)
- 📊 View service guides with requirements & fees
- 🗺️ Interactive office location maps
- 🌐 English/Amharic language toggle

### 🏛 Government Dashboard
- 📈 AI sentiment analysis (Gemini API)
- 🧠 Automatic theme categorization (corruption, delays, etc.)
- 📉 Real-time trend visualization
- 📥 PDF/CSV report generation
- 💬 Public response to citizen feedback

### 🔒 Admin Portal
- 👥 User management & role control
- 🏢 Office/service CRUD operations
- ⚠️ Flagged content moderation
- 📊 System performance monitoring

## Technology Stack

| Component              | Technology                           |
|------------------------|--------------------------------------|
| **Frontend**           | Next.js 14, React 18, TypeScript     |
| **Styling**            | Tailwind CSS, Shadcn UI              |
| **Backend**            | Next.js API Routes, Node.js 18       |
| **Database**           | PostgreSQL 16 (via Supabase)         |
| **AI/ML**              | Google Gemini API                    |
| **Authentication**     | JWT, OAuth2, Next-Auth              |
| **Deployment**         | Vercel, Supabase                     |
| **Testing**            | Jest, React Testing Library, Cypress |
| **Localization**       | i18next, react-i18next               |

## Getting Started

### Prerequisites
- Node.js v18+
- PostgreSQL 16+
- Google Cloud API key (for Gemini)
- Vercel account (for deployment)

### Installation
```bash
# Clone repository
git clone https://github.com/kirubelatk/negari.git
cd negari

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env.local
# Edit .env.local with your credentials

# Run database migrations
npx prisma migrate dev

# Start development server
npm run dev
