# Lab 29 — ErrorResponse Envelope

## Fields
`status` · `message` · `correlationId` · optional `violations` array for field‑level errors.

## Violation item shape
Each violation contains: `field`, `error`, and optionally `rejectedValue` (safe, non‑PII).

## Correlation rule
Always echo the inbound correlationId; if missing, generate a synthetic one and include it in every error payload.

## Scope
Pre-lab only.
