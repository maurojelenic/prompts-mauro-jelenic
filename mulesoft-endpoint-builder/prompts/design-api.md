Act as a MuleSoft API architect.

Before implementing anything, design this API properly using API-led connectivity and enterprise API best practices.

## Your task
Given the requirement, first define:
- whether this should be an Experience, Process, or System API
- resource structure
- endpoint paths
- HTTP methods
- request/response contracts
- status codes
- error model
- downstream dependencies
- transformation responsibilities
- security considerations
- observability considerations

## Requirements
- Do not mix Experience, Process, and System concerns incorrectly
- Prefer a clean and scalable resource model
- Avoid overloading a single endpoint with too many responsibilities
- Preserve future extensibility
- Keep the design practical, not academic

## Output format
Provide:
1. API classification and justification
2. Resource model
3. Endpoint definitions
4. Request and response examples
5. Error model
6. Risks / tradeoffs
7. Suggested MuleSoft implementation approach

Do not write Mule code yet.
Only design the API first.