---
# Slidev deck: Software development is evolving (SDD)
theme: default
layout: cover
title: "Software Development Isn’t Disappearing — It’s Evolving"
info: |
  Vibe Coding → Context Engineering → Spec-Driven Development
author: "Jacques Camier"
download: true
selectable: true
css: ./styles.css
class: cover
drawings:
  persist: false
transition: slide-left
mdc: true
---

# Software development isn’t disappearing, it’s evolving

<div class="cover-row">
  <img
    class="cover-gif"
    src="/assets/kermit-coding.gif"
    alt="Kermit coding furiously"
  />
  <div class="cover-subtitle">
    From <i>typing code</i> → to <b>designing systems that generate, validate, and evolve code</b> (with agents).
  </div>
</div>

<div class="cover-cards">
  <div class="card">
    <div class="kicker">Explore</div>
    <div class="title">Vibe Coding</div>
    <div class="desc">Fast prototypes</div>
  </div>
  <div class="card">
    <div class="kicker">Stabilize</div>
    <div class="title">Context Engineering</div>
    <div class="desc">Consistent outputs</div>
  </div>
  <div class="card">
    <div class="kicker">Ship</div>
    <div class="title">Spec-Driven Development</div>
    <div class="desc">Production reliability</div>
  </div>
</div>

<!--
Hook: “Don’t believe the hype.” Engineers aren’t going away.
The shift is where the value lives: intent + constraints + verification.

Personal context (optional):
- “Two years ago at DFW Pythoneers we predicted: devs won’t go away;
  devs who don’t leverage AI will be at a disadvantage.”
- “Also predicted: big companies shrink teams, but more companies hire
  smaller teams.”

If you want a quick “macro” datapoint (optional):
- Tech sector growth claim: cite and caveat (varies by definition).
  Source: [TechNoise global count](https://technoise.co.uk/how-many-technology-companies-are-in-the-world-a-global-count/)
- Venture funding headline (optional): [Crunchbase](https://news.crunchbase.com/venture/record-breaking-funding-ai-global-q1-2026/)
-->

---

## What’s changing

### The shift
- We still build software — we’re shifting **where engineering judgment lives**
- Smaller teams, higher leverage, faster iteration
- The craft moves “up” to **intent, constraints, and verification**

<!--
This slide is the “why now” without throwing stats on screen.
-->

---

## Today’s Talk

### Part 1 — The landscape
- The shift, the abstraction stack, the ladder

### Part 2 — Vibe Coding
- Demo + debrief

### Part 3 — Context Engineering

### Part 4 — Spec-Driven Development
- Workflow + demo + validation mindset

### Q&A and Rabbit Holes :rabbit:

<!--
Set expectations: You might go over because the demos are the point.
If time is tight, you can shorten demo #2 and extend SDD.
-->

---

---
layout: statement
class: section
---

# Part 1
## The landscape

<!--
Use this as a clean section divider.
-->

---

## The noise vs the shift

### The noise
- “AI will replace developers.”

### The shift
- We’re moving from writing code line-by-line…
- to **writing intent** that agents can implement and verify.

<!--
Frame: This is an evolution of abstraction, not an extinction event.
-->

---

## A familiar abstraction stack

Specs → Source Code → Machine Code

### What changed
- **Natural language** is now a first-class abstraction layer.
- The engineering question becomes: *How do we make that layer precise and durable?*

<!--
Anchor to your notes: “English has become the high-level abstraction language.”
-->

---

## The ladder: three AI-native ways of building

<div class="three-up">
  <div class="tile vibe">
    <div class="kicker">1) Explore</div>
    <div class="title">Vibe Coding</div>
    <div class="desc">Speed-first exploration</div>
  </div>
  <div class="tile context">
    <div class="kicker">2) Stabilize</div>
    <div class="title">Context Engineering</div>
    <div class="desc">Consistency via curated context</div>
  </div>
  <div class="tile sdd">
    <div class="kicker">3) Ship</div>
    <div class="title">Spec-Driven Development</div>
    <div class="desc">Reliability via contracts + validation</div>
  </div>
