# Misión Olimpia

### Plataforma interactiva para el entrenamiento del razonamiento matemático

**Caso de estudio de desarrollo de software educativo · Portafolio técnico**

> **Estado:** prototipo funcional de uso local. Este repositorio es una presentación del proyecto y **no contiene código fuente ni datos de estudiantes**.

Misión Olimpia nació para apoyar sesiones de tutoría matemática de nivel primaria mediante actividades interactivas, retos de geometría, simulacros y dinámicas de gamificación. El proyecto prioriza la continuidad de las sesiones, la retroalimentación y el uso sin conexión a internet.

## Vista general

| Característica | Estado |
| --- | --- |
| Actividades interactivas de geometría y razonamiento | Implementadas en el prototipo |
| Simulacro de opción múltiple | Implementado |
| Gamificación: NIMO Stars y NIMO Brick Rush | Implementada |
| Guardado local y recuperación de sesiones | Implementados |
| Importación y exportación de datos | Implementadas |
| Ejecución local sin conexión (`file://`) | Verificada durante el desarrollo |
| Pruebas automatizadas | 80 pruebas aprobadas en el último cierre reportado |
| Plataforma multiusuario en línea | Propuesta; no implementada |

## Galería

Las capturas reales y anonimizadas se incorporarán progresivamente. No se utilizan imágenes simuladas para representar funcionalidades implementadas.

| Pantalla | Qué demuestra |
| --- | --- |
| Inicio | Navegación por actividades y sesiones |
| Desafíos de geometría | Construcción y validación de figuras |
| Simulacro | Resolución de reactivos y flujo de entrega |
| NIMO Brick Rush | Gamificación del entrenamiento |
| Panel del instructor | Seguimiento de actividades y resultados de demostración |
| Vista móvil | Adaptación de la interfaz a pantallas pequeñas |

## Tecnologías utilizadas actualmente

- **Frontend:** HTML5, CSS3 y JavaScript.
- **Persistencia:** almacenamiento local del navegador, con mecanismos de recuperación y transferencia de datos.
- **Ejecución:** aplicación web local, sin servidor obligatorio y sin dependencia de internet para las actividades incluidas.
- **Calidad:** pruebas automatizadas de JavaScript ejecutadas con Node.js.
- **Control de versiones:** Git, con desarrollo incremental documentado.

## Arquitectura propuesta para una futura versión pública

Las siguientes tecnologías son **opciones de diseño bajo evaluación**, no componentes ya implementados:

- **React + TypeScript** para una interfaz modular y mantenible.
- **Node.js + NestJS** para una API y servicios de aplicación, si el modelo multiusuario lo requiere.
- **PostgreSQL** para persistencia centralizada.
- **PWA y estrategias offline-first** para conservar parte de la experiencia sin conexión.
- **Autenticación y roles** para instructores y estudiantes, con especial atención a la privacidad de menores.
- **Analítica pedagógica e IA asistida**, sujetas a validación educativa y salvaguardas de datos.

La selección definitiva dependerá de pruebas de uso, alcance del MVP, costos de operación y requisitos de privacidad.

## Decisiones de ingeniería

1. **Offline-first:** facilitar actividades sin depender de una conexión estable.
2. **Persistencia recuperable:** reducir el riesgo de perder avances ante cierres o recargas.
3. **Separación entre evaluación y gamificación:** mantener claros los objetivos pedagógicos.
4. **Pruebas automatizadas:** verificar reglas, almacenamiento y comportamientos críticos.
5. **Privacidad desde el diseño:** excluir datos reales de estudiantes del material de demostración.

## Evolución del producto

| Fase | Objetivo | Estado |
| --- | --- | --- |
| 1. Prototipo local | Actividades, simulacro, juegos, persistencia y pruebas | Funcional |
| 2. MVP público | Validar usuarios, experiencia, accesibilidad y arquitectura | Planeado |
| 3. Gestión educativa | Grupos, contenidos, seguimiento y reportes | Propuesto |
| 4. Asistencia inteligente | Recomendaciones y adaptación de ejercicios con supervisión | Exploratorio |

Consulta [la hoja de ruta](docs/roadmap.md) y [la arquitectura](docs/arquitectura.md) para conocer las decisiones pendientes.

## Privacidad y disponibilidad

Este repositorio contiene exclusivamente documentación del producto. El código de la aplicación, las preguntas utilizadas en tutorías, las evaluaciones individuales y los archivos de referencia se mantienen fuera de esta publicación. Las futuras capturas deberán usar datos ficticios y revisarse antes de incorporarse.

**El código fuente no está disponible públicamente en esta etapa.** Esta publicación no concede licencia sobre el software original ni sobre contenidos de terceros.

---

*Proyecto presentado como evidencia de desarrollo de producto, experiencia de usuario, pruebas y diseño de software educativo.*
