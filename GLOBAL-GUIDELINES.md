# Global API Standards

## Naming
- URL paths: kebab-case
/order-history
/customer-profile

## Model Names
- PascalCase
UserBasic, OrderItem, PaginationResponse

## Common Error Structure
All services must import this schema:
ErrorResponse:
type: object
properties:
code:
type: string
message:
type: string
traceId:
type: string

## Examples
Every endpoint MUST include:
- sample request body
- sample successful response
- sample error response

## Versioning
- MAJOR: breaking
- MINOR: new addition
- PATCH: internal fixes
