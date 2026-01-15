Setup Guide
===========

Goals
-----
- Run CI on `develop`
- Publish Docker images to Docker Hub
- Prepare (optional) deployment workflows

Prerequisites
-------------
- GitHub repository with Actions enabled
- Secrets: `DOCKERHUB_TOKEN` (required), `DOCKERHUB_USERNAME` (optional)
- Docker Hub account and token

Steps
-----
1. Configure secrets in GitHub
2. Push to `develop`
3. Verify CI completes and images appear in Docker Hub
4. (Optional) Review disabled deployment workflows and enable with credentials

Verification checklist
----------------------
- CI passes on `develop`
- Images `pg-agi-backend` and `pg-agi-frontend` tagged with `latest` and short SHA
- Documentation available (see [CI-CD-INDEX.md](CI-CD-INDEX.md))

References
----------
- [QUICKSTART.md](QUICKSTART.md)
- [.github/PIPELINE.md](.github/PIPELINE.md)
- [.github/SECRETS.md](.github/SECRETS.md)
