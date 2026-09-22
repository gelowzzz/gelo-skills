# System Definition Output Template

Use this section order. Omit instructional brackets from the final deliverable.

```markdown
# System Definition: [System Name]

## 1. System Overview

[What is being built and its purpose in one short paragraph.]

## 2. Problem / Current State

[How the work or experience happens today, what is painful or insufficient, and why change is needed.]

## 3. Users

| User or role | What they need to accomplish |
| --- | --- |
| [Role] | [Goal] |

## 4. Core Workflows

### [Workflow name]

[Trigger] → [Step] → [Step] → [Outcome]

## 5. Critical Business Rules & Known Exceptions

### Business Rules

- [Rule that materially shapes behavior]

### Known Exceptions

- [Common variation or failure already known]

## 6. Success

- [Observable or measurable outcome]

## 7. Scope Boundary

### In Scope

- [Current capability or workflow]

### Outside Current Scope

- [Explicit exclusion or deferred area]

## Open Questions for PRD

- [Important but nonblocking question, if any]
```

Keep workflows behavioral, not screen-based. Keep rules separate from exceptions. Write outcomes rather than features. Do not add technical design sections.
