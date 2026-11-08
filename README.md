# claude-backend-to-frontend-handoff-docs-skill

A Claude Code skill for producing clear API handoff documents that let frontend developers integrate backend work with minimal back-and-forth.

## Overview

A backend handoff should explain the business behavior and technical contract required by the frontend. It should cover endpoints, request and response shapes, authentication, validation, errors, edge cases, and implementation constraints.

This skill helps create a copy-ready handoff after backend API work is complete.

## Main Capabilities

- Summarize completed backend features.
- Document endpoints and HTTP methods.
- Describe request and response DTOs.
- Explain authentication and authorization.
- Document validation rules.
- Capture business logic and state transitions.
- List error codes and expected UI behavior.
- Explain edge cases and known limitations.
- Provide example requests and responses.
- Maintain versioned handoff documents after feedback.

## When to Use It

Use this skill after completing backend work that needs frontend integration. It is especially useful when endpoints contain non-obvious business rules, validation, permissions, or multi-step state changes.

For a simple CRUD API, a concise endpoint and request/response example may be enough.

## Installation

```bash
git clone https://github.com/Brajesh31/claude-backend-to-frontend-handoff-docs-skill.git ~/.claude/skills/backend-to-frontend-handoff-docs
```

## Usage

Invoke the skill when preparing an integration handoff:

```text
/backend-to-frontend-handoff-docs
```

Provide the completed backend implementation, relevant user story, endpoint definitions, DTOs, authentication rules, and known edge cases.

## Recommended Workflow

1. Confirm the feature and intended frontend behavior.
2. Inspect routes, controllers, services, and DTOs.
3. Identify authentication and authorization requirements.
4. Document each endpoint and HTTP method.
5. Include request and response examples.
6. Explain validation and error behavior.
7. Record business rules and state transitions.
8. List edge cases and integration constraints.
9. Save the handoff in the project documentation structure.
10. Review the document against the actual implementation.

## Handoff Document Structure

A useful handoff commonly includes:

- Feature overview and business context.
- Endpoint list and methods.
- Authentication requirements.
- Request parameters and payloads.
- Response structures.
- Validation rules.
- Error codes and UI handling.
- Loading, empty, and failure states.
- Business rules and edge cases.
- Example frontend integration flow.
- Known limitations and open questions.

## Quality Checklist

- Endpoint paths match the implementation.
- DTO fields and types are accurate.
- Required and optional fields are distinguished.
- Auth and permission behavior is clear.
- Error responses are documented.
- Business rules are explicit.
- Examples use valid data.
- Unknown behavior is marked for clarification.
- Handoff version matches the backend change.

## Repository Contents

- `SKILL.md`: Main API handoff workflow and output requirements.
- `README.md`: Documentation structure and validation guidance.

## Practical Principle

The frontend team should not have to reverse-engineer backend behavior from controllers. Document the contract and the business rules that affect the UI.
