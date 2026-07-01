# test-halo

A small monorepo with a React frontend and a FastAPI backend.

## Structure

| Path | Stack | Tooling |
|------|-------|---------|
| `frontend/` | React + Vite + TypeScript | ESLint, Prettier |
| `backend/` | FastAPI (Python 3.12) | ruff, black, mypy, pytest |

## CI

GitHub Actions runs on every pull request and push to `main`:

- **frontend-ci** — lint, format check, build
- **backend-ci** — lint, format check, type check, tests

## Local development

```bash
# Frontend
cd frontend && npm install && npm run dev

# Backend
cd backend && python3 -m venv .venv && .venv/bin/pip install -r requirements-dev.txt
.venv/bin/uvicorn app.main:app --reload
```

## aaaa
