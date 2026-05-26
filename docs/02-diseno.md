# Diseño de infraestructura

## Arquitectura general

```mermaid
graph LR
    A[Cliente] --> B[HAProxy]
    B --> C[Apache / PHP]
    C --> D[MySQL]
Cliente → HAProxy → Apache/PHP → MySQL

## Tabla de software

| Software | Versión | Función |
|---|---|---|
| Ubuntu Server | 22.04 | Sistema operativo |
| Apache | 2.4.60 | Servidor web |
| PHP | 8.2 | Backend |
| MySQL | 8.0 | Base de datos |

## Puertos utilizados

| Puerto | Servicio |
|---|---|
| 22 | SSH |
| 80 | HTTP |
| 443 | HTTPS |
| 3306 | MySQL |
