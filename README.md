## SpecDriven (talk materials)

This repo contains a Slidev presentation on where software development is
going: **Vibe Coding -> Context Engineering -> Spec-Driven Development**.

### Repo layout

- `presentation/`: Slidev deck (`slides.md`, `styles.css`, assets)
- `demo/`: live demo artifacts rendered inside SDD demo slides
- `templates/`: reusable starter templates for SDD artifacts

### Share with others

- To share a working deck exactly as-is, share **both** `presentation/` and
  `demo/`.
- The SDD artifact slides load content from `demo/*.md`; sharing only
  `presentation/` will break those live artifact slides unless paths are
  changed.

### Run the slides (Slidev)

#### Prereqs

- Node.js (>= 20.19) recommended

#### Install dependencies

```bash
cd presentation
npm install --include=optional
```

#### Present locally

```bash
cd presentation
npx slidev slides.md --open
```

#### Present with local-only private slides

Use the gitignored local wrapper deck when you want private content
(for example a personal bio slide that should never be committed):

```bash
cd presentation
npx slidev slides.local.md --open --port 3031
```

#### Export (PDF / PPTX / PNG)

```bash
cd presentation
npx slidev export slides.md
```

#### Live artifact behavior

- The three SDD artifact slides in `presentation/slides.md` read from:
  - `demo/constitution.md`
  - `demo/tech-stack.md`
  - `demo/implementation-plan.md`
- Editing those files updates slide content on hot reload (or browser refresh).

#### If you hit native binding errors (macOS / arm64)

Slidev uses native bindings via `rolldown` / `oxc-parser`. If you see
"Cannot find native binding", do a clean local install:

```bash
cd presentation
rm -rf node_modules package-lock.json
npm install --include=optional
```

Reference: https://sli.dev/guide/

