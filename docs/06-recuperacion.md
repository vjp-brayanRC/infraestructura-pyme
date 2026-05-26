# 06-recuperacion.md

# Plan de Recuperación ante Desastres (DRP)

## 1. Objetivo

Este documento establece el Plan de Recuperación ante Desastres (Disaster Recovery Plan) de la infraestructura LAMP de la PYME, con el fin de restaurar los servicios críticos en el menor tiempo posible tras una incidencia grave.

---

## 2. Alcance

Este plan aplica a:

- Servidor web (Apache)
- Base de datos (MySQL/MariaDB)
- Aplicaciones desplegadas en el sistema
- Sistema operativo Linux
- Copias de seguridad y almacenamiento
- Acceso remoto (SSH)

---

## 3. Tipos de desastres contemplados

### 3.1 Fallo de hardware
- Caída del disco duro
- Fallo de RAM o CPU
- Avería del servidor físico o máquina virtual

### 3.2 Fallo de software
- Corrupción del sistema operativo
- Fallo de Apache o MySQL
- Actualizaciones defectuosas

### 3.3 Pérdida de datos
- Eliminación accidental de bases de datos
- Corrupción de archivos
- Ransomware o ataques externos

### 3.4 Ciberataques
- Accesos no autorizados
- Ataques de denegación de servicio (DDoS)
- Robo de credenciales

---

## 4. Estrategia de recuperación

### 4.1 Prioridades de restauración

1. Base de datos (MySQL/MariaDB)
2. Servidor web (Apache)
3. Aplicación web
4. Acceso SSH y administración
5. Servicios secundarios

---

## 5. Copias de seguridad

### 5.1 Tipos de backup

- Copia diaria de base de datos
- Copia semanal completa del sistema
- Copia incremental de archivos críticos

### 5.2 Ubicación de backups

- /backups/local/
- Servidor remoto o almacenamiento externo

### 5.3 Verificación

Se debe comprobar diariamente:

```bash
ls -lh /backups