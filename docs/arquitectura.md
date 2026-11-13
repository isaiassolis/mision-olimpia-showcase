# Misión Olimpia — Arquitectura del prototipo

## Una aplicación educativa que funciona sin conexión

Diseñé Misión Olimpia para utilizarse durante sesiones individuales de aprendizaje, sin requerir acceso a internet ni infraestructura de servidor.

El prototipo funciona directamente desde el navegador mediante archivos locales (`file://`) y está construido con **HTML, CSS y JavaScript**.

## Componentes principales

| Componente | Función |
| --- | --- |
| **Interfaz y retos** | Actividades de geometría, razonamiento y comprobación de soluciones. |
| **Simulacro** | Evaluación de opción múltiple y control del tiempo. |
| **Gamificación** | NIMO Stars y NIMO Brick Rush como experiencias complementarias. |
| **Persistencia** | Guardado local y recuperación de sesiones. |
| **Transferencia de información** | Importación y exportación JSON. |
| **Pruebas** | Validación automatizada mediante Node.js. |

## Decisiones técnicas

- **Offline-first:** permitir el uso sin servidor ni red.
- **Guardado recuperable:** evitar que un cierre inesperado haga perder el avance.
- **Separación de actividades:** mantener el simulacro independiente de los minijuegos.
- **Interacción comprobable:** validar las condiciones de los retos matemáticos.
- **Privacidad:** conservar la información local y no incluir datos reales de estudiantes en las capturas públicas.

## Validación

El último cierre de desarrollo documentó **80 pruebas automatizadas aprobadas**. También se revisó el funcionamiento desde archivos locales y la presentación de la interfaz en escritorio y móvil.

## Una posible arquitectura futura

Si el producto evoluciona hacia una plataforma para instructores o escuelas, evaluaré una interfaz con **React y TypeScript**, un servicio con **Node.js y NestJS** y persistencia centralizada con **PostgreSQL**.

También sería necesario definir sincronización offline, roles, accesibilidad, protección de datos de menores y criterios pedagógicos para cualquier función asistida por IA.

Estas son **opciones de evolución**, no tecnologías utilizadas en la versión local actual.

[← Volver al proyecto](../README.md)
