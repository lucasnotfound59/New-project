# New Project Collection

A monorepo for housing multiple independent projects, each following a shared development lifecycle and standards.

---

## Repository Structure

Each project lives in its own isolated folder at the root of this repository. Projects must not share dependencies, files, or side effects with one another.

```
New-project/
├── README.md
├── DevelopmentRequirements.md
├── ProjectA/
│   ├── README.md
│   ├── DevLog.md
│   ├── Outline.md
│   ├── frontend/
│   ├── backend/
│   └── resources/
└── ProjectB/
    └── ...
```

---

## Development Lifecycle

Every project in this collection follows the same five-stage lifecycle:

### 1. Ideas
- Brainstorm ideas in the WeChat group.
- Once an idea is sufficiently mature, document it in a dedicated `Outline.md` inside a new project folder.

### 2. Research
- List all possible solutions to the problem being solved.
- Identify new technologies that need to be learned.
- Conduct a survey to validate demand (e.g., among classmates or potential users).
- Assess feasibility: technical complexity, cost, and resource availability.

### 3. Proof of Concept
- Build a lightweight demo that exercises all key technologies to be used.
- Release the demo to a small group of selected users.
- Announce the project to a broader audience to build early awareness.
- Collect and document feedback from demo participants.

### 4. Development
- Develop the full project according to the `Outline.md` and [DevelopmentRequirements.md](DevelopmentRequirements.md).
- Maintain a `DevLog.md` to record every meaningful change.

### 5. Publishing
- Ensure a sufficient user base before launch.
- If ongoing maintenance is free, the project must be free to use.

### 6. Advancement & Maintenance
- Plan feature improvements based on user feedback.
- Keep dependencies up to date and address reported issues promptly.

---

## Getting Started

1. Read [DevelopmentRequirements.md](DevelopmentRequirements.md) before contributing to any project.
2. Create a new folder for your project.
3. Write an `Outline.md` before writing any code.
4. Follow the lifecycle stages above in order.
