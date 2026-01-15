Architecture Overview
=====================

Components
----------
- Backend: FastAPI service
- Frontend: Next.js app
- CI: GitHub Actions (develop branch)
- Registry: Docker Hub
- Deployment templates: disabled workflows and infra docs for cloud targets

CI flow
-------
1. Checkout and environment setup (Python, Node)
2. Backend tests (pytest)
3. Frontend lint/test and Playwright E2E
4. Build Docker images
5. Push images to Docker Hub

Deployment stance
-----------------
- Workflows for main are present but disabled
- Infra/terraform directories provide guidance for AWS and GCP if needed

Observability and validation
---------------------------
- E2E tests validate backend availability and basic messaging
- Health endpoints covered by pytest
