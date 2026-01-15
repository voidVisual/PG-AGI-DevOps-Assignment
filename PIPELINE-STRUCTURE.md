Pipeline Structure
==================

Repository layout (selected)
----------------------------
- `backend/`: FastAPI app, tests, Dockerfile
- `frontend/`: Next.js app, Playwright E2E, Dockerfile
- `.github/workflows/`: CI and disabled deployment workflows
- `infra/`: deployment checklists and cloud templates
- `infra/terraform/`: Terraform modules and guides
- Docs: `START-HERE.md`, `QUICKSTART.md`, `CI-CD-INDEX.md`, `IMPLEMENTATION-COMPLETE.md`, `README-CICD.md`

Workflows
---------
- `ci-develop.yml`: tests, build, push images to Docker Hub
- `deploy-main.yml.disabled` / `cd-main.yml.disabled`: example deployment pipelines (disabled)

Images and tagging
------------------
- Backend image: `<dockerhub-user>/pg-agi-backend:{short-sha|latest}`
- Frontend image: `<dockerhub-user>/pg-agi-frontend:{short-sha|latest}`

Key scripts and configs
-----------------------
- `infra/setup-cicd.sh`: optional helper for environment setup
- `infra/aws-ecs-config.md`, `infra/k8s-deployment.md`: deployment templates
- `infra/terraform/*`: IaC reference for AWS and GCP modules
