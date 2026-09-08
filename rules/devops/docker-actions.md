# DevOps, Docker & CI/CD Guidelines for AI Agents

## 1. Dockerfile Optimization
- Always use specific base image tags with Alpine or slim variants (avoid `:latest`).
- Implement multi-stage builds to ensure runtime images contain zero build tooling or secrets.
- Run containers under an unprivileged user (`USER nonroot` or `USER 1001`), never as `root`.

## 2. GitHub Actions Security
- Pin all third-party GitHub Actions by full git commit SHA rather than floating branch tags (e.g., `@v4`).
- Grant minimum necessary permissions per workflow using explicit top-level `permissions` blocks.
- Never print or echo environment variables or GitHub Secrets in script steps.

## 3. Configuration Management
- Separate configuration from application logic using strictly validated environment variables.
- Always provide an updated `.env.example` file omitting any real credentials.
