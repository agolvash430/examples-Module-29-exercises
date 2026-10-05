# Lab 29 — GlobalExceptionHandler TODOs

## Advice annotation
`@RestControllerAdvice` to centralize error shaping for all controllers.

## Handlers (list)
Handle:
- Validation errors (`MethodArgumentNotValidException`)
- Not‑found domain errors (`CustomerNotFoundException`)
- Forbidden/authorization errors
- Generic fallback (`Exception`) for unexpected failures

## 500 rule
Never leak stack traces or internal exception names; return a safe 500 payload with correlationId and a generic message.

## Scope
Pre-lab only.