</div>

<!--
Set expectation: We’ll do live coding in each mode.
-->

---

---
layout: statement
class: section
---

# Part 2
## Vibe Coding

---

## Part 2 — Vibe Coding

Speed-first exploration.

<!--
Transition line:
“Let’s start with what most people mean by ‘agentic coding’: vibe coding.”
-->

---

## 1) Vibe Coding

### What it is
- Prompt → code → tweak → repeat
- Minimal upfront structure

### When it shines
- Prototyping
- UI experiments
- Exploring ideas

### Failure mode
- Inconsistent architecture
- Hidden bugs accumulate
- Technical debt becomes cognitive debt

---

## Live demo #1 (Vibe)

<div class="demo">
  <div class="demo-head">
    <div class="kicker">Live demo #1</div>
    <div class="title">Vibe Coding</div>
    <div class="desc">Build something fast… and feel the friction.</div>
  </div>
  <div class="demo-grid">
    <div class="demo-card">
      <div class="label">Goal</div>
      <div class="body">Build a small feature <b>fast</b>.</div>
    </div>
    <div class="demo-card">
      <div class="label">Watch for</div>
      <div class="body">
        <ul>
          <li>“Hope-based engineering”</li>
          <li>Drift in naming, layering, assumptions</li>
          <li>The “spec” exists only as chat history</li>
        </ul>
      </div>
    </div>
    <div class="demo-card">
      <div class="label">Debrief</div>
      <div class="body">What would make this maintainable next week?</div>
    </div>
  </div>
</div>

---

## Demo #1 script (Vibe) — keep it intentionally vague

<div class="two-col">
  <div class="col">
    <div class="callout">
      <div class="label">Pick a tiny feature</div>
      <ul>
        <li>A button + small UI behavior, or a tiny endpoint</li>
      </ul>
    </div>
    <div class="callout">
      <div class="label">Prompt style</div>
      <ul>
        <li>One-liner request with missing constraints (on purpose)</li>
      </ul>
    </div>
  </div>
  <div class="col">
    <div class="callout">
      <div class="label">Narrate while it runs</div>
      <ul>
        <li>“We didn’t give architecture, conventions, or validation.”</li>
        <li>“We’re optimizing for speed and surprise.”</li>
      </ul>
    </div>
    <div class="callout subtle">
      <div class="label">Debrief (2 minutes)</div>
      <ul>
        <li>What assumptions did the agent make?</li>
        <li>What became implicit knowledge living only in chat?</li>
        <li>What would future-you need to maintain this?</li>
      </ul>
    </div>
  </div>
</div>

<!--
If you want a concrete example:
“Add a ‘Subscribe’ button that stores an email and shows a success state.”
But keep it vague: no naming conventions, no error behavior, no tests.
-->

---

---
layout: statement
class: section
---

# Part 3
## Context Engineering

---

## 2) Context Engineering

### What it is
You control the **inputs** that shape generation:
- Rules / constraints
- Codebase snippets
- Schemas
- Retrieved docs (RAG)

### Benefit
**Consistency** and fewer bad assumptions.

### Failure mode
Still no single “contract” for the system behavior.

---

## Live demo #2 (Context)

<div class="demo">
  <div class="demo-head">
    <div class="kicker">Live demo #2</div>
    <div class="title">Context Engineering</div>
    <div class="desc">Same feature — but with curated context.</div>
  </div>
  <div class="demo-grid">
    <div class="demo-card">
      <div class="label">Goal</div>
      <div class="body">Build the <b>same</b> feature with guardrails and constraints.</div>
    </div>
    <div class="demo-card">
      <div class="label">Watch for</div>
      <div class="body">
        <ul>
          <li>Better alignment with conventions</li>
          <li>Fewer hallucinated decisions</li>
          <li>Still easy to lose “the why” between sessions</li>
        </ul>
      </div>
    </div>
    <div class="demo-card">
      <div class="label">Debrief</div>
      <div class="body">What survives if we swap agents tomorrow?</div>
    </div>
  </div>
