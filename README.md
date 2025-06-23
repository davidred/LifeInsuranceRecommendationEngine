# Life Insurance Recommendation Engine – Starter Template

This repo provides a base project structure for candidates applying to build a full-stack insurance recommendation engine.

## Stack Overview

- **Frontend**: Next.js (React + TypeScript)
- **Backend**: Node.js with Express
- **Database**: PostgreSQL
- **DevOps**: Docker + Docker Compose

---

## 📁 Folder Structure

```bash
.
├── backend
│   ├── src
│   │   ├── routes
│   │   │   └── recommendation.ts
│   │   ├── db.ts
│   │   └── index.ts
│   ├── Dockerfile
│   └── package.json
├── frontend
│   ├── pages
│   │   ├── index.tsx
│   │   └── result.tsx
│   ├── components
│   │   └── RecommendationForm.tsx
│   ├── Dockerfile
│   └── package.json
├── docker-compose.yml
└── README.md
```

---

### ✅ Instructions

#### 1. Clone the repo

```bash
git clone <your-fork-url>
cd life-insurance-recommendation-template
```

#### 2. Start the app locally

```bash
docker-compose up --build
```

This will run:

- Frontend at `http://localhost:3000`
- Backend at `http://localhost:4000`
- PostgreSQL at port 5432

### 3. Environment Variables

Add a `.env` file inside `/backend`:

```bash
DATABASE_URL=postgres://postgres:postgres@db:5432/recommendation_db
```

---

### 💡 Your Tasks

- Implement the recommendation logic in `backend/src/routes/recommendation.ts`
- Build a simple form in `frontend/pages/index.tsx` that hits the backend endpoint
- Store user submissions in PostgreSQL
- Display the recommendation on `result.tsx`
- Dockerize both apps (already scaffolded)

---

### 📦 Tools You May Use

- TailwindCSS, Material UI (for frontend styling)
- Prisma or Knex.js (optional ORM for PostgreSQL)
- Zod or Joi (for backend input validation)

---

### 📝 Submission

When complete, please:

1. Push your changes to a public GitHub repo
2. Include a `README.md` with setup and deployment instructions
3. (Optional) Deploy the app using Vercel + Render or AWS

---

Happy building! 🚀
