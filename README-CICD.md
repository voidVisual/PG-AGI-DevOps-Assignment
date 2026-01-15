CI/CD Overview
==============

Pipelines
---------
- CI (`develop`): `.github/workflows/ci-develop.yml`
	- Backend tests: pytest
	- Frontend: npm lint/test, Playwright E2E
	- Build and push Docker images (backend and frontend) to Docker Hub
- Deployment (main): `.github/workflows/deploy-main.yml.disabled`, `.github/workflows/cd-main.yml.disabled` (provided as templates)

Images
------
- Backend: `<dockerhub-user>/pg-agi-backend:{short-sha|latest}`
- Frontend: `<dockerhub-user>/pg-agi-frontend:{short-sha|latest}`

Secrets
-------
- Required: `DOCKERHUB_TOKEN`
- Optional: `DOCKERHUB_USERNAME` (falls back to repository owner)

Docs map
--------
- Start: [START-HERE.md](START-HERE.md), [QUICKSTART.md](QUICKSTART.md)
- Index: [CI-CD-INDEX.md](CI-CD-INDEX.md)
- Reference: [.github/PIPELINE.md](.github/PIPELINE.md), [.github/SECRETS.md](.github/SECRETS.md), [.github/TROUBLESHOOTING.md](.github/TROUBLESHOOTING.md)