</div>

---

## Demo #2 script (Context) — same feature, better context

<div class="two-col">
  <div class="col">
    <div class="callout">
      <div class="label">Before you prompt, paste guardrails</div>
      <ul>
        <li>File structure expectations</li>
        <li>Naming conventions</li>
        <li>Schema / data model constraints</li>
        <li>Security + validation rules (basic)</li>
        <li><b>Do not change X</b>; only implement Y</li>
      </ul>
    </div>
  </div>
  <div class="col">
    <div class="callout">
      <div class="label">Narrate while it runs</div>
      <ul>
        <li>“Context engineering is input design.”</li>
        <li>“We remove ambiguity to reduce hallucinations.”</li>
      </ul>
    </div>
    <div class="callout subtle">
      <div class="label">Debrief (2 minutes)</div>
      <ul>
        <li>Output is more consistent… but where is the <i>contract</i>?</li>
        <li>If we swap agents tomorrow, what survives?</li>
      </ul>
    </div>
  </div>
</div>

<!--
If time is short, compress this demo:
Show the same request with constraints, then jump to SDD as the durable artifact.
-->

---

---
layout: statement
class: section
---

# Part 4
## Spec-Driven Development

---

## Part 4 — Spec-Driven Development (SDD)

Reliability-first engineering.

<!--
Transition line:
“Now let’s stop ‘prompting’ and start ‘specifying’.”
-->

---

## 3) Spec-Driven Development (SDD)

### What it is
You define behavior first:
- Inputs
- Outputs
- Rules
- Edge cases

Then the agent generates:
- Implementation
- Tests
- Validation logic

### Principle
**Specification (what/why) is decoupled from Implementation (how).**

---

## Why SDD is the professional response

### 1) Leverage
Small changes to the spec can reshape large code changes.

### 2) Anti–context decay
Specs persist between sessions and agents.

### 3) Intent fidelity
The spec forces clarity: success criteria, constraints, flows.

---

## The SDD workflow you can copy

### A) Write the “Constitution”
- **Mission**: why, audience, scope
- **Tech stack**: constraints, defaults, deployment assumptions
- **Roadmap**: phases and features

### B) Feature loop (repeat)
- Plan → implement → validate
- Keep branches and diffs reviewable

---

## Constitution: what it does

### For humans
- Shared agreement on non-negotiables
- Faster onboarding and fewer “silent rewrites”

### For agents
- High-quality context *at boot*
- A stable anchor for decisions

---

## Feature spec: the three artifacts

### 1) Plan
Approach, task groups, sequencing.

### 2) Requirements
Constraints, acceptance criteria, key decisions.

### 3) Validation (scorecard)
How to check success (tests, manual steps, CLI commands, etc.).

---

## Human-in-the-loop: your new core job

You are the architect / supervisor:
- Review for **spec alignment**
- Keep changes **manageable**
- Fix drift by updating **spec + implementation**

### The risk to manage
**AI fatigue**: huge diffs that exhaust review capacity.

---

## Live demo #3 (SDD)

<div class="demo">
  <div class="demo-head">
    <div class="kicker">Live demo #3</div>
    <div class="title">Spec-Driven Development</div>
    <div class="desc">Turn intent into a contract, then generate + validate.</div>
  </div>
  <div class="demo-grid">
    <div class="demo-card">
      <div class="label">Goal</div>
      <div class="body">Build one feature from a <b>mini-spec</b>.</div>
    </div>
    <div class="demo-card">
      <div class="label">Watch for</div>
      <div class="body">
        <ul>
          <li>The spec becomes the durable artifact</li>
          <li>Implementation becomes an execution step</li>
          <li>Validation is explicit (scorecard)</li>
        </ul>
      </div>
    </div>
    <div class="demo-card">
      <div class="label">Debrief</div>
      <div class="body">What changed in your role as “developer”?</div>
    </div>
  </div>
