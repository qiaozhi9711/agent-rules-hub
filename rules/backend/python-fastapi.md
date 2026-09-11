# FastAPI & Python AI Agent Guidelines

## 1. Type Hints & Pydantic Validation
- Enforce explicit type annotations across all function signatures and return types.
- Use Pydantic v2 `BaseModel` schemas for strict request body and query parameter validation.

## 2. Asynchronous Route Architecture
- Declare route handlers as `async def` for I/O-bound operations (database queries, external API calls).
- Use standard synchronous `def` for CPU-bound tasks to prevent event loop starvation.

## 3. Dependency Injection & Error Handling
- Manage database sessions, authorization, and caching strictly via FastAPI's `Depends()` dependency injection.
- Raise standardized `HTTPException` payloads with consistent JSON error envelopes.
