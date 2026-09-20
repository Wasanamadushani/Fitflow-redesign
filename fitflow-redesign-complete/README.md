# FitFlow Redesign

Redesigned FitFlow fitness app — AI-powered personalized workout plans, private social
circles, and camera-based nutrition tracking. Built for IT3060 (Human Computer
Interaction) Lab Exercise 05.

## Recommended Technology Stack

| Layer | Choice |
|---|---|
| Frontend | React Native + React Native Web |
| Backend API | Node.js / NestJS |
| AI Microservice | Python / FastAPI + TensorFlow |
| Primary Database | PostgreSQL |
| Real-time Layer | Firebase Firestore / Realtime Database |
| Authentication | Firebase Auth |
| Cache | Redis |

See `docs/comparison-matrix.md` for the full weighted decision matrix and
`docs/ADR-001.md` for the architecture decision record.

## Project Structure

```
fitflow-redesign/
├── frontend/       # React Native app (mobile + web)
├── backend/        # NestJS services (auth, workout, nutrition, social)
├── ai-service/     # FastAPI AI microservice (recommendations, computer vision)
├── docs/           # Comparison matrix, architecture diagram, ADRs
└── .github/workflows/  # CI pipelines
```

## Getting Started

### Frontend
```bash
cd frontend
npm install
npm run start
```

### Backend
```bash
cd backend
npm install
npm run start:dev
```

### AI Service
```bash
cd ai-service
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
uvicorn main:app --reload
```

## Documentation

- [Technology Comparison Matrix](docs/comparison-matrix.md)
- [Architecture Diagram](docs/architecture-diagram.png)
- [ADR-001: Technology Stack Decision](docs/ADR-001.md)

## Repository Structure

- `frontend/` — React Native + React Native Web frontend placeholder
- `backend/` — Node.js/NestJS backend services placeholder
- `ai-service/` — Python/FastAPI AI microservice placeholder
- `docs/comparison-matrix.md` — Activities 1–3 comparison and weighted matrix
- `docs/architecture.md` — high-level architecture documentation
- `docs/architecture-diagram.png` — architecture diagram
- `docs/ADR-001.md` — Architecture Decision Record
- `.github/workflows/ci.yml` — optional CI workflow
