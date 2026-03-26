# vibecoding-template

A ready-to-use AI project template pre-configured for **Claude** (Anthropic), **Codex** (OpenAI), and **Gemini** (Google). Drop these files into any project to give every AI coding agent the context it needs to work effectively.

---

## 📁 Template Files

| File | AI Agent | Purpose |
|------|----------|---------|
| [`CLAUDE.md`](./CLAUDE.md) | Anthropic Claude | Project context, conventions, and instructions for Claude |
| [`AGENTS.md`](./AGENTS.md) | OpenAI Codex / GPT | Project context, conventions, and instructions for Codex |
| [`GEMINI.md`](./GEMINI.md) | Google Gemini | Project context, conventions, and instructions for Gemini |
| [`.cursorrules`](./.cursorrules) | Cursor IDE | AI behavior rules for the Cursor code editor |
| [`.env.example`](./.env.example) | All agents | Template for API keys and environment variables |

---

## 🚀 Getting Started

### 1. Use this template

Click **"Use this template"** on GitHub to create a new repository, or copy the files manually:

```bash
# Copy all AI config files into your existing project
BASE=https://raw.githubusercontent.com/reomgit/vibecoding-template/main
curl -o CLAUDE.md        "$BASE/CLAUDE.md"
curl -o AGENTS.md        "$BASE/AGENTS.md"
curl -o GEMINI.md        "$BASE/GEMINI.md"
curl -o .cursorrules     "$BASE/.cursorrules"
curl -o .env.example     "$BASE/.env.example"
curl -o .gitignore       "$BASE/.gitignore"
```

### 2. Customize each file

Open each config file and fill in the `<!-- placeholders -->` with your project-specific details:

- **Project overview** — What does your project do?
- **Architecture** — How is your codebase structured?
- **Development commands** — How do you build, test, and lint?
- **Coding conventions** — What style and patterns does your team follow?

### 3. Set up environment variables

```bash
cp .env.example .env.local
# Edit .env.local and add your API keys
```

---

## 📝 File Descriptions

### `CLAUDE.md`
Read automatically by **Anthropic Claude** when it is invoked inside your repository. Tells Claude about your project structure, tech stack, commands to run, and coding conventions.

### `AGENTS.md`
Read automatically by **OpenAI Codex** and other OpenAI-based agents. Equivalent to `CLAUDE.md` but targeted at the OpenAI ecosystem.

### `GEMINI.md`
Read by **Google Gemini** to understand your project context. Follows the same structure as `CLAUDE.md` and `AGENTS.md`.

### `.cursorrules`
Loaded by the **Cursor IDE** to customize AI assistant behavior inside the editor. Controls code style preferences, do/don't rules, and context about the project.

### `.env.example`
A safe-to-commit template of all environment variables used in the project — including API keys for Claude, Codex, and Gemini. Copy to `.env.local` (never commit the copy).

---

## 🔒 Security

- **Never** commit `.env`, `.env.local`, or any file containing real API keys.
- The `.env.example` file contains only placeholder values and is safe to commit.
- Add `.env.local` (and any other real env files) to your `.gitignore`.

---

## 📄 License

[MIT](./LICENSE)
