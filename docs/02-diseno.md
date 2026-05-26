# Diseño de infraestructura

## Arquitectura general

```mermaid
graph LR
    A[Cliente] --> B[HAProxy]
    B --> C[Apache / PHP]
    C --> D[MySQL]