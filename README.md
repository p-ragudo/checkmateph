<div align="center">

# CheckMatePH

**A political fact-checking and civic engagement platform for Filipino voters.**

[![Next.js](https://img.shields.io/badge/Next.js-black?style=flat-square&logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-blue?style=flat-square&logo=typescript)](https://www.typescriptlang.org/)
[![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase)](https://supabase.com/)
[![Vercel](https://img.shields.io/badge/Vercel-black?style=flat-square&logo=vercel)](https://vercel.com/)

*SIKAPTala 2026 · Hackathon · Team Debuggerinas · DLSU–Dasmariñas*

</div>

---

## What It Does

CheckMatePH is a web-based political social media platform where every post is **fact-checked by AI before it goes live**, then open to review by accredited human experts. It gives Filipino citizens — especially first-time voters and youth — a trustworthy space to read, post, and debate political claims.

**Core features:**
- **AI Fact-Check Gate** — posts are analyzed by OpenAI before publishing; each receives a verdict (`Likely True`, `Needs Verification`, or `Likely False`) with a confidence score and rationale
- **Political Discussion Feed** — structured civic feed with upvotes, threaded comments, and topic categories
- **Verified Politician Profiles** — integrity scores, claims history, and a promise vs. action tracker
- **Debate Rooms** — real-time structured debates with live voting via Supabase Realtime
- **Role-Based Access** — Regular Users, Verified Experts, Moderators, and Verified Politicians

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | Next.js (React) + TypeScript |
| Styling | Tailwind CSS + shadcn/ui |
| Backend & Database | Supabase (PostgreSQL + Realtime) |
| Authentication | Supabase Auth (JWT + RLS) |
| AI | OpenAI API |
| Deployment | Vercel + Supabase Cloud |

---

## Getting Started

**Prerequisites:** Node.js 18+, a Supabase project, an OpenAI API key.

```bash
git clone https://github.com/jpmartirez/checkmateph.git
cd checkmateph
npm install
```

Create a `.env.local` file:

```env
NEXT_PUBLIC_SUPABASE_URL=your_supabase_project_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
OPENAI_API_KEY=your_openai_api_key
```

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

---

## Project Structure

```
checkmateph/
├── app/          # Next.js App Router pages & layouts
├── components/   # Reusable UI components
├── lib/          # Supabase client, utilities, API helpers
└── public/       # Static assets
```

---

## Hackathon Scope

- AI fact-checking is probabilistic, not a legal determination of truth
- Debate rooms are text-only (no audio/video)
- Tagalog NLP and OAuth login are deferred post-hackathon
- Web-only; no native mobile app (fully responsive)

---

## Team

**Debuggerinas** — Manuel S. Enverga University Foundation – Lucena, City  
Built for SIKAPTala 2026: The National CS & IT Competition
