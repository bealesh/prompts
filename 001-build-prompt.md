You are building a production-minded system based on the following product and architectural specification.

---

## 1. Context

[Describe the product clearly and *what it is NOT*]

- What this system is:
- What this system is NOT:
- Core concept:
- Key users (humans, agents, systems):
- High-level narrative (1–2 sentences max):

---

## 2. Product Philosophy

[Define how to think, not just what to build]

- Primary value being created:
- Why this matters:
- Constraints (technical, regulatory, UX, etc.):
- What we are explicitly avoiding:

---

## 3. System Architecture

[Define boundaries early]

- Components:
  - Frontend (if applicable):
  - Backend / core services:
  - Machine interface (API / MCP / etc):
- Deployment expectations:
- Separation of concerns:
- What must be standalone vs embedded:

---

## 4. Scope (V1)

[Be brutally clear about what to build now]

Build only:

- Feature / tool 1:
- Feature / tool 2:
- Feature / tool 3:

Goals:
- [e.g. read-heavy, low-risk, high-signal]

---

## 5. Non-Goals (V1)

[Prevents overbuilding]

Do NOT implement:

- Feature:
- Feature:
- Feature:

---

## 6. Interfaces / Tools

[This is the core of agent-driven systems]

Define the system interface as structured tools:

- tool_name
  - description
  - inputs
  - outputs

Repeat for each tool.

Guidelines:
- Strong typing
- Machine-readable responses
- Stable schemas
- Pagination where applicable

---

## 7. Data Modeling

[Design for evolution]

Core entities:
- Entity 1
- Entity 2
- Entity 3

Requirements:
- stable IDs
- timestamps everywhere
- explicit enums
- provenance-friendly fields

If schema unknown:
→ create clean placeholder interfaces

---

## 8. Auth & Permissions

- public vs authenticated access
- scope-based permissions
- future extensibility for advanced roles (agents, admins, etc.)

---

## 9. Reliability & Safety

- validation requirements
- rate limiting considerations
- error handling structure
- explicitly disallowed behaviors

---

## 10. Implementation Requirements

- language / framework:
- validation library:
- testing expectations:
- folder structure:

Example:
- /src/server
- /src/tools
- /src/domain
- /src/services
- /src/repositories
- /src/types
- /tests

---

## 11. Developer Experience

Include:
- local setup instructions
- seed data
- example usage
- clear README

---

## 12. Deliverables

- working system
- documented interfaces
- test coverage
- extensible architecture

---

## 13. Product Intent (Anchor)

[This is the soul of the system]

Write 2–3 sentences that explain:
- what this system enables
- who it is for
- why it matters

This should guide all implementation decisions.