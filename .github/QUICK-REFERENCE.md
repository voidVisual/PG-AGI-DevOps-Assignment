Quick Reference
===============

Branches
--------
- `develop`: CI (tests, build, push images)
- `main`: Deployment templates (disabled)

Secrets
-------
- `DOCKERHUB_TOKEN` (required)
- `DOCKERHUB_USERNAME` (optional)

Image tags
----------
- `{short-sha}` and `latest`
- Backend: `<dockerhub-user>/pg-agi-backend`
- Frontend: `<dockerhub-user>/pg-agi-frontend`

Key commands (local)
--------------------
Backend: `pip install -r requirements.txt && python -m pytest app/test_main.py`
Frontend: `npm ci && npm run lint && npx playwright install --with-deps && npx playwright test`
