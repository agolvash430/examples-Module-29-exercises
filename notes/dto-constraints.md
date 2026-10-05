# Lab 29 — DTO Constraint Plan

| Field | Constraints |
| --- | --- |
| fullName | Not blank; length > 1; trim and reject pure whitespace |
| email | Not blank; must match email format; lowercase normalization |
| status | Must be one of allowed enum values (ACTIVE, PROSPECT); reject invalid/misspelled |

## How triggered
Constraints fire during request‑body binding/validation (`@Valid` + `@NotBlank` + custom enum validator), producing 400 with field‑level errors.

## Scope
Pre-lab only.
