# CLAUDE.md

This file provides guidance to Claude (Anthropic) when working with code in this repository.

## Project Overview

<!-- Describe your project here -->
This is a [project type] built with [technologies]. It [brief description of what it does].

## Architecture

<!-- Describe your project architecture -->
```
src/
├── components/    # Reusable UI components
├── lib/           # Utility functions and helpers
├── pages/         # Page-level components / routes
└── types/         # TypeScript type definitions
```

## Development Commands

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Run tests
npm test

# Run linter
npm run lint

# Build for production
npm run build
```

## Coding Conventions

- **Language**: TypeScript (strict mode)
- **Formatting**: Prettier with default config
- **Linting**: ESLint with project rules
- **Testing**: Jest + Testing Library
- **Commits**: Conventional Commits (`feat:`, `fix:`, `chore:`, etc.)

## Key Files & Directories

| Path | Purpose |
|------|---------|
| `src/` | Main source code |
| `public/` | Static assets |
| `tests/` | Test files |
| `.env.example` | Example environment variables |

## Environment Variables

Copy `.env.example` to `.env.local` and fill in the values:

```bash
cp .env.example .env.local
```

## Important Notes for Claude

- Always run `npm run lint` and `npm test` after making changes.
- Keep components small and focused on a single responsibility.
- Prefer named exports over default exports.
- Write tests for all new functions and components.
- Do not commit secrets or API keys — use environment variables.
- Follow existing patterns in the codebase when adding new features.
