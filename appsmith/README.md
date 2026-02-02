


# Appsmith Instance Management API Specification

## Project Overview
I created a standardized OpenAPI 3.1.1 specification for Appsmith's self-hosted management endpoints. Previously, these endpoints were only documented in static prose, making it difficult for DevOps engineers to integrate them into automated monitoring tools.

## Key Challenges
* **Complex Nesting:** The `/consolidated-api/view` endpoint returns deeply nested JSON. I modelled this using recursive schemas to ensure technical accuracy.
* **Reusability:** I implemented `components/schemas` to follow the DRY (Don't Repeat Yourself) principle, allowing the `ResponseMeta` object to be reused across multiple endpoints.
* **Security Modeling:** Defined `apiKey` security schemes to reflect the authentication required for admin-level data.

## Tools Used
* **OpenAPI 3.1.1**
* **Swagger Editor** (Validation)
* **Redocly** (Rendering)
