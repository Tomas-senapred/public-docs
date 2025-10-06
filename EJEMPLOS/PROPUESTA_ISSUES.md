# Plantillas de Issues para GitHub

Esta guía proporciona plantillas estandarizadas para crear issues de calidad en GitHub. Utiliza estas plantillas como base y adáptalas según las necesidades de tu proyecto.

---

## 📋 Tabla de Contenidos

- [Bug Report](#-bug-report)
- [Feature Request](#-feature-request)
- [Improvement](#-improvement)
- [Documentation](#-documentation)
- [Question](#-question)
- [Performance Issue](#-performance-issue)
- [Security Vulnerability](#-security-vulnerability)
- [Refactoring](#-refactoring)

---

## 🐛 Bug Report

**Template para reportar bugs o errores en el sistema**

```markdown
## 🐛 Descripción del Bug

Descripción clara y concisa del problema encontrado.

## 📝 Pasos para Reproducir

1. Ve a '...'
2. Haz clic en '...'
3. Desplázate hasta '...'
4. Observa el error

## 🎯 Comportamiento Esperado

Descripción clara de lo que debería suceder.

## 🔴 Comportamiento Actual

Descripción de lo que realmente sucede.

## 📸 Screenshots

Si aplica, agrega capturas de pantalla para ayudar a explicar el problema.

## 🖥️ Ambiente

- **OS:** [e.g. Windows 11, macOS 14, Ubuntu 22.04]
- **Navegador:** [e.g. Chrome 120, Firefox 121, Safari 17]
- **Versión de la App:** [e.g. 1.2.3]
- **Node Version:** [e.g. 18.17.0]
- **Otros:** [cualquier información relevante]

## 📋 Logs / Mensajes de Error

```
Pega aquí los logs o mensajes de error relevantes
```

## 🔍 Contexto Adicional

Agrega cualquier otro contexto sobre el problema aquí.

## ⚡ Severidad

- [ ] Crítico - El sistema no funciona / pérdida de datos
- [ ] Alto - Funcionalidad principal afectada
- [ ] Medio - Funcionalidad secundaria afectada  
- [ ] Bajo - Problema cosmético o menor

## 👥 Usuarios Afectados

- [ ] Todos los usuarios
- [ ] Solo ciertos roles: [especificar]
- [ ] Solo en ciertos ambientes: [especificar]
- [ ] Casos específicos: [especificar]

## 💡 Posible Solución (Opcional)

Si tienes ideas de cómo podría solucionarse, compártelas aquí.
```

**Ejemplo Real:**

```markdown
## 🐛 Descripción del Bug

El botón "Guardar" en el formulario de creación de usuario no responde cuando se hace clic después de completar todos los campos requeridos.

## 📝 Pasos para Reproducir

1. Navega a `/admin/users/new`
2. Completa todos los campos del formulario (nombre, email, rol)
3. Haz clic en el botón "Guardar"
4. El botón no responde, no hay feedback visual ni se guarda el usuario

## 🎯 Comportamiento Esperado

Al hacer clic en "Guardar", debería:
- Mostrar un spinner o indicador de carga
- Guardar el usuario en la base de datos
- Redirigir a la lista de usuarios o mostrar mensaje de éxito

## 🔴 Comportamiento Actual

El botón no responde al click, no hay feedback visual y el usuario no se guarda.

## 📸 Screenshots

[Captura del formulario con el botón que no responde]

## 🖥️ Ambiente

- **OS:** Windows 11
- **Navegador:** Chrome 120.0.6099.129
- **Versión de la App:** 1.2.3
- **Node Version:** 18.17.0

## 📋 Logs / Mensajes de Error

```
Console Error:
Uncaught TypeError: Cannot read properties of null (reading 'addEventListener')
    at UserForm.js:45
```

## ⚡ Severidad

- [x] Alto - Funcionalidad principal afectada
- No se pueden crear usuarios nuevos

## 👥 Usuarios Afectados

- [x] Solo ciertos roles: Administradores
```

---

## ✨ Feature Request

**Template para solicitar nuevas funcionalidades**

```markdown
## ✨ Descripción de la Funcionalidad

Descripción clara y concisa de la funcionalidad que te gustaría ver implementada.

## 🎯 Problema que Resuelve

¿Qué problema o necesidad resuelve esta funcionalidad?

**Ejemplo de uso:**
Como [tipo de usuario], quiero [objetivo] para poder [beneficio].

## 💡 Solución Propuesta

Descripción clara de cómo te gustaría que funcionara la solución.

## 🔄 Alternativas Consideradas

¿Has considerado otras alternativas? Descríbelas aquí.

## 📊 Beneficios

- Beneficio 1: [descripción]
- Beneficio 2: [descripción]
- Beneficio 3: [descripción]

## 👥 Usuarios Beneficiados

¿Qué tipos de usuarios se beneficiarían de esta funcionalidad?

- [ ] Todos los usuarios
- [ ] Administradores
- [ ] Usuarios finales
- [ ] Desarrolladores
- [ ] Otro: [especificar]

## 🎨 Mockups / Wireframes (Opcional)

Si tienes ideas visuales, adjúntalas aquí.

## 🔗 Referencias

Enlaces a recursos, ejemplos en otros sistemas, documentación relevante, etc.

## ⚖️ Prioridad Sugerida

- [ ] Alta - Crítico para el negocio
- [ ] Media - Importante pero no urgente
- [ ] Baja - Nice to have

## 📋 Criterios de Aceptación

- [ ] Criterio 1
- [ ] Criterio 2
- [ ] Criterio 3

## 🔍 Contexto Adicional

Cualquier otra información relevante sobre la feature request.
```

**Ejemplo Real:**

```markdown
## ✨ Descripción de la Funcionalidad

Implementar exportación de reportes de incidentes a formato PDF y Excel.

## 🎯 Problema que Resuelve

Actualmente los usuarios solo pueden ver los reportes en pantalla, pero necesitan compartirlos en reuniones y enviarlos por email en formatos estándar.

**Ejemplo de uso:**
Como supervisor de operaciones, quiero exportar reportes de incidentes en PDF y Excel para poder compartirlos con otros departamentos y en reuniones ejecutivas.

## 💡 Solución Propuesta

1. Agregar botones "Exportar a PDF" y "Exportar a Excel" en la vista de reportes
2. El PDF debe incluir:
   - Logo de la organización
   - Título del reporte
   - Fecha de generación
   - Tabla con datos de incidentes
   - Gráficos relevantes
3. El Excel debe incluir:
   - Hoja con datos tabulados
   - Filtros automáticos en las columnas
   - Formato condicional para estados

## 📊 Beneficios

- Facilita la comunicación con stakeholders externos
- Mejora la documentación de incidentes
- Reduce tiempo de preparación de reportes manuales
- Permite análisis offline con herramientas estándar

## 👥 Usuarios Beneficiados

- [x] Administradores
- [x] Supervisores
- [x] Usuarios finales con permisos de reporte

## ⚖️ Prioridad Sugerida

- [x] Media - Importante pero no urgente

## 📋 Criterios de Aceptación

- [ ] Botones de exportación visibles en vista de reportes
- [ ] PDF generado incluye todos los datos del reporte
- [ ] Excel generado es compatible con Microsoft Excel y LibreOffice
- [ ] Exportación funciona con reportes de hasta 10,000 registros
- [ ] Proceso de exportación muestra indicador de progreso
```

---

## 🔧 Improvement

**Template para mejoras a funcionalidades existentes**

```markdown
## 🔧 Área a Mejorar

¿Qué componente, página o funcionalidad específica necesita mejora?

## 📝 Situación Actual

Descripción del estado actual de la funcionalidad.

## 🎯 Mejora Propuesta

Descripción clara de la mejora que propones.

## 📈 Beneficios Esperados

- Mejora en performance: [detalles]
- Mejora en UX: [detalles]
- Mejora en mantenibilidad: [detalles]
- Otros: [detalles]

## 🔢 Métricas de Éxito

¿Cómo medirás que la mejora fue exitosa?

- Métrica 1: [descripción]
- Métrica 2: [descripción]

## 💻 Implementación Sugerida (Opcional)

Si tienes ideas técnicas de implementación, compártelas.

## 🎯 Prioridad

- [ ] Alta
- [ ] Media
- [ ] Baja

## 🔗 Issues Relacionados

#[número] - [descripción breve]
```

---

## 📚 Documentation

**Template para solicitar o mejorar documentación**

```markdown
## 📚 Tipo de Documentación

- [ ] Documentación de API
- [ ] Guía de usuario
- [ ] Documentación técnica
- [ ] Tutorial
- [ ] README
- [ ] Comentarios en código
- [ ] Otro: [especificar]

## 📝 Descripción

¿Qué documentación falta o necesita mejorarse?

## 🎯 Objetivo

¿Qué debería lograr esta documentación?

## 👥 Audiencia

¿Para quién es esta documentación?

- [ ] Usuarios finales
- [ ] Desarrolladores
- [ ] Administradores
- [ ] Nuevos contribuidores
- [ ] Otro: [especificar]

## 📋 Contenido Sugerido

Outline o estructura sugerida para la documentación:

1. Sección 1
2. Sección 2
3. Sección 3

## 🔗 Referencias

Enlaces a documentación existente o recursos útiles.
```

---

## ❓ Question

**Template para preguntas sobre el proyecto**

```markdown
## ❓ Pregunta

Formula tu pregunta de manera clara y específica.

## 🔍 Contexto

Proporciona contexto sobre por qué estás haciendo esta pregunta.

## 🔗 Recursos Consultados

¿Qué documentación o recursos ya consultaste?

- [ ] README.md
- [ ] Wiki del proyecto
- [ ] Issues existentes
- [ ] Documentación de API
- [ ] Otro: [especificar]

## 💡 Lo que ya Intentaste (si aplica)

Si ya intentaste algo para resolver tu duda, descríbelo aquí.
```

---

## ⚡ Performance Issue

**Template para reportar problemas de rendimiento**

```markdown
## ⚡ Descripción del Problema de Performance

Descripción clara del problema de rendimiento observado.

## 📍 Ubicación

¿En qué parte del sistema ocurre?

- **Página/Módulo:** [especificar]
- **Acción específica:** [especificar]

## 📊 Métricas Actuales

- **Tiempo de carga:** [Xs]
- **Tiempo de respuesta:** [Xms]
- **Uso de memoria:** [XMB]
- **Uso de CPU:** [X%]
- **Tamaño de payload:** [XKB]

## 🎯 Métricas Esperadas

- **Tiempo de carga objetivo:** [Xs]
- **Tiempo de respuesta objetivo:** [Xms]

## 🔍 Análisis Realizado

¿Qué análisis o profiling has realizado?

- [ ] Chrome DevTools Performance
- [ ] Network tab
- [ ] Lighthouse
- [ ] Backend profiling
- [ ] Database query analysis
- [ ] Otro: [especificar]

## 📋 Datos de Prueba

Describe el volumen de datos con el que probaste:

- Número de registros: [X]
- Tamaño de dataset: [XMB]
- Usuarios concurrentes: [X]

## 💡 Posible Causa

Si identificaste una posible causa, descríbela aquí.

## 🔧 Solución Propuesta

Si tienes ideas de optimización, compártelas:

- Sugerencia 1
- Sugerencia 2

## 🖥️ Ambiente

- **OS:** [especificar]
- **Hardware:** [CPU, RAM, etc.]
- **Navegador/Cliente:** [especificar]
- **Versión:** [especificar]
```

---

## 🔒 Security Vulnerability

**Template para reportar vulnerabilidades de seguridad**

> ⚠️ **IMPORTANTE:** Si la vulnerabilidad es crítica, considera reportarla de forma privada primero al equipo de seguridad antes de crear un issue público.

```markdown
## 🔒 Tipo de Vulnerabilidad

- [ ] Inyección SQL
- [ ] XSS (Cross-Site Scripting)
- [ ] CSRF (Cross-Site Request Forgery)
- [ ] Autenticación/Autorización
- [ ] Exposición de datos sensibles
- [ ] Configuración insegura
- [ ] Dependencias vulnerables
- [ ] Otro: [especificar]

## 📝 Descripción

Descripción clara de la vulnerabilidad encontrada.

## 🎯 Severidad

- [ ] Crítica - Explotación remota, acceso no autorizado a datos sensibles
- [ ] Alta - Compromiso de cuentas de usuario
- [ ] Media - Exposición limitada de información
- [ ] Baja - Riesgo teórico o requiere condiciones especiales

## 📍 Ubicación

¿Dónde se encuentra la vulnerabilidad?

- **Archivo/Módulo:** [especificar]
- **Línea de código:** [especificar]
- **Endpoint:** [especificar]

## 🔍 Pasos para Reproducir

1. Paso 1
2. Paso 2
3. Paso 3

## 🎯 Impacto

Describe el impacto potencial si la vulnerabilidad es explotada.

## 🔧 Solución Recomendada

Propón una solución para mitigar la vulnerabilidad.

## 🔗 Referencias

- [OWASP - Referencia]
- [CVE - ID si aplica]
- Otros recursos relevantes

## 📋 Checklist de Remediación

- [ ] Código corregido
- [ ] Tests de seguridad agregados
- [ ] Documentación actualizada
- [ ] Deployment en producción
- [ ] Notificación a usuarios afectados (si aplica)
```

---

## 🔨 Refactoring

**Template para proponer refactoring de código**

```markdown
## 🔨 Código/Módulo a Refactorizar

¿Qué componente o módulo necesita refactoring?

## 📝 Situación Actual

Descripción del estado actual del código.

**Problemas identificados:**
- Problema 1: [descripción]
- Problema 2: [descripción]
- Problema 3: [descripción]

## 🎯 Objetivo del Refactoring

¿Qué se busca lograr con este refactoring?

- [ ] Mejorar legibilidad
- [ ] Reducir complejidad ciclomática
- [ ] Eliminar código duplicado
- [ ] Mejorar performance
- [ ] Facilitar testing
- [ ] Actualizar a mejores prácticas
- [ ] Otro: [especificar]

## 💡 Propuesta de Refactoring

Descripción de cómo se propone refactorizar el código.

**Cambios principales:**
1. Cambio 1
2. Cambio 2
3. Cambio 3

## 📊 Beneficios

- Beneficio 1
- Beneficio 2
- Beneficio 3

## ⚠️ Riesgos

¿Qué riesgos existen al hacer este refactoring?

- Riesgo 1: [descripción y mitigación]
- Riesgo 2: [descripción y mitigación]

## 🧪 Plan de Testing

¿Cómo se verificará que el refactoring no rompe funcionalidad?

- [ ] Tests unitarios existentes pasan
- [ ] Nuevos tests agregados
- [ ] Tests de integración
- [ ] Testing manual de [funcionalidad]

## 📋 Checklist

- [ ] Análisis de código actual completado
- [ ] Propuesta de diseño aprobada
- [ ] Tests escritos/actualizados
- [ ] Refactoring implementado
- [ ] Code review completado
- [ ] Documentación actualizada
- [ ] Deploy en staging
- [ ] Deploy en producción
```

---

## 🎯 Buenas Prácticas para Crear Issues

### ✅ DOs (Hacer)

1. **Usa un título descriptivo y conciso**
   - ❌ "Problema con el botón"
   - ✅ "El botón 'Guardar' no responde en el formulario de usuarios"

2. **Proporciona contexto completo**
   - Incluye screenshots, logs, ambiente
   - Pasos claros para reproducir
   - Comportamiento esperado vs actual

3. **Usa labels apropiados**
   - `bug`, `feature`, `enhancement`, `documentation`
   - `priority: high`, `priority: low`
   - `good first issue`, `help wanted`

4. **Vincula issues relacionados**
   - Usa `#numero` para referenciar otros issues
   - Usa `fixes #numero` en PRs para cerrar automáticamente

5. **Mantén el issue actualizado**
   - Comenta con nueva información
   - Actualiza el estado si ya no es relevante
   - Cierra cuando esté resuelto

### ❌ DON'Ts (No Hacer)

1. **No crees issues duplicados**
   - Busca primero en issues existentes
   - Si encuentras uno similar, comenta ahí

2. **No mezcles múltiples problemas en un issue**
   - Un issue = un problema/feature
   - Facilita tracking y resolución

3. **No uses lenguaje ambiguo**
   - Sé específico y técnico cuando sea necesario
   - Proporciona ejemplos concretos

4. **No omitas información de ambiente**
   - Sistema operativo, versión, navegador
   - Configuración relevante

---

## 📝 Configuración de Templates en GitHub

Para usar estos templates automáticamente en tu repositorio:

1. Crea la carpeta `.github/ISSUE_TEMPLATE/` en la raíz de tu proyecto

2. Crea archivos para cada tipo de issue:

```
.github/
└── ISSUE_TEMPLATE/
    ├── bug_report.md
    ├── feature_request.md
    ├── improvement.md
    └── config.yml
```

3. Ejemplo de `bug_report.md`:

```yaml
---
name: Bug Report
about: Reportar un bug o error en el sistema
title: '[BUG] '
labels: bug
assignees: ''
---

[Contenido del template aquí]
```

4. Ejemplo de `config.yml`:

```yaml
blank_issues_enabled: true
contact_links:
  - name: 💬 Discusiones
    url: https://github.com/tu-org/tu-repo/discussions
    about: Para preguntas generales y discusiones
  - name: 📚 Documentación
    url: https://docs.tu-proyecto.com
    about: Consulta la documentación oficial
```

---

## 🏷️ Sistema de Labels Recomendado

### Por Tipo
- `bug` - Error o comportamiento inesperado
- `feature` - Nueva funcionalidad
- `enhancement` - Mejora a funcionalidad existente
- `documentation` - Mejoras o adiciones a documentación
- `performance` - Problemas de rendimiento
- `security` - Vulnerabilidades de seguridad
- `refactoring` - Refactorización de código

### Por Prioridad
- `priority: critical` - Requiere atención inmediata
- `priority: high` - Alta prioridad
- `priority: medium` - Prioridad media
- `priority: low` - Baja prioridad

### Por Estado
- `needs-triage` - Requiere revisión inicial
- `needs-investigation` - Requiere investigación adicional
- `blocked` - Bloqueado por otro issue o factor externo
- `in-progress` - En desarrollo activo
- `ready-for-review` - Listo para code review

### Por Dificultad
- `good first issue` - Bueno para nuevos contribuidores
- `help wanted` - Se busca ayuda de la comunidad
- `difficulty: easy` - Fácil de implementar
- `difficulty: medium` - Complejidad media
- `difficulty: hard` - Alta complejidad

### Por Área
- `frontend` - Relacionado con frontend
- `backend` - Relacionado con backend
- `database` - Relacionado con base de datos
- `api` - Relacionado con API
- `infrastructure` - Relacionado con infraestructura
- `testing` - Relacionado con testing

---

## 🔗 Referencias

- [GitHub Docs - About Issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues)
- [GitHub Docs - Issue Templates](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/about-issue-and-pull-request-templates)
- [How to Write a Good Bug Report](https://developer.mozilla.org/en-US/docs/Mozilla/QA/Bug_writing_guidelines)

---

**Nota:** Estos templates son guías flexibles. Adapta según las necesidades y cultura de tu equipo/proyecto.
