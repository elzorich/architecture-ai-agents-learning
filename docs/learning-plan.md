# Learning Plan

## Goal

Learn how to approach a software problem systematically: from requirements to
architecture to implementation, and understand where AI and agents add real
value.

## Current learning vehicle

A small booking application with one resource type and a minimal create, view,
and cancel flow. The exact domain remains open until it is confirmed with the
mentor.

## Phases

### Phase 1: Problem Framing

- Define users, use cases, and the MVP scope.
- Write functional and non-functional requirements.
- Create a basic domain model.
- **Output:** one-page scope document and domain diagram.

### Phase 2: System Design & Baseline Architecture

- Design presentation, application, domain, and data layers.
- Select the initial frontend, backend, and storage stack.
- Build the MVP as a monolith.
- Start recording Architecture Decision Records (ADRs).
- **Output:** working MVP, C4 context and container diagrams, and first ADRs.

### Phase 3: Explore Architectures & Stacks

- Compare a modular monolith, microservices, and serverless architecture.
- Compare synchronous APIs and event-driven communication.
- Discuss trade-offs in complexity, cost, scalability, and team size.
- Optionally extract one capability, such as notifications.
- **Output:** trade-off table and updated diagrams.

### Phase 4: Where AI Makes Sense

- Separate deterministic rules from suitable AI features.
- Select one small LLM-powered feature.
- Keep validation and state changes in deterministic application logic.
- **Output:** AI suitability matrix and first AI feature.

### Phase 5: Agents

- Study an agent as an LLM combined with tools, a reasoning loop, and memory.
- Build an assistant that uses controlled application APIs as tools.
- Compare possible architectural placement of the agent.
- Add confirmation, validation, logging, cost controls, and other guardrails.
- Optionally compare a single-agent and multi-agent approach.
- **Output:** working agent and architectural placement notes.

### Phase 6: Retrospective & Next Steps

- Review lessons learned and decisions that would be changed.
- Decide whether to deepen the agent work or apply the foundation to a game.
- **Output:** retrospective and next-project decision.

## Working format

- Discuss requirements, architecture, and reviews during mentor sessions.
- Complete small design or implementation tasks between sessions.
- Review each phase before starting the next one.
- Keep the plan adaptable as understanding changes.

