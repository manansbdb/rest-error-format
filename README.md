<p align="center">
  <img src="docs/banner.svg" alt="REST Error Format banner" width="100%" />
</p>

<h1 align="center">rest-error-format</h1>

<p align="center">
  <strong>EN</strong> Standardized JSON error envelope for REST APIs<br/>
  <strong>PT</strong> Envelope JSON padronizado para erros REST
</p>

<p align="center">
  <a href="https://github.com/manansbdb/rest-error-format/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-22c55e?style=for-the-badge" alt="MIT" /></a>
  <img src="https://img.shields.io/badge/lang-EN%20%7C%20PT-3b82f6?style=for-the-badge" alt="EN PT" />
  <img src="https://img.shields.io/badge/topic-REST-ef4444?style=for-the-badge" alt="REST" />
  <a href="#support--apoio"><img src="https://img.shields.io/badge/donate-BTC-f59e0b?style=for-the-badge" alt="Donate BTC" /></a>
</p>

---

## What it does / Para que serve

| English | Português |
|---------|-----------|
| A **standard JSON error envelope** plus examples so clients parse failures consistently. | Um **envelope JSON de erro** padrão e exemplos para clientes tratarem falhas de forma consistente. |
| Adopt the shape in middleware and document it in your OpenAPI. | Adota o formato no middleware e documenta-o no OpenAPI. |

```mermaid
flowchart LR
  A["⚠️ Handler error"] --> B["📦 error-envelope.json"]
  B --> C["🌐 HTTP 4xx/5xx"]
  C --> D["📱 Client parses"]
  style A fill:#f97316,stroke:#c2410c,color:#fff
  style B fill:#ef4444,stroke:#b91c1c,color:#fff
  style C fill:#6366f1,stroke:#4338ca,color:#fff
  style D fill:#14b8a6,stroke:#0f766e,color:#fff
```

---

## Install / Instalação

### 1) Clone / Clona

```bash
git clone https://github.com/manansbdb/rest-error-format.git
cd rest-error-format
```

### 2) Apply / Aplica

```bash
mkdir -p docs/api
cp error-envelope.json docs/api/
cp examples.md docs/api/error-examples.md
# mirror the JSON shape in your error middleware
```

### Requirements / Requisitos

- `git`
- Any HTTP API stack

---

## Quick start / Início rápido

```bash
git clone https://github.com/manansbdb/rest-error-format.git
# open error-envelope.json and mirror fields in your API errors
```

---

## Contents / Conteúdos

| Path | Purpose / Função |
|------|------------------|
| `error-envelope.json` | Canonical error shape |
| `examples.md` | Sample payloads |
| `SUPPORT.md` | Donations / Doações |

---

## Project layout / Estrutura

```text
rest-error-format/
├── docs/banner.svg
├── error-envelope.json
├── examples.md
├── SUPPORT.md
└── README.md
```

---

## Support / Apoio

Bitcoin donations welcome / Doações em Bitcoin bem-vindas:

```
bc1q0qfnlnxyum9u45stzxe0a7jnhtj4j0usfkqdjw
```

See [SUPPORT.md](./SUPPORT.md).

---

## License / Licença

[MIT](./LICENSE) © 2026 manansbdb
