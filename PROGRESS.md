# Apprenticeship Progress

## Current Phase

**Phase 1 — Product Definition and Requirements**

## Product

**Sentinel — Production Operations & Security Platform**

Sentinel is a centralized platform for organizations that operate multiple software projects. It will provide a common view of projects, people, services, deployments, logs, alerts, and security incidents so engineering and security teams do not have to operate each project in isolation.

The application is deliberately being built as a learning vehicle for the apprenticeship. Its lifecycle will progressively expose the intern to software development, web architecture, networking, Linux, databases, authentication, infrastructure, containers, CI/CD, cloud, application security, observability, detection engineering, and incident response.

## Current Assignment

**ASSIGNMENT-001 — Requirements Review**

### Status

**COMPLETED — BASELINE REVIEWED**

The intern produced an initial understanding of Sentinel without researching the unknown concepts first. The baseline showed good product intuition but limited familiarity with web/application architecture and operations terminology.

## What the Intern Currently Understands

- Sentinel is intended to provide centralized visibility across multiple projects.
- Different roles will require different levels of access, including developers, project administrators, a central Sentinel administrator, and security engineers.
- Deployments should retain information such as version, time, actor, environment, and success/failure status.
- Alerts and incidents are different stages of a security/operations workflow.
- Security requires protecting more than databases: identity, authorization, data, infrastructure, applications, and audit trails all matter.

## Concepts Introduced During Review

- A service is a distinct software component that performs a particular function within a larger system.
- Developers should not manually report every activity; systems should generate and exchange useful events automatically where possible.
- An alert indicates something requiring attention; an incident is a confirmed or sufficiently serious event requiring investigation/response.
- A basic web application commonly separates frontend, backend/API, and database responsibilities.
- An API provides a communication interface between software components.
- A reverse proxy sits in front of application servers and can provide routing, TLS termination, rate limiting, and related edge functions.
- A load balancer distributes traffic across multiple application instances.

## Requirements Direction

The first requirements baseline is now being formalized by the Senior Engineer. The intern is not expected to choose the product or technology stack. Technology and architecture will be selected only after requirements justify them and their learning value is understood.

## Next Engineering Milestone

Formalize Sentinel's initial functional and non-functional requirements, define the system boundary and actors, then produce the first system-context architecture.

## Synchronization Rule

At the beginning of a future session, the Senior Engineer should inspect the repository state, recent commits, progress documentation, architecture/decision records, and relevant source code before assigning the next task.

## Documentation Ownership

The intern is not responsible for manually maintaining the apprenticeship Markdown state files unless explicitly instructed. The Senior Engineer maintains them so they remain synchronized with the actual project and apprenticeship state.
