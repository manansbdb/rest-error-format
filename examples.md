# Examples / Exemplos

## English

| HTTP | code | when |
|------|------|------|
| 400 | `VALIDATION_FAILED` | Bad input |
| 401 | `UNAUTHORIZED` | Missing/invalid auth |
| 403 | `FORBIDDEN` | Authenticated but not allowed |
| 404 | `NOT_FOUND` | Resource missing |
| 409 | `CONFLICT` | State conflict |
| 429 | `RATE_LIMITED` | Too many requests |
| 500 | `INTERNAL_ERROR` | Unexpected failure |

Always include a stable machine-readable `code` and a human `message`.

## Português

| HTTP | code | quando |
|------|------|--------|
| 400 | `VALIDATION_FAILED` | Input inválido |
| 401 | `UNAUTHORIZED` | Auth em falta/inválida |
| 403 | `FORBIDDEN` | Autenticado sem permissão |
| 404 | `NOT_FOUND` | Recurso inexistente |
| 409 | `CONFLICT` | Conflito de estado |
| 429 | `RATE_LIMITED` | Demasiados pedidos |
| 500 | `INTERNAL_ERROR` | Falha inesperada |

Inclua sempre um `code` estável e uma `message` humana.
