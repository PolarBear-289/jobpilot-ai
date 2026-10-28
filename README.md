# JobPilot AI

A local-first, AI-powered job discovery and application management platform.

JobPilot AI discovers relevant job opportunities, evaluates them against a user's professional profile, generates job-specific resume versions, and assists with application workflows.

The project is being developed with an emphasis on privacy, reliability, automation safety, and production-oriented software engineering practices.

## Objectives

- Discover relevant jobs from supported sources.
- Filter opportunities using configurable job preferences.
- Evaluate job descriptions against the user's profile.
- Use a local language model for job matching and resume assistance.
- Generate tailored resumes without inventing qualifications or experience.
- Track applications and prevent duplicate submissions.
- Support human review when automation is restricted or uncertain.
- Run locally without requiring paid AI APIs.

## Technology Stack

### Backend
- Python 3.12
- FastAPI
- SQLAlchemy
- Alembic
- PostgreSQL
- Pydantic

### Frontend
- React
- Vite
- TypeScript

### AI and Automation
- Ollama for local language model inference
- Playwright for permitted browser automation

### Development and Deployment
- uv for Python dependency management
- npm for frontend dependency management
- Docker and Docker Compose
- pytest for backend testing
- GitHub Actions for CI

## Project Structure

```text
jobpilot-ai/
├── backend/
├── frontend/
├── config/
├── deploy/
├── docs/
├── scripts/
├── tests/
├── .env.example
├── .gitignore
└── README.md
```

## Development Status

The project is currently in the initial setup and architecture phase.

Application features, database models, and automation workflows will be implemented incrementally with appropriate testing and documentation.

## Development Principles

- Keep personal data and credentials out of source control.
- Use database migrations for schema changes.
- Prefer deterministic business rules for eligibility and safety checks.
- Validate AI-generated output before using it.
- Make application workflows idempotent and recoverable.
- Respect website terms, access restrictions, and authentication requirements.
- Test changes before integrating them into the main branch.

## License

License selection is pending.