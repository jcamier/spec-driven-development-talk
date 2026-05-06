# Tech Stack

## Project

- Name: `<project-name>`
- Last updated: `<yyyy-mm-dd>`

## Architecture Summary

`<Describe the system architecture in plain language.>`

## Runtime and Languages

- Backend: `<framework/language/version>`
- Frontend: `<framework/language/version>`
- Package manager: `<tool>`
- Test runner: `<tool>`
- Type checking: `<tool or none>`

## System Boundaries

### Inputs

- `<input-1>`
- `<input-2>`

### Outputs

- `<output-1>`
- `<output-2>`

### External Systems

- `<system-1>`
- `<system-2>`

## Data and Storage

- Primary database: `<database>`
- Cache: `<redis/none>`
- File storage: `<provider/none>`
- Vector storage: `<pgvector/qdrant/chroma/none>`
- Search: `<tool/none>`

## API and Contracts

- API style: `<REST/GraphQL/RPC/events>`
- Contract format: `<OpenAPI/JSON Schema/Pydantic/Zod/etc>`
- Versioning strategy: `<path/header/semantic versioning>`

## Schemas and Invariants

Strong contracts:

- `<schema or model name>`: `<purpose>`
- `<schema or model name>`: `<purpose>`

Rules that must always remain true:

- INV-001: `<business or data rule>`
- INV-002: `<business or data rule>`
- INV-003: `<business or data rule>`

## Infrastructure

- Hosting: `<cloud/platform>`
- Deployment model: `<container/serverless/VM>`
- Environments: `<dev/stage/prod>`
- CI/CD: `<GitHub Actions/etc>`
- Secret management: `<tool>`

## Security

- Authentication: `<approach>`
- Authorization: `<approach>`
- Secrets: `<approach>`
- Sensitive data handling: `<approach>`
- Input validation: `<approach>`

## Observability

- Logging: `<tool/approach>`
- Metrics: `<tool/approach>`
- Tracing: `<tool/approach>`
- Error reporting: `<tool/approach>`

## Performance Constraints

- Latency target: `<target>`
- Throughput target: `<target>`
- Resource constraints: `<CPU/RAM/storage/cost>`
- Scalability assumptions: `<assumptions>`

## Dependency Rules

The agent may add a dependency only when:

- [ ] the current stack cannot reasonably solve the problem
- [ ] the dependency is actively maintained
- [ ] the dependency does not conflict with existing architecture
- [ ] the reason is documented