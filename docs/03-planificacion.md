# Planificación del proyecto

## Diagrama de Gantt

```mermaid
gantt
    title Planificación de infraestructura
    dateFormat  YYYY-MM-DD
    axisFormat  %d/%m

    section Análisis
    Estudio de requisitos        :done, a1, 2026-05-01, 3d
    Diseño de arquitectura       :done, a2, after a1, 4d

    section Implementación
    Configuración servidor web   :active, b1, 2026-05-10, 5d
    Configuración base de datos  :b2, after b1, 4d
    Configuración HAProxy        :b3, after b2, 3d

    section Monitorización
    Instalación Netdata          :c1, after b3, 2d
    Pruebas de carga             :c2, after c1, 3d

    section Despliegue
    Pruebas finales              :d1, after c2, 2d
    Puesta en producción         :d2, after d1, 1d