# Constitution

## Project

- Name: `DFW Pythoneers Website`
- Owner(s): `DFW Pythoneers / Demo Project`
- Last updated: `2026-05-07`

## Mission

### Why this exists

Create a modern community website for DFW Pythoneers that clearly communicates who the group is, what members can expect, and how people can join upcoming Python events.

This project is also a short demo of Spec-Driven Development (SDD): define the project rules and intent first, then let the agent generate the implementation within those constraints.

### Target audience

- Python developers in the Dallas-Fort Worth area
- Beginners who want to learn Python
- Experienced engineers interested in community, talks, workshops, and networking
- Sponsors or speakers interested in supporting the meetup

### Desired outcome

A polished, responsive, single-page website that looks credible enough for a real technical community and can be created quickly during a live demo.

## Business Requirements

- BR-001: The website must quickly explain what DFW Pythoneers is.
- BR-002: The website must make the community feel active, welcoming, and professional.
- BR-003: The website must highlight upcoming events, learning opportunities, and reasons to join.
- BR-004: The website must include clear calls to action such as `Join the Meetup`, `View Events`, or `Become a Speaker`.
- BR-005: The website must visually demonstrate the value of SDD compared with a loose one-shot prompt.

## Scope

### In scope

- Landing page
- Hero section
- About section
- Event highlights section
- Community benefits section
- Speaker/sponsor callout
- Newsletter or join call to action
- Responsive layout
- Polished Tailwind CSS design using the required palette
- Django backend serving basic data through an application structure
- React frontend built with Vite

### Out of scope

- User authentication
- Payment processing
- Real event registration
- Admin dashboard
- External Meetup API integration
- Production deployment
- Complex database models
- Search
- Blog CMS

## Success Criteria

The project is successful when:

- [ ] A user can understand the purpose of DFW Pythoneers within 5 seconds.
- [ ] The homepage looks modern, polished, and suitable for a real community website.
- [ ] The required Tailwind color palette is used consistently.
- [ ] The site is responsive on desktop and mobile.
- [ ] The backend and frontend can run locally.
- [ ] The project demonstrates how SDD creates stronger results than a simple prompt.

## Non-Negotiables

The agent must not violate these:

- Use Django for the backend.
- Use React for the frontend.
- Use SQLite for the database.
- Use Tailwind CSS for styling.
- Use the required DFW Pythoneers color palette.
- Keep the project simple enough to build in a short demo.
- Do not add authentication unless explicitly requested.
- Do not add unnecessary services, queues, containers, or cloud infrastructure.
- Do not add speculative features.

## Coding Standards

The agent must follow:

- Existing project patterns first.
- Simple code over clever code.
- Clear names over abbreviated names.
- Small functions over large functions.
- Python imports must always be at the top of the file.
- JavaScript imports must always be at the top of the file.
- No unused imports.
- No unrelated refactors.
- No speculative abstractions.
- No new dependency without justification.
- Prefer readable, maintainable code over dense code.
- Keep components focused and easy to understand.

## Python Best Practices

- Use a virtual environment.
- Use `uv` for Python dependency management where practical.
- Use Django conventions for project structure.
- Use `black` for Python formatting.
- Use linting before final validation.
- Keep Django views simple for the demo.
- Avoid business logic in settings files.
- Use environment variables only if needed.
- Do not hardcode secrets.
- Keep imports grouped in this order:
  1. Python standard library
  2. Third-party packages
  3. Local application imports

## JavaScript Best Practices

- Use Vite for the React development server and hot reload.
- Use functional React components.
- Keep components small and composable.
- Keep styling in Tailwind classes unless a small CSS file is clearly better.
- Avoid unnecessary state.
- Avoid unnecessary frontend routing for this demo.
- Do not add large UI libraries unless explicitly requested.
- Use meaningful component and variable names.
- Keep imports at the top of each file.

## Quality Bar

All implementation must include:

- clean formatting
- basic validation of the local run commands
- no unrelated file changes
- no generated code that is unused
- no excessive test scaffolding
- no complex architecture beyond the demo need
- a simple README with local setup instructions if time allows

## Agent Role

The agent is responsible for:

- generating the Django backend
- generating the React frontend
- generating the Tailwind configuration
- creating a polished homepage
- creating simple local run instructions
- preserving the SDD constraints
- identifying ambiguity
- making conservative implementation decisions

The agent must not:

- invent new product requirements
- silently change the architecture
- expand scope without approval
- optimize before correctness
- add unnecessary abstractions
- add real integrations that are not required for the demo

## Human Feedback Loop

Human review is required when:

- requirements are ambiguous
- architecture changes
- security or privacy is affected
- new dependencies are introduced
- generated code changes the intended demo scope
- the design feels too plain for a live presentation

## Clarifications

No clarification is required for the initial demo build. The agent should make reasonable choices that preserve the constraints above.
