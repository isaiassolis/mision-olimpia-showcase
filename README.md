<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0B1220,50:12395D,100:087F8C&height=205&section=header&text=Misi%C3%B3n%20Olimpia&fontSize=42&fontColor=ffffff&desc=Educational%20Software%20%7C%20Offline-First%20%7C%20Gamification&descAlignY=66&descSize=15&animation=fadeIn" width="100%" alt="Misión Olimpia — aprendizaje matemático, software offline y gamificación" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Frontend-HTML%20%7C%20CSS%20%7C%20JavaScript-087F8C?style=for-the-badge" alt="HTML, CSS y JavaScript" />
  <img src="https://img.shields.io/badge/Architecture-Offline--First-12395D?style=for-the-badge" alt="Arquitectura offline-first" />
  <img src="https://img.shields.io/badge/Tests-80%20Passed-0B91A1?style=for-the-badge" alt="80 pruebas aprobadas en el último cierre" />
  <img src="https://img.shields.io/badge/Status-Functional%20Prototype-12395D?style=for-the-badge" alt="Prototipo funcional" />
</p>

# Misión Olimpia — Matemáticas, aprendizaje interactivo y gamificación

**Producto educativo propio · Desarrollo web offline · Experiencias de aprendizaje y evaluación**

Desarrollé **Misión Olimpia** para apoyar sesiones individuales de preparación matemática en educación primaria. Quería convertir una serie de ejercicios en una experiencia donde fuera posible **explorar soluciones, comprobar razonamientos y practicar bajo condiciones parecidas a las de una evaluación**, sin perder el carácter didáctico de la tutoría.

El resultado es un **prototipo funcional que trabaja sin conexión a internet**, con actividades de geometría y razonamiento, simulacros, recuperación de sesiones y dos experiencias de gamificación protagonizadas por **NIMO**.

![Pantalla de bienvenida de Misión Olimpia](screenshots/01-bienvenida.png)

## El desafío educativo

Preparar a un estudiante para resolver problemas matemáticos requiere algo más que mostrar preguntas y calificar respuestas. Es importante que pueda probar estrategias, detectar errores, volver a intentarlo y conservar un registro útil para revisar su proceso.

Diseñé Misión Olimpia como una **herramienta de apoyo para el instructor**, no como un sustituto de la enseñanza presencial ni del trabajo con papel y lápiz.

## Qué desarrollé

| Componente | Funcionalidad |
| --- | --- |
| **Retos interactivos** | Actividades de razonamiento y construcción de figuras geométricas. |
| **Comprobación de soluciones** | Reglas para revisar restricciones y distintas respuestas válidas. |
| **Simulacro** | Ejercicios de opción múltiple y seguimiento del tiempo de evaluación. |
| **Persistencia local** | Guardado automático y recuperación de sesiones. |
| **Intercambio de datos** | Importación y exportación de información en archivos JSON. |
| **NIMO Stars** | Actividad lúdica de pausa y exploración. |
| **NIMO Brick Rush** | Minijuego de práctica complementaria, separado de la calificación del simulacro. |
| **Ejecución offline** | Funcionamiento desde archivos locales, sin servidor ni conexión obligatoria. |

## Misión Olimpia en imágenes

### Inicio y selección de actividades

![Pantalla de bienvenida con los retos de Misión Olimpia](screenshots/01-bienvenida.png)

*La bienvenida organiza la experiencia y presenta las actividades matemáticas.*

### Construcción de figuras

![Construcción interactiva de figuras de seis cuadrados](screenshots/02-construccion-seis-cuadrados.png)

*Diseñé retos de geometría en los que el estudiante construye figuras, comprueba condiciones y explora soluciones mediante desplazamientos, giros y reflexiones.*

### NIMO Stars

![Minijuego NIMO Stars](screenshots/03-nimo-estrellas.png)

*Una experiencia recreativa entre actividades, sin penalizaciones ni puntuaciones competitivas.*

### NIMO Brick Rush

![Minijuego NIMO Brick Rush](screenshots/04-nimo-brick-rush.png)

*Actividad gamificada independiente de la calificación del simulacro, con controles de pausa, reanudación y reinicio.*

## Decisiones de diseño y aprendizaje

Desde el principio busqué que la aplicación pudiera utilizarse durante una sesión real, incluso sin acceso a internet.

Por eso prioricé:

- **Interacción antes que memorización:** los retos de geometría permiten comprobar ideas y construir soluciones.
- **Continuidad de la sesión:** el trabajo se guarda localmente y puede recuperarse después de una interrupción.
- **Evaluación y juego por separado:** las actividades recreativas complementan la práctica, sin alterar el resultado del simulacro.
- **Uso sencillo:** una interfaz adaptada a sesiones individuales y revisión por el instructor.
- **Control local de la información:** las actividades no necesitan cuentas de usuario ni enviar datos a un servidor.

## Tecnologías y arquitectura

Construí la versión actual con **HTML5, CSS3 y JavaScript**, manteniendo una aplicación ejecutable directamente desde el navegador.

| Área | Implementación |
| --- | --- |
| **Interfaz** | HTML, CSS y JavaScript |
| **Ejecución** | Navegador local, compatible con `file://` |
| **Persistencia** | Almacenamiento local del navegador |
| **Respaldo e intercambio** | Exportación e importación JSON |
| **Pruebas** | Validaciones automatizadas con Node.js |
| **Versionado** | Git y desarrollo incremental |

La arquitectura evita depender de un servidor para realizar las actividades disponibles en el prototipo.

[Conocer la arquitectura](docs/arquitectura.md).

## Validación del prototipo

Durante el desarrollo probé el funcionamiento de los retos, sus reglas de comprobación, la persistencia, la recuperación de sesiones y los minijuegos.

El último cierre de desarrollo registró **80 pruebas automatizadas aprobadas**, junto con revisiones en navegador de escritorio y móvil y verificación de funcionamiento sin conexión.

Estos resultados corresponden al cierre documentado de esa etapa del prototipo.

## Mi participación

Concebí y desarrollé Misión Olimpia como una solución que combina **programación, diseño de interacción y preparación de actividades educativas**.

Trabajé en la estructura del producto, las reglas de los ejercicios, los mecanismos de guardado, los simulacros, la gamificación y las pruebas. La experiencia en tutorías me permitió orientar las decisiones del software a necesidades concretas de aprendizaje.

## Evolución del producto

Mi prioridad es consolidar la experiencia individual antes de decidir si conviene convertirla en una plataforma pública.

Entre las posibilidades que estudiaré están la creación de contenidos para instructores, el seguimiento de grupos, las mejoras de accesibilidad y la adaptación de actividades con apoyo de inteligencia artificial.

Una versión multiusuario requeriría estudiar una arquitectura diferente, así como medidas específicas de privacidad cuando participen menores.

[Consultar la hoja de ruta](docs/roadmap.md).

## Sobre el repositorio

Aquí comparto las características, la arquitectura y capturas del prototipo. El código de desarrollo y la información de las sesiones individuales permanecen privados.

[Política de publicación y privacidad](docs/privacidad.md).

---

<p align="center"><strong>Aprendizaje matemático, desarrollo de software y diseño de experiencias interactivas.</strong></p>
<p align="center"><a href="https://github.com/isaiassolis">Isaías Solís · Portafolio profesional</a></p>
