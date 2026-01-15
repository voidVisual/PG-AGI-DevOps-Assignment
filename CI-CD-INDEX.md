CI/CD Documentation Index
=========================

Orientation
-----------
- Overview: [START-HERE.md](START-HERE.md)
- Quick setup: [QUICKSTART.md](QUICKSTART.md)
- Repo map: [PIPELINE-STRUCTURE.md](PIPELINE-STRUCTURE.md)
- Implementation summary: [IMPLEMENTATION-COMPLETE.md](IMPLEMENTATION-COMPLETE.md)

Workflows
---------
- CI: `.github/workflows/ci-develop.yml` (tests, build, push to Docker Hub)
- Deployment (disabled): `.github/workflows/deploy-main.yml.disabled`, `.github/workflows/cd-main.yml.disabled`
- Reference: [.github/WORKFLOW_REFERENCE.md](.github/WORKFLOW_REFERENCE.md)

Secrets and credentials
-----------------------
- Required: `DOCKERHUB_TOKEN`
- Optional: `DOCKERHUB_USERNAME`
- Guidance: [.github/SECRETS.md](.github/SECRETS.md)

Architecture and pipeline details
---------------------------------
- Pipeline deep dive: [.github/PIPELINE.md](.github/PIPELINE.md)
- System architecture: [.github/ARCHITECTURE.md](.github/ARCHITECTURE.md)
- Troubleshooting: [.github/TROUBLESHOOTING.md](.github/TROUBLESHOOTING.md)
- Quick reference: [.github/QUICK-REFERENCE.md](.github/QUICK-REFERENCE.md)

Infrastructure
--------------
- Deployment checklist: [infra/DEPLOYMENT-CHECKLIST.md](infra/DEPLOYMENT-CHECKLIST.md)
- Cloud templates: [infra/aws-ecs-config.md](infra/aws-ecs-config.md), [infra/k8s-deployment.md](infra/k8s-deployment.md)
- Terraform docs: see [infra/terraform/README.md](infra/terraform/README.md) and related guides
