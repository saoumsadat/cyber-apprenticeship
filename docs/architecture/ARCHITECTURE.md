# Architecture Record

## Status

**Requirements / pre-architecture**

No production application architecture has been finalized yet.

## Product

**Sentinel — Production Operations & Security Platform**

Sentinel is intended to provide centralized visibility and operational/security management across multiple software projects operated by an organization.

## Current System Concepts

The first product discussion established these conceptual entities:

- Organization / central Sentinel environment
- Projects
- People and roles
- Services
- Deployments
- Logs / events
- Alerts
- Incidents
- Security and audit information

These are product concepts only. They are not yet a finalized database schema or technical architecture.

## Initial Actor Model

Expected actors include:

- **Developer** — works on project services and participates in development/deployment workflows.
- **Project Administrator** — manages project membership, permissions, and project-level administration.
- **Central Administrator** — manages the Sentinel environment itself and organization-wide configuration.
- **Security Engineer** — reviews security activity, alerts, incidents, and audit information across projects.

End consumers of the underlying projects are not expected to be primary Sentinel users.

## Architectural Direction

The eventual system is expected to connect a web frontend, backend/API, persistent data storage, and operational/security components. The exact component boundaries, technologies, deployment topology, and integration mechanisms will be determined after formal requirements are established.

A conceptual application path currently used for learning is:

`User → Frontend → Backend/API → Database`

This is only a teaching baseline and must not be treated as the final architecture.

## Planned Evolution

The architecture will be recorded progressively:

1. Product requirements
2. System context and actors
3. High-level components
4. Data model
5. Application/API architecture
6. Deployment architecture
7. Security architecture
8. Observability architecture
9. Scaling and reliability considerations

## Architectural Constraint

Technology choices must be justified by requirements and learning value. We will not select a large technology stack simply because it is popular.

## Decision Record Rule

Every significant architectural decision should record the problem, alternatives considered, decision, and consequences in `docs/decisions/`.
