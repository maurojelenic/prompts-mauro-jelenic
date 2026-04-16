---
name: mulesoft-api-documenter
description: Use this skill to generate structured, professional documentation for MuleSoft APIs, including endpoint explanations, purpose, request/response details, error handling, and API-led connectivity classification.
---

# Goal
Generate clear, structured, and professional API documentation for MuleSoft projects, suitable for internal teams, onboarding, and long-term maintenance.

# When to use this
Use this skill when:
- documenting an existing MuleSoft API
- explaining endpoints for a team
- preparing internal documentation
- improving readability and maintainability of APIs

Do not use for:
- frontend documentation
- unrelated systems
- marketing content

# Workflow

## 1. Analyze the project
Inspect:
- Mule flows
- endpoints and routes
- listener configuration
- DataWeave transformations
- error handling
- naming conventions

## 2. Identify API type
Classify the API:
- Experience API
- Process API
- System API

Explain why.

## 3. Extract endpoint information
For each endpoint:
- path
- method
- purpose
- input (path params, query params, headers, body)
- output (response structure)
- downstream dependencies
- transformations applied
- error handling behavior

## 4. Describe behavior
Explain:
- what the endpoint does
- how it processes data
- what systems it interacts with
- any important logic or assumptions

## 5. Document clearly
Write documentation in a structured, serious, and professional format.

---

# Documentation standards

- Use clear section headers
- Avoid unnecessary technical noise
- Be precise and direct
- Do not invent behavior
- If something is unclear, explicitly state assumptions
- Keep tone professional and technical
- Make it easy for another developer to understand and maintain

---

# Output format

## API Overview
- Purpose
- API-led classification
- High-level architecture

## Endpoints

For each endpoint:

### [METHOD] /path

**Purpose**  
Explain what this endpoint does.

**Request**
- Path parameters
- Query parameters
- Headers
- Body (if applicable)

**Response**
- Structure
- Example (if possible)

**Processing**
- What happens internally
- Transformations (DataWeave)
- External systems called

**Error Handling**
- Possible errors
- Status codes
- Behavior

---

## Notes
- assumptions
- limitations
- improvement opportunities

---

# Rules

- Do not modify code
- Do not invent functionality
- Do not assume hidden logic
- Always base documentation on actual implementation
- Keep it readable and structured