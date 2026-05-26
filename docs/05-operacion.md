# Guía de Operación y Mantenimiento Diario

## Objetivo

Este documento describe las tareas básicas de operación y mantenimiento diario de la infraestructura de la PYME basada en entorno LAMP. Su finalidad es garantizar la estabilidad, disponibilidad y correcto funcionamiento de los servicios desplegados.

---

# 1. Comprobación del estado del servidor

Cada día se debe verificar que todos los servicios principales estén funcionando correctamente.

## Servicios a comprobar

- Apache2
- MySQL/MariaDB
- SSH
- Firewall (UFW)

## Comandos de comprobación

### Estado de Apache

```bash
sudo systemctl status apache2