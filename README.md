---
members:
  - name: John Lakos
    email: jlakos@bloomberg.net
    affiliation: Bloomberg LP
    github: jslakos
    status: active
    roles:
      - Large-Scale Deployment
      - Safety & Correctness
  - name: Joshua Berne
    email: jberne4@bloomberg.net
    affiliation: Bloomberg LP
    github: notadragon
    status: active
    roles:
      - Language Specification
      - Library Architecture
  - name: Pablo Halpern
    email: pablo@halpern.dev
    affiliation: Bloomberg LP
    github: phalpern
    status: active
    roles:
      - Library Architecture
      - Concurrency & Systems
  - name: Harold Bott
    email: harry@cppalliance.org
    affiliation: C++ Alliance
    github: bottha123
    status: active
    roles:
      - Performance Engineering
      - Pedagogy & Teachability
  - name: Mungo Gill
    email: mungo@cppalliance.org
    affiliation: C++ Alliance
    github: MungoG
    status: active
    roles:
      - Large-Scale Deployment
      - Pedagogy & Teachability
---

# The PRAGMA Group

**Public Review and Advisory Group for Mailing Analysis**

PRAGMA evaluates WG21 standardization proposals against disclosed principles. The methodology is public. The papers are informational. The work succeeds by being useful.

Welcome. Everything here is meant to be read.

---

## Members

| Name           | Affiliation    | Status | Roles                                            |
|----------------|----------------|--------|--------------------------------------------------|
| John Lakos     | Bloomberg LP   | Active | Large-Scale Deployment, Safety & Correctness     |
| Joshua Berne   | Bloomberg LP   | Active | Language Specification, Library Architecture     |
| Pablo Halpern  | Bloomberg LP   | Active | Library Architecture, Concurrency & Systems      |
| Harold Bott    | C++ Alliance   | Active | Performance Engineering, Pedagogy & Teachability |
| Mungo Gill     | C++ Alliance   | Active | Large-Scale Deployment, Pedagogy & Teachability  |

The YAML front matter in this file is the authoritative membership record. Changes to membership must update both the front matter and the visible list.

---

## Repository Layout

### `const/`

The founding documents. What PRAGMA is, why it operates the way it does, and the values that define the institution. Changes to these documents require a separate deliberation process with the highest bar for unanimity.

- **[pragma.md](const/pragma.md)** - The founding document. Values, process, and scope. Start here.
- **[pragma-once.md](const/pragma-once.md)** - The strategy document. Single scope, the five values, and the argument behind the posture.
- **[pragma-pack.md](const/pragma-pack.md)** - The composition document. Structure, roles, and the principle that evaluation capability resides in the members.

### `process/`

How the group works day to day. Decisions, open questions, operational principles. This is the group's working memory.

- **[pragma-next.md](process/pragma-next.md)** - The operational log. Changes rapidly, especially in early periods.

### `props/`

PRAGMA Proposals. Numbered proposals that modify PRAGMA documents through group unanimity. The PROP process governs itself.

- **[PROP-000.md](props/PROP-000.md)** - The PROP protocol. Defines the format, lifecycle, and rules for all subsequent PROPs.
- **[PROP-001.md](props/PROP-001.md)** - The agentic condensation rule. Applied to PROP submissions before group review.
- **[PROP-002.md](props/PROP-002.md)** - Commit message questions. Five questions every commit must answer.
- **[PROP-003.md](props/PROP-003.md)** - Membership lifecycle. Size cap, inactivity timeout, emeritus status, succession.

### `chair/`

The chair's working directory. The chair determines its contents. Includes an inbox for formal suggestions and any process materials the chair maintains. Transfers intact on succession.

- **[inbox/](chair/inbox/)** - Proposals for the chair to consider. No suggestion implies obligation.
