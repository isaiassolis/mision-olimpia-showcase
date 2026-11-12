# Arquitectura: estado actual y alternativas futuras

## Estado actual — verificado a partir del cierre de desarrollo

- Interfaz construida con HTML, CSS y JavaScript.
- Ejecución local sin servidor obligatorio (`file://`).
- Persistencia en almacenamiento del navegador, con recuperación e importación/exportación de datos.
- Módulos de actividades, simulacro y gamificación.
- Pruebas automatizadas ejecutadas mediante Node.js.

La arquitectura local fue elegida para permitir uso individual sin infraestructura de despliegue.

## Arquitectura futura — propuesta, no implementada

**Cliente:** React + TypeScript, con diseño responsive y evaluación de capacidades PWA.

**Servidor (condicional):** API con Node.js y NestJS para usuarios, contenidos, progreso y permisos, si las pruebas de producto justifican una solución centralizada.

**Datos:** PostgreSQL como opción de almacenamiento centralizado, complementado con una estrategia explícita de uso offline y sincronización.

**Privacidad:** minimización de datos, control de acceso, políticas de conservación y consentimiento aplicable cuando participen menores.

**Calidad:** ampliar las pruebas unitarias actuales con integración, accesibilidad y pruebas de extremo a extremo.

## Decisiones abiertas

1. ¿El primer lanzamiento será individual, para instructores o para escuelas?
2. ¿Qué datos deben sincronizarse y cuáles deben permanecer en el dispositivo?
3. ¿Qué funciones requieren cuentas de usuario?
4. ¿Cuál será el costo operativo aceptable para el MVP?
5. ¿Cómo validar pedagógicamente recomendaciones automáticas antes de incorporar IA?

Ninguna tecnología futura se presenta como ya desplegada.
