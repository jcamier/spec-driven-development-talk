## Run the slides (Slidev)

### Prereqs
- Node.js \(>= 20.19\) (recommended)

### Install

```bash
npm i -g @slidev/cli
```

### Present locally

```bash
cd presentation
npx slidev slides.md --open
```

### Export (PDF / PPTX / PNG)

```bash
cd presentation
npx slidev export slides.md
```

### If you hit native binding errors (macOS / arm64)

Slidev uses native bindings via `rolldown` / `oxc-parser`. If you see
“Cannot find native binding”, do a clean local install:

```bash
cd presentation
rm -rf node_modules package-lock.json
npm install --include=optional
```

Reference: `https://sli.dev/guide/`

