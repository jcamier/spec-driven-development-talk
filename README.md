## SpecDriven (talk materials)

This repo contains a Slidev presentation on where software development is going:
**Vibe Coding → Context Engineering → Spec-Driven Development**.

### Share with others

- **Share just the deck**: copy the `presentation/` folder.
- Research notes / transcripts live under `resources/` and are intentionally ignored by git.

### Run the slides (Slidev)

#### Prereqs
- Node.js \(>= 20.19\) (recommended)

#### Install

```bash
npm i -g @slidev/cli
```

#### Present locally

```bash
cd presentation
npx slidev slides.md --open
```

#### Export (PDF / PPTX / PNG)

```bash
cd presentation
npx slidev export slides.md
```

#### If you hit native binding errors (macOS / arm64)

Slidev uses native bindings via `rolldown` / `oxc-parser`. If you see
“Cannot find native binding”, do a clean local install:

```bash
cd presentation
rm -rf node_modules package-lock.json
npm install --include=optional
```

Reference: `https://sli.dev/guide/`

