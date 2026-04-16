# API-led connectivity guidelines

## API classification
- Experience API: tailored for channel/client experience.
- Process API: orchestration, aggregation, business process logic, transformations across systems.
- System API: direct interaction with backend systems with minimal business logic.

## Rules
- Do not mix concerns across layers unless explicitly required.
- Justify the API classification before implementation.
- Keep Experience APIs consumer-focused.
- Keep Process APIs orchestration-focused.
- Keep System APIs backend-focused and thin.