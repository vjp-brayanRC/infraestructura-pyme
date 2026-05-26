# Diseño de infraestructura

## Arquitectura general

Cliente → HAProxy → Apache/PHP → MySQL

## Tabla de software

| Software | Versión | Función |
|---|---|---|
| Ubuntu Server | 22.04 | Sistema operativo | Certbot para SSL |
| Apache     | 2.4.60 | Servidor web (versión actualizada) |
| MySQL      | 8.0    | Base de datos                      |
| Certbot    | 2.9    | SSL/TLS automático (añadido)
| PHP | 8.2 | Backend |
| Netdata | Latest | Monitorización |

## Puertos utilizados

| Puerto | Servicio |
|---|---|
| 22 | SSH |
| 80 | HTTP |
| 443 | HTTPS |
| 3306 | MySQL |