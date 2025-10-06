# Public Docs

Repositorio de documentación pública con propuestas técnicas y análisis de proyectos.

## 📄 Documentos Disponibles

### [Propuesta de Escalabilidad - App Valparaíso](PROPUESTA_ESCALABILIDAD_APP_VALPO.md)
Análisis técnico y propuesta de mejora para el Sistema de Monitoreo Regional SENAPRED Valparaíso. Incluye:
- Evaluación de la arquitectura actual
- Identificación de problemas críticos de escalabilidad
- Propuesta de solución con plan de implementación por fases
- Stack tecnológico recomendado y estimación de costos

---

## 📚 Plantillas y Ejemplos

La carpeta [`EJEMPLOS/`](EJEMPLOS/) contiene archivos base y plantillas para estandarizar la documentación de futuros proyectos. Estos son **recursos de referencia** que deben adaptarse según las necesidades específicas de cada proyecto.

### [Plantilla de README](EJEMPLOS/PROPUESTA_README.md)
Template completo y detallado para documentar proyectos. Incluye estructura profesional con:
- Características y demo del proyecto
- Guías de instalación y configuración
- Documentación de uso y API
- Testing y estructura del proyecto
- Deployment y tecnologías utilizadas
- Contribución, roadmap y contacto

### [Guía de Contribución](EJEMPLOS/CONTRIBUTING.md)
Documento general que establece estándares y procesos para contribuir a proyectos. Este archivo **es bastante estándar** y requiere mínimas modificaciones entre proyectos. Incluye:
- Código de conducta y comportamientos esperados
- Proceso completo de contribución (fork, branch, commit, PR)
- Estándares de código y buenas prácticas
- Convenciones de commits (Conventional Commits)
- Convenciones de branches y flujo de trabajo
- Proceso de code review y criterios de aprobación
- Guías para reportar bugs y sugerir mejoras
- FAQ y recursos adicionales

**Personalización mínima requerida:**
- Actualizar enlaces de contacto y comunicación
- Ajustar herramientas de linting específicas del proyecto
- Modificar requisitos de coverage de tests si es necesario
- Adaptar ejemplos de comandos según el stack tecnológico

### Carpeta [`.github/`](EJEMPLOS/.github/)
Estructura completa de configuración para GitHub que incluye workflows de CI/CD y templates para colaboración. **Esta estructura se copia directamente a la raíz del proyecto.**

#### [Workflows CI/CD](EJEMPLOS/.github/workflows/)
Pipelines automatizados para integración y despliegue continuo:

- **[`ci.yml`](EJEMPLOS/.github/workflows/ci.yml)** - Integración Continua
  - Lint y validación de código
  - Tests unitarios, integración y E2E
  - Análisis de seguridad (npm audit, Snyk, CodeQL)
  - Build y verificación de artefactos
  - Coverage y análisis con SonarCloud
  - Ejecuta en push y PR a `develop` y `main`

- **[`cd.yml`](EJEMPLOS/.github/workflows/cd.yml)** - Despliegue Continuo
  - Build y push de imágenes Docker
  - Deploy automático a Staging (desde `develop`)
  - Deploy automático a Producción (desde `main`)
  - Smoke tests post-deployment
  - Rollback automático si fallan las pruebas
  - Notificaciones a Slack y email
  - Monitoreo post-deployment

**Personalización requerida:**
- Configurar secrets en GitHub (Docker, Kubernetes, APIs)
- Ajustar nombres de servicios y deployments
- Adaptar según infraestructura (AWS, Azure, GCP, Heroku, etc.)
- Modificar comandos de tests según el proyecto

#### [Issue Templates](EJEMPLOS/.github/ISSUE_TEMPLATE/)

- **[`PROPUESTA_ISSUES.md`](EJEMPLOS/.github/ISSUE_TEMPLATE/PROPUESTA_ISSUES.md)** - Guía completa con templates para:
  - Bug reports con información estructurada
  - Feature requests con criterios de aceptación
  - Templates para mejoras, documentación y refactoring
  - Reportes de performance y vulnerabilidades de seguridad
  - Guías de buenas prácticas y sistema de labels
  - Configuración de templates automáticos en GitHub

#### [Pull Request Template](EJEMPLOS/.github/PULL_REQUEST_TEMPLATE.md)
Template estandarizado para PRs con:
- Descripción detallada de cambios
- Checklist completo de validación
- Sección de testing (automatizado y manual)
- Screenshots/videos para cambios visuales
- Notas para reviewers
- Plan de deployment
- Evaluación de riesgos

---

## 💡 Cómo Usar las Plantillas

1. **No copies todo**: Selecciona solo las secciones relevantes para tu proyecto
2. **Adapta el contenido**: Personaliza ejemplos, comandos y tecnologías según tu stack
3. **Mantén la estructura**: Respeta la organización general para mantener consistencia
4. **Actualiza regularmente**: La documentación debe evolucionar con el proyecto