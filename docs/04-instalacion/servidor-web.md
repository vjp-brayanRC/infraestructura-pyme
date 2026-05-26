# servidor-web.md

# Configuración del Servidor Web (Apache + PHP)

## 1. Objetivo

Este documento describe la instalación y configuración del servidor web Apache con soporte PHP dentro de una infraestructura LAMP para una PYME. Su finalidad es servir aplicaciones web de forma segura, estable y eficiente.

---

## 2. Software utilizado

- Sistema operativo: Ubuntu Server 22.04
- Servidor web: Apache2
- Lenguaje backend: PHP
- Módulo de base de datos: MySQL/MariaDB

---

## 3. Instalación de Apache

### Actualizar repositorios

```bash id="a1p1u1"
sudo apt update
