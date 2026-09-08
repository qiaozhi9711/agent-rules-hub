# React & Tailwind CSS AI Agent Guidelines

## 1. Component Architecture & TypeScript
- Use TypeScript with React 19+ strict mode enabled.
- Avoid using `React.FC`; define props with explicit interfaces (`interface ButtonProps { ... }`).
- Implement small, single-responsibility functional components. Prefer Server Components in Next.js/framework setups unless client interactivity (`"use client"`) is required.

## 2. Styling Standards (Tailwind CSS)
- Always use utility-first styling; avoid inline CSS styles.
- Organize class order logically: layout -> spacing -> typography -> visual -> state (e.g., hover/focus).
- Use `clsx` or `tailwind-merge` when constructing conditional class names to prevent class conflicts.

## 3. Performance & Accessibility
- Ensure all interactive elements include proper ARIA attributes (`aria-label`, `role`).
- Always specify explicit `alt` text for images and dimensions to prevent layout shifts.
- Optimize rerenders using standard React hooks (`useCallback`, `useMemo`) only when measured bottlenecks exist.
