# Engineering Log

This is the chronological record of the apprenticeship. Entries are maintained by the Senior Engineer and summarize meaningful work, decisions, discoveries, mistakes, and the next engineering direction.

## 2026-10-04 — Apprenticeship Initialized

### Session

Repository infrastructure was created for the long-term cybersecurity engineering apprenticeship.

### Work Completed

- Created the public `cyber-apprenticeship` GitHub repository.
- Created the initial workspace directories for application, infrastructure, security, labs, and documentation.
- Added the repository `.gitignore` with protection for common secrets, credentials, local environments, build artifacts, logs, and private keys.
- Configured SSH authentication for GitHub.
- Successfully pushed the initial workspace commit to the `main` branch.
- Connected the repository to the Senior Engineer workflow so repository state can be inspected and maintained across future sessions.

### Engineering Lesson

GitHub authentication for Git operations should use SSH or a supported token-based mechanism rather than a normal GitHub account password. SSH is now configured for this workstation.

### Current Position

The repository is intentionally almost empty. No application technology has been selected yet. Product requirements and architecture will be defined before implementation begins.

## 2026-10-04 — Product Direction and Baseline Review

### Session

The product direction was deliberately taken away from the intern. The Senior Engineer selected **Sentinel — Production Operations & Security Platform** because a central operations/security platform can naturally create engineering problems spanning application development, infrastructure, networking, deployment, monitoring, and cybersecurity.

### Product Concept

Sentinel will provide centralized visibility and operational/security management across multiple software projects. A project may contain people, services, deployments, logs, alerts, and incidents. The long-term goal is to connect software development, production operations, and security workflows rather than build an isolated CRUD application.

### Intern Baseline

The intern correctly recognized the central-visibility purpose and identified useful roles: developers, project administrators, a central Sentinel administrator, and security engineers. The intern also correctly identified deployment metadata such as version, actor, time, and outcome, and had the basic intuition that alerts precede or trigger investigation while incidents represent events requiring response.

The main knowledge gaps were expected at this stage: service/component concepts, automatic event generation, application/API architecture, system boundaries, reverse proxies, load balancers, and the distinction between authentication and authorization.

### Engineering Lessons Introduced

- Manual reporting by developers should be minimized; useful activity should be generated and exchanged by systems where possible.
- A service is a distinct software component with a particular responsibility inside a larger system.
- An alert is a signal requiring attention; an incident is a confirmed or sufficiently serious event requiring investigation and response. Not every alert becomes an incident.
- A basic web application commonly separates frontend, backend/API, and database responsibilities.
- An API is a defined interface through which software components communicate.
- A reverse proxy sits in front of application servers and can provide routing, TLS termination, rate limiting, and related edge functions.
- A load balancer distributes traffic across multiple application instances.
- Security must include identity, authorization, data, infrastructure, application behavior, and auditability rather than only database protection.

### Decision

The intern will not choose the product, primary architecture, or technology stack merely from personal familiarity. The Senior Engineer owns the direction and will justify major choices based on requirements, learning value, and realistic engineering practice.

### Next

Formalize Sentinel's initial functional and non-functional requirements, define actors and the system boundary, and establish the first system-context architecture.
