# AGENTS.md

This file provides guidance to OpenAI Codex and other OpenAI-based AI coding agents when working with code in this repository.

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

## Instructions for Codex

- Always run `npm run lint` and `npm test` after making changes.
- Do not make changes outside of the `src/` and `tests/` directories unless explicitly asked.
- When creating new files, place them in the correct directory based on their purpose.
- Each function should have a clear, single responsibility.
- Write unit tests for every new function and component you create.
- Do not commit secrets or API keys — use environment variables.
- When fixing bugs, add a regression test to prevent future regressions.
