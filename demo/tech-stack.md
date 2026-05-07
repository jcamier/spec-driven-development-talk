# Tech Stack

## Project

- Name: `DFW Pythoneers Website`
- Last updated: `2026-05-07`

## Architecture Summary

The project is a small full-stack local development app.

The backend uses Django with SQLite. The frontend uses React with Vite for fast local development and hot reload. Tailwind CSS provides the visual design system. The first version should be a polished single-page community website, not a complex production platform.

## Runtime and Languages

- Backend: `Django + Python`
- Frontend: `React + JavaScript`
- Frontend build tool: `Vite`
- Styling: `Tailwind CSS`
- Database: `SQLite`
- Python package manager: `uv`
- Python environment: local `.venv`
- Python formatting: `black`
- Python linting: use a lightweight lint command if configured
- JavaScript package manager: `npm`
- JavaScript formatting: default Vite/React conventions; Prettier optional only if already installed

## System Boundaries

### Inputs

- Static community content
- Event sample data
- Speaker/sponsor callout content
- Required color palette

### Outputs

- Responsive DFW Pythoneers landing page
- Local Django backend
- Local React frontend
- Optional simple JSON endpoint for homepage content

### External Systems

- None required for the demo

## Required Tailwind Palette

The site must use this palette consistently.

```js
colors: {
  primary: {
    DEFAULT: '#2E5C8F',
    light: '#4A7BB5',
    dark: '#1F3E63',
  },
  secondary: {
    DEFAULT: '#FFD200',
    light: '#FFE04D',
    dark: '#CCAA00',
  },
  accent: {
    DEFAULT: '#E63946',
    light: '#FF6B6B',
    dark: '#B71C2B',
  },
  neutral: {
    900: '#0B0B0B',
    800: '#1A1A1A',
    700: '#2A2A2A',
    300: '#D1D5DB',
    100: '#F3F4F6',
  },
}
```

## Visual Design Direction

The website should feel:

- modern
- technical
- welcoming
- community-oriented
- credible enough for a real developer group

Design guidance:

- Use a bold hero section with strong typography.
- Use the primary blue for structure and trust.
- Use the secondary yellow for energy and calls to action.
- Use the accent red sparingly for highlights.
- Use dark neutral backgrounds for contrast.
- Use cards for events, benefits, and community features.
- Use rounded corners, spacing, and subtle shadows.
- Use responsive layout from mobile to desktop.

## Data and Storage

- Primary database: `SQLite`
- Cache: `none`
- File storage: `none`
- Vector storage: `none`
- Search: `none`

For the demo, homepage data may be hardcoded in React or served from a simple Django JSON endpoint. Prefer the simplest approach that still demonstrates a real full-stack structure.

## API and Contracts

- API style: simple REST-style JSON endpoint if needed
- Suggested endpoint: `/api/homepage/`
- Contract format: plain JSON for demo simplicity
- Versioning strategy: none for demo

Suggested homepage response shape:

```json
{
  "groupName": "DFW Pythoneers",
  "tagline": "Python community, talks, workshops, and practical engineering in Dallas-Fort Worth.",
  "events": [
    {
      "title": "Python Project Night",
      "date": "Next Thursday",
      "description": "Bring a project, ask questions, and build with other Python developers."
    }
  ]
}
```

## Schemas and Rules That Must Always Remain True

Strong contracts:

- Homepage content must include a group name, tagline, event list, and call to action.
- Event cards must include title, date, and description.
- Calls to action must be visible without scrolling on desktop.

Rules that must always remain true:

- INV-001: The site must clearly identify itself as DFW Pythoneers.
- INV-002: The site must not imply real registration or payment exists.
- INV-003: The Tailwind palette must be used instead of random colors.
- INV-004: The demo must remain simple enough to explain quickly.

## Infrastructure

- Hosting: local development only
- Deployment model: local Django server plus Vite development server
- Environments: local development
- Continuous Integration / Continuous Deployment (CI/CD): not required for demo
- Secret management: no secrets required

## Security

- Authentication: none
- Authorization: none
- Secrets: none required
- Sensitive data handling: no sensitive data should be collected
- Input validation: no public input forms required for first version

If a contact form is added, it should be visual-only for the demo unless explicitly requested.

## Observability

- Logging: Django default console logging is enough
- Metrics: none required
- Tracing: none required
- Error reporting: console/browser output during local demo

## Performance Constraints

- The homepage should load quickly in local development.
- Avoid unnecessary dependencies.
- Avoid large image assets unless generated locally or referenced intentionally.
- Keep the first version lightweight and easy to run.

## Suggested Local Commands

Backend:

```bash
uv venv
source .venv/bin/activate
uv pip install django django-cors-headers
python manage.py migrate
python manage.py runserver
```

Frontend:

```bash
npm create vite@latest frontend -- --template react
cd frontend
npm install
npm install tailwindcss @tailwindcss/vite
npm run dev
```

## Dependency Rules

The agent may add a dependency only when:

- [ ] the current stack cannot reasonably solve the problem
- [ ] the dependency is actively maintained
- [ ] the dependency does not conflict with the simple demo architecture
- [ ] the reason is documented

Avoid adding:

- authentication packages
- payment packages
- complex state management
- component libraries
- animation libraries
- background job systems
- Docker unless explicitly requested
