# Agents

## Build/Lint/Test Commands

- **Development**: `pnpm run dev` (Vite dev server)
- **Build**: `pnpm run build` (Vite build)
- **Type check**: `pnpm run check` (SvelteKit sync + svelte-check)
- **Lint**: `pnpm run lint` (ESLint)
- **Unit tests**: `pnpm run test:unit` (Vitest)
- **E2E tests**: `pnpm run test:e2e` (Playwright)
- **Single test**: `pnpm run test:unit -- <file-path>` (e.g., `pnpm run test:unit -- src/routes/page.svelte.spec.ts`)
- **All tests**: `pnpm run test` (runs both unit and e2e)

## Code Style Guidelines

- **Language**: TypeScript with strict mode enabled
- **Framework**: Svelte 5 with runes ($derived, $state, etc.)
- **Styling**: Tailwind CSS v4
- **Imports**: Use `$lib/` for lib directory, relative paths for local files
- **Naming**: camelCase for variables/functions, PascalCase for components/classes
- **Types**: Explicit typing required, interfaces for complex objects
- **Error handling**: Use try/catch for async operations, proper TypeScript error types
- **Components**: Script tag first, then markup, then styles; use lang="ts"
- **Testing**: Vitest for unit tests, Playwright for e2e; use descriptive test names
- **Linting**: ESLint with recommended configs for JS/TS/Svelte; no custom rules
