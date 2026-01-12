# Arquitectura Git del Proyecto

## 1. Estructura del Repositorio

El repositorio sigue una estructura modular y escalable, separando claramente el código fuente, pruebas y documentación:

```text
scv-empresarial/
├── src/
│   ├── components/   # Componentes principales del sistema
│   ├── utils/        # Funciones utilitarias reutilizables
│   └── services/     # Lógica de negocio y servicios
│
├── tests/
│   ├── unit/         # Pruebas unitarias
│   └── integration/  # Pruebas de integración
│
├── docs/
│   ├── architecture/ # Documentación de arquitectura
│   └── guides/       # Guías de uso y contribución
│
├── README.md         # Información general del proyecto
├── .gitignore        # Archivos y carpetas ignoradas por Git
└── CONTRIBUTING.md   # Guía de contribuciones
Esta estructura permite un desarrollo ordenado, mantenimiento sencillo y escalabilidad del proyecto.

2. Estrategia de Branching

Se utiliza una estrategia de branching simple y clara basada en buenas prácticas:

main

Rama principal y estable

Contiene únicamente código listo para revisión y entrega

Todos los commits deben estar firmados

feature/

Ramas para el desarrollo de nuevas funcionalidades

Ejemplo: feature/git-architecture-doc

fix/

Ramas para corrección de errores

Ejemplo: fix/readme-typo

Flujo recomendado:

Crear rama desde main

Desarrollar cambios

Realizar commits pequeños y descriptivos

Integrar a main mediante merge

3. Políticas de Commits

El proyecto adopta convenciones de commits para mantener un historial claro y profesional.

3.1 Formato del mensaje
<tipo>: <descripción breve>
3.2 Tipos permitidos

docs: cambios en documentación

feat: nuevas funcionalidades

fix: corrección de errores

chore: tareas de mantenimiento

test: pruebas

refactor: mejoras de código sin cambiar funcionalidad

Ejemplo:
git commit -S -m "docs: add git architecture documentation"
4. Commits Firmados

Todos los commits deben realizarse con firma GPG:
git commit -S -m "mensaje del commit"
Esto garantiza:

Autenticidad del autor

Integridad del historial

Cumplimiento de estándares profesionales

5. Buenas Prácticas

Commits pequeños y frecuentes

Mensajes claros y descriptivos

No subir archivos generados o temporales

Mantener la rama main siempre estable
