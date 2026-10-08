# Phase 1: Problem Framing

> Status: Draft to be completed and reviewed with the mentor.

Use this template to think through the problem before making technology or
architecture decisions. Keep the final result concise enough to fit on roughly
one page, with the domain diagram stored separately if needed.

## 1. Problem statement

Answer in two or three sentences:

- Who experiences the problem?
- What are they trying to accomplish?
- What difficulty exists today?
- Why is solving it useful?

**Draft:**

<!-- Write your problem statement here. -->

## 2. Goal

Describe the outcome the system should enable. Avoid describing a technical
solution.

**Draft:**

<!-- Write the system goal here. -->

## 3. Actors

For each actor, describe their responsibility and what they need from the
system.

| Actor | Responsibility | Main need |
| --- | --- | --- |
|  |  |  |

## 4. Main use cases

Write short user-focused actions, for example: “View available resources.”

1. 
2. 
3. 
4. 
5. 

## 5. Functional requirements

Describe what the system must do. Use clear, testable statements beginning
with “The system shall...”

- [ ] 
- [ ] 
- [ ] 

## 6. Business rules

Describe rules that must always remain true, independent of the interface or
technology.

- 
- 
- 

## 7. Non-functional requirements

Record only requirements that matter to the first slice. Avoid inventing scale
or performance targets without a reason.

| Quality | Requirement | Why it matters |
| --- | --- | --- |
| Security |  |  |
| Reliability |  |  |
| Performance |  |  |
| Usability |  |  |

## 8. MVP scope

### In scope

- 
- 
- 

### Out of scope

- 
- 
- 

## 9. Assumptions and constraints

Separate current assumptions from confirmed facts so they can be challenged
during the mentor discussion.

| Item | Type | Validation needed |
| --- | --- | --- |
|  | Assumption / constraint |  |

## 10. Domain model

List the main domain concepts before drawing relationships.

| Concept | Meaning | Important attributes |
| --- | --- | --- |
|  |  |  |

Add the resulting diagram to [`../../diagrams`](../../diagrams/README.md) and
link it here.

## 11. Open questions for mentor review

- 
- 
- 

## Phase 1 completion checklist

- [ ] The problem is described without prescribing a solution.
- [ ] Every MVP feature supports a defined use case.
- [ ] Business rules are testable and deterministic where required.
- [ ] In-scope and out-of-scope items are explicit.
- [ ] Assumptions are separated from confirmed requirements.
- [ ] The domain model uses business language rather than framework terms.
- [ ] Open questions are ready for the mentor session.

