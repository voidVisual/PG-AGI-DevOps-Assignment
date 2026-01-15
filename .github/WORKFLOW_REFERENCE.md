Workflow Reference
==================

ci-develop.yml (develop)
------------------------
- Setup: checkout, Python 3.12, Node 20
- Backend: install requirements, run pytest on `app/test_main.py`
- Frontend: npm ci, Playwright install with deps, npm test, Playwright E2E
- Build and push: backend and frontend images to Docker Hub with short-SHA and `latest` tags

deploy-main.yml.disabled and cd-main.yml.disabled (main)
-------------------------------------------------------
- Templates for deployment; disabled to avoid unintended runs
- Adapt for target platforms and add credentials before enabling

Caching and tagging
-------------------
- Buildx with GitHub Actions cache
- Tag format: `{short-sha}` and `latest`
