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

---

## What’s changing

### The shift
- We **still build** software, **but** we’re shifting **where engineering judgment lives**
- Smaller teams, higher leverage, faster iteration
- The craft levels “up” to **architecture, intent, constraints, and verification** away from the actual writing lines of code

![level-up](https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExMzQ4amZhdnpkbHFzdGZpNjhmZ3BkY2F0eXc5MXhyMTVlMW9laXplbCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/fnxbTLqRqIONtWeDSr/giphy.gif)

---

## The Landscape

#### DFW Preditions:
- Two years ago at DFW Pythoneers we predicted: devs won’t go away;
  devs who don’t leverage AI will.”
- We also predicted: big companies will shrink teams, but there will be more tech companies (startups) with smaller teams.”

#### Industry:
- Tech sector continues to grow at 8 - 12 % a year. [source: TechNoise](https://technoise.co.uk/how-many-technology-companies-are-in-the-world-a-global-count/)

- Headlines: "Q1 2026 Shatters Venture Funding Records as AI Boom Pushes Startup Investment To $300B." [source: Crunchbase](https://news.crunchbase.com/venture/record-breaking-funding-ai-global-q1-2026/)

LinkedIn Post this week, May 4th, 2026
<img
  class="landscape-img"
  src="/assets/linked_in_notification_this_week.jpg"
  alt="LinkedIn weekly hiring notification"
/>

---
class: compact-history
---

## The History of Developer's Fears

| Era | Worry at the time | What actually happened |
|---|---|---|
| 1970s-80s (Assembly -> HLLs) | "Compilers replace programmers" | Productivity jumped; value moved to system design |
| 1990s-2000s (Desktop -> Web) | "Web is a toy" | Web became dominant; SaaS/platform work exploded |
| 2010s (On-prem -> Cloud) | "Cloud kills ops jobs" | Roles evolved into DevOps, SRE, platform engineering |
| Late 2000s-2010s (Mobile) | "Too many frameworks" | Mobile development jobs explode |
| 2020s-present (AI agents) | "AI replaces developers" | Coding accelerates; judgment + validation matter more |

**Pattern:** new abstraction -> fear spikes -> productivity rises -> role evolves -> adapters win.
---
layout: two-cols
class: franklin-slide
---

## History Lesson: Build Through Uncertainty

**Benjamin Franklin (1706-1790) built during very bad and uncertain conditions:**
- Short life expectancy (34-37 yrs), limited medicine, war, inequality, weak infrastructure.

### Yet, he still had amazing impact
- Incredible inventions and experiments
- New civic institutions and systems
- Focus on discipline and service-oriented

### Why this matters now
- Uncertainty is normal during major transitions.
- Great builders do not wait for perfect conditions.

**Build anyway - this is how eras change!**

::right::

<img
  class="franklin-img"
  src="/assets/ben_franklin_inventory.jpg"
  alt="Benjamin Franklin inventor"
/>
<p class="franklin-caption">Output over certainty.</p>
---

## The New Abstraction Stack

English Specs → "Compiles" to High-level Source Code (Python) → Compiles to Byte/Machine Code

### What's changed?
- **Natural language (English)** has become the new, high-level abstraction language.

- What are the new syntax rules?
  `Prompt Engineering`

### What stays the same?
-  Domain knowledge expertise required. Designing and solving complex problems.

- The engineering is still: **How do we make the application meet requirements and production grade?**

<img
  class="landscape-img"
  src="/assets/new_compilation.jpg"
  alt="English Computer Compilation"
/>

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

---
layout: two-cols
class: vibe-compact
---

## 1) Vibe Coding

Speed-first exploration.

### What it is
- Prompt → code → tweak → repeat
- Minimal upfront structure

### When it shines
- Rapid Prototyping
- UI experiments
- Exploring ideas
- Almost everyone can do it

### Failure mode
- Inconsistent and haphazard architecture
- Hidden bugs accumulate, big time!
- Technical debt balloons with AI Slop
- False sense of code (Working, Non-Production)

::right::

<img
  class="vibe-img"
  src="https://media.giphy.com/media/ZS57kdXudVqsDX0TLH/giphy.gif"
  alt="Vibe coding hamster"
/>

---

## Live demo #1 (Vibing)

<div class="two-col">
  <div class="col">
    <div class="callout">
      <div class="label">Prompt (all the context)</div>
      <p><code>create the DFW Pythoneers Website</code></p>
    </div>
    <div class="callout">
      <div class="label">Goal</div>
      <ul>
        <li>Build something <b>fast</b> and see what happens.</li>
      </ul>
    </div>
    <div class="callout subtle">
      <div class="label">Watch for</div>
      <ul>
        <li>“Hope-based engineering”</li>
        <li>Drift in naming, layering, assumptions</li>
        <li>The “spec” exists only as chat history</li>
      </ul>
    </div>
  </div>
  <div class="col">
    <div class="callout">
      <div class="label">Narrate while it runs</div>
      <ul>
        <li>“We didn’t give architecture, conventions, or validation.”</li>
        <li>“We’re optimizing for speed and surprise.”</li>
        <li>“This is vibe coding: fast output, low control.”</li>
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

---
layout: two-cols
class: context-compact
---

## 2) Context Engineering

### What it is
You control the **inputs** that shape generation:
- Rules / constraints
- Codebase snippets
- Great prompts and initial context

### Benefit:
- **Better Output** and fewer bad assumptions.

### Failure mode
- No single “contract” for the system behavior and hard to prevent scope/requirements drift.
- Confusion that this is Spec Driven Development.
- Context rot
- Can drift into vibe coding, lol

::right::

<img
  class="context-img"
  src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExbzhzMWo3amw2eTR3YmRxbzBtOXNrNDlkaTRpMmE4OHJrd2tybTRueCZlcD12MV9naWZzX3NlYXJjaCZjdD1n/e6EYL4isGAGo8/giphy.gif"
  alt="DJ Context Engineering"
/>

---

## Live demo #2 (Context)

### Prompt we use (more context, same feature)

```txt
Create the DFW Pythoneers Website.

Tech stack constraints:
- Backend: Django (Python)
- Frontend: React
- Database: SQLite
- Styling: Tailwind CSS

Tailwind palette (must use):
- primary: #2E5C8F (light #4A7BB5, dark #1F3E63)
- secondary: #FFD200 (light #FFE04D, dark #CCAA00)
- accent: #E63946 (light #FF6B6B, dark #B71C2B)
- neutral: 900 #0B0B0B, 800 #1A1A1A, 700 #2A2A2A, 300 #D1D5DB, 100 #F3F4F6
```

---
class: context-demo-compact
---

## Live demo #2 (Context) — run + debrief

<div class="demo">
  <div class="demo-head">
    <div class="kicker">Live demo #2</div>
    <div class="title">Context Engineering</div>
    <div class="desc">Same feature, now with explicit guardrails and constraints.</div>
  </div>
  <div class="demo-grid">
    <div class="demo-card">
      <div class="label">Goal</div>
      <div class="body">Build the <b>same</b> feature with detailed context and compare output quality.</div>
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
      <div class="label">Narrate + Debrief</div>
      <div class="body">
        <ul>
          <li>“Context engineering is input design.”</li>
          <li>“We reduce ambiguity to reduce hallucinations.”</li>
          <li>Output is more consistent… but where is the <i>contract</i>?</li>
          <li>If we swap agents tomorrow, what survives?</li>
        </ul>
      </div>
    </div>
  </div>
</div>


---
class: sdd-compact
---

## 3) Spec-Driven Development (SDD)

**Production-ready, Reliability-first engineering**
- Define the *specification first*, then generate the implementation.
- Specification (what/why) is **decoupled** from implementation (how).

**Define Upfront ("The Constitution")**
- Business requirements + use case
- Architecture + constraints (inputs/outputs)
- Acceptance criteria + edge cases
- Coding standards

**Agent Role**
- Generate code, tests, validation logic

**Built-in Quality**
- Strong contracts (schemas, APIs, invariants)
- Constrained, verifiable outputs
- Automated validation

**Human Feedback Loop (HFL)**
- Refine the spec (upstream), Guide output (downstream)

<img
  class="sdd-float-img"
  src="/assets/spec_driven_development.jpg"
  alt="AI Dev Engineer"
/>

---

## Why SDD is the New AI Development Paradigm
- Allows developers to make production-grade application using AI Agents
- Requires domain knowledge expertise, skill, art, intelligence and judgement
- AI is automating tasks (typing code) not the ability to solve problems and build solutions (engineering)

### 1) Leverage
Small changes to the spec can reshape large parts of the system.

### 2) Anti–context decay
Specs persist across sessions, agents, and time.

### 3) Intent fidelity
The spec enforces clarity: success criteria, constraints, and flows.

### 4) Verifiability
Specs enable automated validation: tests and rules the system must always follow to ensure correct behavior.
---
layout: center
class: short-video
---

<div class="shorts-wrap">
  <iframe
    src="https://www.youtube.com/embed/MscLPdZVMA0"
    title="SDD short video"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    allowfullscreen
  ></iframe>
</div>

---

## The SDD Workflow Standardized (3 docs only)

This is simplied to just **3 artifacts**:
- Some use 5, 6, 7 😉, etc...

- `constitution.md` → business requirements, mission, scope, quality bar
- `tech-stack.md` → architecture, contracts, invariants, stack constraints
- `implementation-plan.md` → phases, features, exit criteria, feature specs

### Execution loop (repeat)
- Plan → implement → validate
- Keep branches and diffs reviewable

### Note
Another way to do this is [GitHub Spec Kit](https://github.com/github/spec-kit). With 11 folders and who knows how many files... 😅

<div class="workflow-qr-wrap">
  <img
    class="workflow-qr"
    src="/assets/github_spec_qr.png"
    alt="QR code to GitHub Spec Kit"
  />
  <p class="workflow-qr-caption">Scan for Spec Kit</p>
</div>


---
layout: two-cols
class: constitution-compact
---

## Constitution: what it does

### For humans
- Shared agreement on non-negotiables
- Faster onboarding and fewer “silent rewrites”

### For agents
- High-quality context *at boot*
- A stable anchor for decisions

::right::

<img
  class="constitution-img"
  src="/assets/constitution.jpg"
  alt="Spec Constitution"
/>

---


## Human Feedback Loop (HFL):
- You, the engineer, have agency and use judgment to review, redirect, and approve the agent’s work

### You are the architect / AI supervisor:
- Review for **spec alignment**
- Keep changes **manageable**
- Fix drift by updating **spec + implementation**

### The risk to manage:
**Cognitive fatigue**: huge diffs that exhaust review capacity.
- Work within your context limits, not your Agents.
- Ultimately, you have agency and you will be held accountable for your work, not the AI Agents

---
class: sdd-demo-compact
---

## Live demo #3 (SDD)

### Artifact 1 — `demo/constitution.md`

Live view from the demo artifact (auto-updates when file changes):

<script setup>
import constitutionArtifact from '../demo/constitution.md?raw'
</script>

<pre><code>{{ constitutionArtifact }}</code></pre>

---
class: sdd-demo-compact
---

## Live demo #3 (SDD)

### Artifact 2 — `demo/tech-stack.md`

Live view from the demo artifact (auto-updates when file changes):

<script setup>
import techStackArtifact from '../demo/tech-stack.md?raw'
</script>

<pre><code>{{ techStackArtifact }}</code></pre>

---
class: sdd-demo-compact
---

## Live demo #3 (SDD)

### Artifact 3 — `demo/implementation-plan.md`

Live view from the demo artifact (auto-updates when file changes):

<script setup>
import implementationPlanArtifact from '../demo/implementation-plan.md?raw'
</script>

<pre><code>{{ implementationPlanArtifact }}</code></pre>

---
class: sdd-demo-compact
---

## Live demo #3 (SDD) — run + debrief

<div class="demo">
  <p class="demo-intro">Turn intent into a contract, then generate + validate.</p>
  <div class="demo-grid">
    <div class="demo-card">
      <div class="label">Goal</div>
      <div class="body">Build one feature from the three artifacts in <b>demo/</b>.</div>
    </div>
    <div class="demo-card">
      <div class="label">Watch for</div>
      <div class="body">
        <ul>
          <li>Specs drive implementation decisions</li>
          <li>Code generation follows explicit constraints</li>
          <li>Validation gates are visible and repeatable</li>
        </ul>
      </div>
    </div>
    <div class="demo-card">
      <div class="label">Narrate + Debrief</div>
      <div class="body">What changed in your role as “developer” when the spec becomes the source of truth?</div>
    </div>
  </div>
</div>

---

## Questions ???




