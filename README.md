# agent-rules-hub
A curated collection of production-ready rules and instructions for AI coding assistants (Codex, Cursor, Claude Code).
# Agent Rules Hub 🤖

A production-grade, community-driven collection of system prompts, agent instructions, and `.cursorrules` optimized for OpenAI Codex, Cursor, and modern AI coding assistants.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

## 📌 Features
- **Strict Guidelines**: Context-aware coding standards to prevent LLM hallucinations.
- **Multi-Stack Coverage**: Python (FastAPI/Django), TypeScript (React/Next.js), Go, and DevOps configs.
- **Security Guardrails**: Hardened constraints against secret leaks and insecure dependencies.

## 📁 Repository Structure

├── rules/
│   ├── frontend/         # React, Next.js, Vue
│   ├── backend/          # Python, Node.js, Go
│   └── devops/           # Docker, GitHub Actions
├── CONTRIBUTING.md       # Contribution guide
└── README.md

### 📦 Available Rule Profiles

| Stack / Framework | Category | File Link | Target Agents |
| :--- | :--- | :--- | :--- |
| **Next.js 15 (App Router)** | Frontend | [`rules/frontend/nextjs-app-router.md`](./rules/frontend/nextjs-app-router.md) | Codex / Cursor / Claude |
| **Node.js & Express** | Backend | [`rules/backend/nodejs-express.md`](./rules/backend/nodejs-express.md) | Codex / Cursor |
| **Python FastAPI** | Backend | [`rules/backend/python-fastapi.md`](./rules/backend/python-fastapi.md) | Codex / Cursor |
| **Docker & CI/CD** | DevOps | [`rules/devops/docker-actions.md`](./rules/devops/docker-actions.md) | Cursor / GitHub Actions |

🚀 How to Use
Locate your technology stack in the rules/ directory.

Copy the content into your project's .cursorrules, .prompt, or AI configuration file.

Customize API paths or project-specific constraints as needed.

🤝 Contributing
Contributions are welcome! Please read CONTRIBUTING.md to submit your own rule profiles.
