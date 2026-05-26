# 05-operacion.md

# Guía de Operación y Mantenimiento Diario

## 1. Objetivo

Este documento describe las tareas diarias necesarias para asegurar el correcto funcionamiento de la infraestructura LAMP de la PYME, garantizando la disponibilidad de los servicios y la detección temprana de incidencias.

---

## 2. Servicios críticos a revisar

Cada día se debe comprobar el estado de los siguientes servicios:

- Apache (servidor web)
- MySQL/MariaDB (base de datos)
- SSH (acceso remoto)
- Firewall UFW (seguridad del sistema)

---

## 3. Comprobación del estado del sistema

### Estado de Apache

```bash
sudo systemctl status apache2