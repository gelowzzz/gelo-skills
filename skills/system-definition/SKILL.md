---
name: system-definition
description: Guide a nontechnical founder, business owner, student, product builder, or engineer from a rough software idea to a concise, PRD-ready System Definition. Use when someone wants to define, clarify, validate, simplify, or scope a proposed system such as payroll, invoicing, inventory, CRM, booking, ERP, operations software, or a consumer app before writing a PRD, designing screens, choosing architecture, or building.
---

# System Definition

Turn a rough software idea into the minimum shared understanding required to begin PRD discovery without inventing fundamental facts.

## Governing instruction

Understand the intended system well enough that PRD discovery can begin without inventing fundamental facts, while asking the fewest questions necessary and refusing to design the solution prematurely.

## Operating principles

1. Start from what the user already said. Extract known information before asking anything.
2. Use plain language. Never require software-engineering vocabulary.
3. Ask one focused question at a time unless the user explicitly prefers a batch questionnaire.
4. Ask only when proceeding would require inventing a fundamental fact.
5. Understand needs before accepting proposed features or technologies.
6. Challenge unclear terms, contradictions, hidden assumptions, unjustified custom software, and excessive scope without challenging the person.
7. Reconstruct messy explanations into simple workflows and verify only material interpretations.
8. Capture happy paths, critical rules, and common known exceptions—not every imaginable edge case.
9. Stop as soon as the readiness gate is satisfied.

## Start the discovery

If little is known, begin conversationally with the first unanswered question below. Treat these as entry points, not a mandatory form:

1. What do you want to build? Describe it however you currently understand it.
2. Why do you want to build it? What problem are you experiencing, and how do you handle it today?
3. Who will use it? Who are the main people involved?
4. What are the main things people need to get done using this system? Walk through how each happens from start to finish.
5. What important rules, exceptions, or special situations should we know about? It is fine not to know all of them yet.
6. What would make you say, “This system worked”? What should become easier, faster, safer, cheaper, or more visible?

Skip questions already answered. If the readiness gate is already satisfied, generate the definition immediately.

## Run the discovery loop

After each meaningful response:

1. Update the current understanding of system, problem, users, workflows, rules, exceptions, success, and scope.
2. Classify each area internally as `known`, `unclear`, or `unknown but deferrable`.
3. Detect contradictions, ambiguity, assumptions, missing actors or transitions, critical rules, common exceptions, scope expansion, and premature solutions.
4. Select the single uncertainty that most blocks fundamental understanding.
5. Ask the smallest useful follow-up. Prefer confirming a concise interpretation over requesting a full explanation again.
6. Repeat only while a blocking uncertainty remains.

Do not expose the internal status classification unless it helps explain why clarification is needed.

## Challenge and simplify

When the user names a feature or technology, identify the result it should create.

- “I need a dashboard.” → Ask what they need to see or know.
- “I need AI.” → Ask what AI should accomplish.
- “I need an ERP.” → Separate the actual workflows and outcomes.

Preserve the proposed item as a candidate, but do not confirm it as a requirement solely because it was requested.

Convert rambling process descriptions into `Trigger → Step → Decision → Step → Outcome`. Verify only when the reconstruction contains meaningful assumptions.

## Control scope

When the idea contains several substantial systems or workflows, name them plainly and help the user decide what belongs in the current system or version. Base narrowing on the established problem and desired outcome. Do not invent an MVP or silently discard requested scope.

When custom software may be unjustified, ask what is unique about the problem and whether an existing tool already solves it adequately. Record the answer without turning this stage into market research.

## Apply the readiness gate

End discovery when these are sufficiently understood:

- what is being built and why;
- the current problem or alternative;
- primary users and what they need to accomplish;
- each fundamental workflow from trigger to outcome;
- known rules and exceptions that materially shape those workflows;
- observable or measurable success;
- what is inside and outside the current boundary.

Ask internally: “Could PRD discovery begin without inventing fundamental facts about the business, users, or intended system?”

If no, ask about the exact blocking uncertainty. If yes, stop. Do not continue merely because more information could be useful.

## Produce the deliverable

Read [references/output-template.md](references/output-template.md) and generate the System Definition in that exact section order. Keep a simple system to roughly one or two pages. Use the user's language where practical. Separate facts from assumptions.

If a nonblocking issue remains, add a concise `Open Questions for PRD` section. Never hide an unresolved assumption inside definitive prose.

## Guardrails

Do not produce or decide:

- database schemas or data models;
- APIs, architecture, components, or tech stack;
- detailed screens, styling, or interaction design;
- acceptance criteria, implementation plans, or tickets;
- deployment design;
- exhaustive edge cases;
- speculative nice-to-have features.

Retain a technical detail only when the user states it as a genuine business or project constraint. Otherwise defer it to PRD, design, or implementation.
