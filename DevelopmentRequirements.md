# Development Requirements

Standards and rules that every project in this repository must follow.

---

## Project Isolation

**REQ-01** — Each project must be contained within its own dedicated folder.

**REQ-02** — A project must not read from, write to, or depend on files belonging to another project. Side effects that cross project boundaries are not allowed.

---

## Documentation

**REQ-03** — A development outline (`Outline.md`) must be written and reviewed **before** any code is written. The outline should describe the project's goal, scope, and planned architecture.

**REQ-04** — A development log (`DevLog.md`) must be maintained throughout the project. Every significant modification — new features, bug fixes, refactors, dependency updates — must be recorded with a date and a brief description.

---

## File & Folder Structure

**REQ-05** — Files must be organized by purpose, not dumped into a single flat directory. The recommended structure is:

```
ProjectName/
├── Outline.md          # Written before any code
├── DevLog.md           # Updated with every meaningful change
├── README.md           # Project-level overview
├── frontend/           # All client-side code
├── backend/            # All server-side code
├── resources/          # Static assets, configs, data files
└── tests/              # Test suites
```

Adapt the structure as needed, but never place all source files at the same level without organization.

---

## Code Quality

**REQ-06** — No code may be committed to the main branch without at least one other team member reviewing it.

**REQ-07** — Sensitive data (API keys, passwords, credentials) must never be committed. Use environment variables or a secrets manager.

**REQ-08** — Third-party dependencies must be explicitly listed in a dependency file (e.g., `requirements.txt`, `package.json`). Vendored or manually copied libraries are not permitted.

---

## Naming Conventions

**REQ-09** — Folder and file names must use `kebab-case` or `PascalCase` consistently within each project. Mixed conventions within the same project are not allowed.

**REQ-10** — Variable and function names within code must follow the conventions of the language being used (e.g., `snake_case` for Python, `camelCase` for JavaScript/TypeScript).

---

## Compliance

All requirements above are mandatory. Any exception must be discussed with the team and documented in the project's `DevLog.md` with a justification.
