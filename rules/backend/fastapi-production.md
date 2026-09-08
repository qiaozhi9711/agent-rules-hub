# FastAPI & Python AI Agent Guidelines

## 1. Code Architecture & Typing
- Exclusively use Python 3.11+ type hints (e.g., use `int | None` instead of `Optional[int]`).
- Follow the official modular APIRouter structure with unified response envelopes.
- Always use asynchronous database drivers (AsyncSession with SQLAlchemy / Tortoise ORM).

## 2. Security & Input Validation
- Validate all incoming request schemas using Pydantic V2 models with strict constraints.
- Never output raw passwords, bearer tokens, or sensitive credentials in logs or responses.
- Implement rate limiting and CORS middleware explicitly for production endpoints.

## 3. Error Handling
- Use structured JSON error responses rather than plain HTTP 500 exceptions.
- Trap database integrity errors and translate them into descriptive client-side messages.
