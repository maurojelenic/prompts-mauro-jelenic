Act as a senior MuleSoft developer working in an existing enterprise API project.

Analyze the current project first and explain:
- project structure
- API type according to API-led connectivity
- listener configuration
- routing pattern
- naming conventions
- error handling pattern
- logging pattern
- DataWeave style
- contract style if present

Then add a new endpoint following the exact existing conventions.

## Implementation rules
- Reuse the current project structure
- Reuse listener config
- Reuse existing error handling and logging
- Keep the diff minimal
- Do not modify unrelated files
- Preserve backward compatibility
- Use readable DataWeave
- Keep flows modular and maintainable

## API quality requirements
- use correct HTTP method
- use clear resource naming
- validate required inputs
- return meaningful status codes
- avoid risky variable names
- document assumptions
- update contract files if the project uses RAML or OAS
- add or update tests if applicable

## Error handling
- handle invalid input
- handle downstream API failures
- handle unexpected errors
- align with the existing error response strategy

## Output
At the end, show:
- changed files
- design decisions
- contract impact
- error handling behavior
- validation results