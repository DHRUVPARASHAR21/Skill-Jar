---
name: idea-to-project
description: "Turn an already-explored product idea, brief, or research notes into a reviewable project foundation before implementation. Use after ideation, not for building or modifying an existing project."
---

# Idea To Project

Create a durable, right-sized handoff from an idea to a build-ready project. Preserve the user's product choices; make reasonable assumptions where they are low-impact and clearly record them.

## Scope and boundary

- Use this after the user has explored an idea in chat, research, a brief, or notes and wants to initiate a new project.
- Do not write application code, scaffold a framework, install dependencies, deploy, create external accounts, or make external changes unless the user separately asks after reviewing the groundwork.
- Do not turn a prototype into an enterprise process. Match the amount of planning to the project's risk, ambiguity, and expected lifetime.

## Workflow

1. Inspect the supplied material and any existing target directory. If a repository already exists, read its applicable `AGENTS.md` files and preserve its conventions.
2. Identify only the decisions that materially block useful planning. Ask concise questions when needed; otherwise state assumptions in the artifacts.
3. Create or update the following project-local files, adapting names and detail to established repository conventions:
   - `docs/intent.md`: problem, target users, outcome, constraints, non-goals, and open questions.
   - `docs/spec.md`: user flows, functional requirements, quality requirements, acceptance criteria, and a proportionate architecture/data outline.
   - `docs/plan.md`: ordered milestones, proposed modules or files, verification strategy, dependencies, risks, and decisions needing approval.
   - `AGENTS.md`: concise instructions for future agent sessions: stack, commands once known, conventions, quality expectations, and protected boundaries.
4. For an early prototype, keep the spec and plan brief. For a higher-risk or long-lived project, make the acceptance criteria, security/privacy constraints, operational assumptions, and test/release approach explicit.
5. Present a compact summary of the proposed stack, key assumptions, scope boundary, and unresolved decisions. Stop and request approval before implementation.

## Quality bar

- Make each artifact readable by both a human collaborator and a later agent session without relying on the originating chat.
- Treat `intent.md` as the source for why; `spec.md` for what; `plan.md` for how. Avoid duplicating prose across them.
- Prefer concrete, testable acceptance criteria over vague promises.
- Record unknowns and tradeoffs rather than silently inventing product requirements.
- When an existing project has its own planning structure, use that structure rather than forcing these filenames.
