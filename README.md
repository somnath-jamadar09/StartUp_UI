# StartUp_UI

**Frontend UI for a technology services & AI engineering consultancy platform** — built with React 18, TypeScript, Vite, and Tailwind CSS in a "Synthetic Precision" dark-mode design system.

This repository contains the client-facing UI screens (project intake, client dashboard, operations/CRM, and engineering/QA control center) along with the full project documentation set that governs delivery, design, and engineering standards.

---

## 🎨 Screens

Generated from a shared design system and 15-step project lifecycle workflow:

1. **Project Intake & Compliance Wizard** — client category switch (Student/SME), Tier 1–4 service matrix, project scope declaration with NLP feedback, budget slider, and live GST estimator.
2. **Client Project Dashboard** — 15-step progress stepper, staging/CI status, milestone & GST invoice ledger, 30-day support SLA tracker.
3. **Operations & CRM Executive Dashboard** — intake queue with NLP compliance screening, feasibility scorecards, team capacity view, SOW/proforma invoice generator.
4. **Engineering & QA Control Center** — sprint backlog, CI/CD pipeline status, QA acceptance checklists, staging deployment controls.

---

## 🧱 Tech Stack

| Layer | Technology |
|---|---|
| Framework | React 18 + TypeScript |
| Build tool | Vite |
| Styling | Tailwind CSS |
| Icons | Lucide React |
| Auth | Google OAuth (`@react-oauth/google`, `jwt-decode`) |
| Utilities | `clsx`, `tailwind-merge` |

See [`Documentation/V1/TechStack.md`](Documentation/V1/TechStack.md) for the full approved stack (backend, database, cloud, CI/CD).

---

## 📁 Repository Structure

```text
StartUp_UI/
├── frontend/                  # React + TypeScript + Vite application
│   ├── src/
│   │   ├── components/        # Shared UI: auth, header, stepper, toasts, notifications
│   │   ├── features/          # Feature screens: intake, dashboard, operations, engineering, browse, home
│   │   ├── context/            # AuthContext
│   │   ├── types/              # Shared data models
│   │   └── utils/               # GST calculation, UGC compliance filter
│   ├── .env.example
│   └── package.json
├── Documentation/
│   ├── GOOGLE_OAUTH_SETUP.md
│   └── V1/                    # Business, legal, design & engineering docs (SRS, SDD, Architecture, Workflow, etc.)
└── LICENSE
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js v20.x LTS
- npm

### Setup

```bash
# Clone the repository
git clone https://github.com/<your-org>/StartUp_UI.git
cd StartUp_UI/frontend

# Install dependencies
npm install

# Configure environment variables
cp .env.example .env
# then set VITE_GOOGLE_CLIENT_ID and VITE_ADMIN_EMAILS (see Documentation/GOOGLE_OAUTH_SETUP.md)

# Start the development server
npm run dev
```

The app runs at `http://localhost:5173` by default.

### Other scripts

```bash
npm run build     # Type-check and build for production
npm run preview   # Preview the production build locally
npm run lint       # Run ESLint
```

---

## 📚 Documentation

Full project documentation lives in [`Documentation/V1/`](Documentation/V1), including:

| Doc | Purpose |
|---|---|
| `SRS.md` / `SDD.md` | Requirements & software design |
| `Architecture.md` | System architecture & APIs |
| `Design.md` | UI/UX design system (Synthetic Precision) |
| `Workflow.md` | 15-step project lifecycle |
| `TechStack.md` | Approved technologies |
| `Roles.md` | Team roles & RACI |
| `Legal.md` | MSA, SOW, NDA, IP agreements |
| `Roadmap.md` | 1/3/5-year roadmap |

---

## ⚖️ Compliance Note

This project follows the **UGC (Promotion of Academic Integrity and Prevention of Plagiarism) Regulations, 2018**. Student/academic engagements are limited to mentorship, code review, debugging, and infrastructure support — not ghostwriting or graded coursework execution. See `Documentation/V1/Readme.md` for full details.

---

## 📄 License

Distributed under the MIT License. See [`LICENSE`](LICENSE) for details.
