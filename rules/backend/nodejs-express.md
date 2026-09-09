# Node.js & Express AI Agent Guidelines

- Use ES Modules exclusively (`import/export`) instead of CommonJS (`require`).
- Always wrap asynchronous route handlers with centralized error-handling middleware.
- Enforce strict environment variable validation via `dotenv` and Zod at application startup.
- Implement explicit CORS policies and secure HTTP headers via `helmet`.