</div>

---

## Demo #3 script (SDD) — the “mini-feature loop”

<div class="two-col">
  <div class="col">
    <div class="callout">
      <div class="label">Step 1 — Write the mini-spec (3–5 min)</div>
      <ul>
        <li>Inputs / outputs / rules / edge cases</li>
        <li>Explicit “won’t do” scope boundary</li>
        <li>Validation checklist</li>
      </ul>
    </div>
    <div class="callout">
      <div class="label">Step 2 — Generate (5–10 min)</div>
      <ul>
        <li>Ask for a plan first</li>
        <li>Then implement</li>
      </ul>
    </div>
  </div>
  <div class="col">
    <div class="callout">
      <div class="label">Step 3 — Validate (5–10 min)</div>
      <ul>
        <li>Run the scorecard</li>
        <li>If something fails: update <b>spec + code</b></li>
      </ul>
    </div>
    <div class="callout subtle">
      <div class="label">Step 4 — Show leverage (optional, 3–8 min)</div>
      <ul>
        <li>Change one line in the spec</li>
        <li>Regenerate / refactor and validate again</li>
      </ul>
    </div>
  </div>
</div>

<!--
Core narration:
“In SDD the spec is the durable artifact. Code is the output.”
-->

---

## A practical mini-spec template (copy/paste)

### Feature
One sentence.

### Inputs / UX
- …

### Outputs
- …

### Rules & edge cases
- …

### Validation
- Tests:
- Manual:

---

## Mini-spec example (good for live demo)

### Feature
Email capture + success state.

### Inputs / UX
- User enters email, clicks Subscribe
- Show inline validation errors

### Outputs
- Success: confirmation message
- Failure: error state with reason

### Rules & edge cases
- Email must be valid format
- Duplicate emails are idempotent (don’t error; return “already subscribed”)

### Validation
- Manual: try invalid, valid, duplicate
- Tests: one per rule

<!--
Swap this for an API example if your audience is backend-heavy.
-->

---

## Greenfield vs Brownfield (legacy)

### Greenfield
Draft constitution in conversation with the agent.

### Brownfield
Reverse-engineer the constitution from:
- Repo structure
- Existing docs / TODOs / tickets
- Constraints implied by code

### Same loop after that
Plan → implement → validate → replan.

---

## Replanning: “run slow to run fast”

After each feature:
- Update constitution if you learned something real
- Improve the workflow (tests, tooling, conventions)
- Decide if scope belongs in replanning or as a new roadmap item

---

## Tooling landscape (lightweight)

SDD is a workflow; tools are interchangeable.

Examples:
- GitHub Spec Kit
- OpenSpec
- BMAD

Key idea:
**Specs live above models, agents, and IDEs.**

---

## The skill that will matter most

### Not “typing faster”
But **converting intention into clear specifications**.

You’ll still code—
but more of your leverage comes from:
- constraints
- contracts
- verification
- system design

---

## Audience takeaway: when to use what

### Use Vibe Coding when
- You’re exploring and speed matters more than longevity

### Use Context Engineering when
- You need consistency across a codebase and team conventions

### Use SDD when
- You need reliability, testability, maintainability, and repeatability

<!--
This slide prevents “SDD for everything” absolutism.
SDD is the backbone; vibe/context remain useful tools.
-->

---

## A simple next-week challenge

Pick one real feature (small but real):
- Write a mini-constitution (1 page)
- Write one feature spec (plan/requirements/validation)
- Let an agent implement
- Validate against the scorecard
- Adjust the spec until it becomes a reliable “memory”

---

## Optional: Q&A prompts (if you have time)

- “What makes a spec *good enough*?”
- “How do you avoid over-specifying?”
- “How do you handle UI/UX specs?”
- “How do you do this on legacy teams?”
- “What does code review become?”

---

## Closing

The best code starts with a great spec.

**Stay the driver of your software.**

<!--
Close with energy: This is engineering returning, not engineering ending.
-->

