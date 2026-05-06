# Implementation Plan

## Project

- Name: `<project-name>`
- Last updated: `<yyyy-mm-dd>`

## Planning Assumptions

- Time horizon: `<quarter/half/year>`
- Team capacity: `<size/constraints>`
- Key risks:
  - `<risk-1>`
  - `<risk-2>`

## Roadmap

### Phase 1: `<phase-name>`

Objective:

`<what this phase proves or delivers>`

Features:

- `<feature-1>`
- `<feature-2>`

Exit criteria:

- [ ] `<criteria-1>`
- [ ] `<criteria-2>`

### Phase 2: `<phase-name>`

Objective:

`<what this phase proves or delivers>`

Features:

- `<feature-1>`
- `<feature-2>`

Exit criteria:

- [ ] `<criteria-1>`
- [ ] `<criteria-2>`

### Phase 3: `<phase-name>`

Objective:

`<what this phase proves or delivers>`

Features:

- `<feature-1>`
- `<feature-2>`

Exit criteria:

- [ ] `<criteria-1>`
- [ ] `<criteria-2>`

---

# Feature Specification

## Feature

- Name: `<feature-name>`
- Status: `draft | approved | implemented | rejected`
- Owner: `<name/team>`

## User Problem

`<Describe the user problem this feature solves.>`

## User Story

As a `<type of user>`,
I want `<capability>`,
so that `<benefit>`.

## Functional Requirements

- FR-001: `<requirement>`
- FR-002: `<requirement>`
- FR-003: `<requirement>`

## Non-Functional Requirements

- NFR-001: Performance: `<latency/throughput expectation>`
- NFR-002: Security: `<security expectation>`
- NFR-003: Reliability: `<failure/retry expectation>`
- NFR-004: Usability: `<user experience expectation>`

## Acceptance Criteria

The feature is accepted when:

- [ ] `<observable behavior>`
- [ ] `<observable behavior>`
- [ ] `<observable behavior>`

## Edge Cases

- `<edge-case-1>`
- `<edge-case-2>`
- `<edge-case-3>`

## Out of Scope

- `<non-goal-1>`
- `<non-goal-2>`

---

# Implementation Tasks

## Pre-Implementation Checklist

Before writing code, the agent must confirm:

- [ ] The feature has clear user value
- [ ] Requirements are testable
- [ ] Acceptance criteria are written
- [ ] Edge cases are listed
- [ ] Existing project patterns were reviewed
- [ ] Security impact was considered
- [ ] No unnecessary abstraction is planned
- [ ] No unrelated refactor is included

## Tasks

### Preparation

- [ ] T001 Inspect existing files: `<paths>`
- [ ] T002 Identify existing patterns to follow
- [ ] T003 Identify test files and test command

### Tests

- [ ] T004 Add or update test for `<behavior>`
- [ ] T005 Add or update test for `<edge case>`

### Implementation

- [ ] T006 Implement `<small behavior>` in `<path>`
- [ ] T007 Implement `<small behavior>` in `<path>`
- [ ] T008 Add error handling for `<case>`

### Validation

- [ ] T009 Run unit tests
- [ ] T010 Run integration tests
- [ ] T011 Run linting
- [ ] T012 Run type checks
- [ ] T013 Manually verify acceptance criteria

## Validation Report

| Check | Status | Evidence |
|---|---|---|
| Unit tests | `<pass/fail/not run>` | `<notes>` |
| Integration tests | `<pass/fail/not run>` | `<notes>` |
| Lint | `<pass/fail/not run>` | `<notes>` |
| Type check | `<pass/fail/not run>` | `<notes>` |
| Acceptance criteria | `<pass/fail>` | `<notes>` |

## Files Changed

| File | Reason |
|---|---|
| `<path>` | `<reason>` |

## Change Log

| Date | Change | Reason |
|---|---|---|
| `<yyyy-mm-dd>` | `<summary>` | `<reason>` |