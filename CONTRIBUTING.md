# Contribution Rules

## Pull Requests

Every API modification must be submitted through a PR.

### PR Must Contain:
- Updated `openapi.yml`
- Version bump (`info.version`)
- CHANGELOG.md entry
- Lint passed
- No unresolved warnings

### PR Naming Format:
[<ServiceName>] <Short Description>

Example:
[CustomerPortal] Add OTP validation endpoint

### Required Checks:
- Spectral linting must pass
- Reviewer approval required
- Breaking changes must be tagged with MAJOR version increment

---

## Developer Checklist

Before raising PR:
- Run `spectral lint`
- Check backward compatibility
- Provide complete examples (request & response)
- Use shared models where applicable
- Follow global naming rules

---

## Breaking Changes

Require:
- Architecture team approval
- `MAJOR` version bump
- Migration notes in CHANGELOG.md
