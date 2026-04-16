# Error handling guidelines

- Separate business errors from technical errors.
- Return meaningful HTTP status codes.
- Reuse the existing project error handling strategy.
- Avoid leaking internal details.
- Handle invalid input gracefully.
- Handle downstream failures clearly.
- Handle unexpected errors consistently.

## Common cases
- 400 Bad Request
- 404 Not Found
- 409 Conflict when relevant
- 500 Internal Server Error
- 502/503/504 for downstream dependency issues when relevant