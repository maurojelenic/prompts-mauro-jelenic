---
name: mulesoft-api-builder
description: Use this skill when designing, implementing, or reviewing MuleSoft APIs following API-led connectivity, enterprise best practices, error handling standards, observability, and maintainability.
---

# Goal
Design, implement, and review MuleSoft APIs using API-led connectivity and enterprise integration best practices.

# When to use this
Use this skill when:
- designing a new API
- adding a new endpoint
- modifying an existing endpoint
- reviewing API quality
- improving error handling
- aligning a MuleSoft API with API-led connectivity

# Workflow
1. Analyze the current project first.
2. Identify the API-led layer: Experience, Process, or System API.
3. Design the resource and contract properly before coding when needed.
4. Reuse existing project structure, listener config, logging, and error handling.
5. Keep changes minimal and maintainable.
6. Review output for production readiness.

# Rules
- Follow API-led connectivity.
- Do not mix Experience, Process, and System concerns incorrectly.
- Reuse existing listener, logging, and error handling patterns.
- Preserve backward compatibility unless explicitly told otherwise.
- Use readable DataWeave.
- Keep flows modular and maintainable.
- Do not modify unrelated files.
- Avoid risky variable names.
- If the path parameter is named `type`, do not store it in a Mule variable named `type`; use a safe variable name such as `pokemonType`.
- Always explain the plan before coding when implementing changes.
- Always summarize changed files, assumptions, and risks.

# Special case: new project

If the project does not contain a MuleSoft structure (no pom.xml, no mule-artifact.json, no src/main/mule):

Then:

1. Create a complete MuleSoft project structure:
   - pom.xml
   - mule-artifact.json
   - src/main/mule/main.xml
   - src/main/resources/config.yaml

2. Define a minimal but production-ready structure:
   - HTTP Listener config
   - HTTP Request config
   - basic logging
   - basic error handling

3. Then proceed with API design and implementation.

Do NOT assume an existing structure in this case.