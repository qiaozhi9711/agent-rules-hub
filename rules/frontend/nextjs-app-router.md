# Next.js 15 App Router Guidelines for AI Agents

## 1. Server & Client Component Boundaries
- Default to React Server Components (RSC); explicitly add `"use client"` directive only when hooks, state, or browser APIs are required.
- Minimize client-side bundle size by pushing `"use client"` boundaries down to leaf nodes.

## 2. Dynamic Routing & Asynchronous APIs
- Handle route parameters and search parameters asynchronously (`await params`, `await searchParams`) following Next.js 15 requirements.
- Utilize built-in `Suspense` and `loading.tsx` conventions for streaming data fetching.

## 3. Server Actions & Mutation Security
- Isolate Server Actions in dedicated modules (`actions.ts`) with top-level `"use server"`.
- Enforce runtime payload validation using Zod schemas before executing database mutations.
