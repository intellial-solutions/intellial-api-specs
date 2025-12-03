# Intellial API Specification Repository

This repository serves as the central source of truth for API specifications 
used across all products and services in our organisation.

All specifications follow the **OpenAPI 3.0 standard**.

Interactive Swagger UI docs are automatically published from the `main` branch.

## 📂 Structure

api-specs/
<application-name>/
openapi.yml
CHANGELOG.md
common/
shared-models.yml
common-errors.yml

## 🧩 Key Principles

1. Specs must always remain valid OpenAPI 3.x format
2. All changes require pull request review
3. Each API spec must have versioning and its own changelog
4. All specs are linted using Spectral via CI

## 🌐 Swagger UI Documentation (Auto Published)

- Hosted from `docs/` folder after merge to `main`
- Each application gets its own UI

Example:
https://<org>.github.io/company-api-specs/customer-portal-ui/

## 🧪 API Linting

We validate specs using:
spectral lint <path>

## 🧾 Adding a New API or Service

1. Create folder under `api-specs/<service>`
2. Copy openapi.yml template
3. Update title, description, version
4. Add to CI and create PR
