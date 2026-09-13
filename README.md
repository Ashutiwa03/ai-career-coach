# AI Career Coach

An AI-powered career guidance platform that helps users build resumes, prepare for interviews, write cover letters, and get personalized career insights — powered by **Google Gemini AI**.

## ✨ Features

- 🧠 **AI-Powered Career Guidance** — Personalized career advice generated using Gemini AI
- 📄 **Smart Resume Builder** — Create and edit professional resumes with markdown support and PDF export
- 🎯 **Interview Preparation** — Practice with AI-generated interview questions and feedback
- 📊 **Industry Insights Dashboard** — Visual insights and trends for different industries using interactive charts
- 💼 **Job Preparation Tools** — Guidance and resources to prepare for job applications
- ✉️ **Cover Letter Generator** — AI-assisted cover letter creation tailored to job roles
- 🔐 **Secure Authentication** — User sign-in/sign-up powered by Clerk
- 🌗 **Light/Dark Theme Support**

## 🛠️ Tech Stack

**Framework & Frontend**
- [Next.js 15](https://nextjs.org/) (App Router, Turbopack)
- [React 19](https://react.dev/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Radix UI](https://www.radix-ui.com/) components
- [Lucide Icons](https://lucide.dev/)
- [Recharts](https://recharts.org/) for data visualization

**Backend & Database**
- [Prisma ORM](https://www.prisma.io/) with PostgreSQL
- [Inngest](https://www.inngest.com/) for background jobs / event-driven functions

**AI & Auth**
- [Google Generative AI (Gemini)](https://ai.google.dev/) for AI-powered features
- [Clerk](https://clerk.com/) for authentication

**Other Libraries**
- React Hook Form + Zod for form handling & validation
- React Markdown & @uiw/react-md-editor for markdown editing
- html2pdf.js for PDF export
- Sonner for toast notifications

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher recommended)
- A PostgreSQL database
- API keys for Clerk and Google Generative AI

### Installation

1. Clone the repository
```bash
git clone <your-repo-url>
cd ai-career-coach
```

2. Install dependencies
```bash
npm install
```

3. Set up environment variables

Create a `.env` file in the root directory and add the required keys:
```env
DATABASE_URL=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
GEMINI_API_KEY=
```

4. Run Prisma migrations
```bash
npx prisma generate
npx prisma migrate dev
```

5. Start the development server
```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the app.

## 📜 Available Scripts

| Command | Description |
|---|---|
| `npm run dev` | Start the development server (Turbopack) |
| `npm run build` | Build the app for production |
| `npm run start` | Start the production server |
| `npm run lint` | Run ESLint |

## 📂 Project Structure

```
ai-career-coach/
├── prisma/           # Database schema & migrations
├── public/           # Static assets (images, logo)
├── app/ (or pages/)  # Application routes
├── components/       # Reusable UI components
├── .env               # Environment variables
└── package.json
```

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to fork the repo and submit a pull request.

## 📄 License

This project is private and intended for personal/educational use.