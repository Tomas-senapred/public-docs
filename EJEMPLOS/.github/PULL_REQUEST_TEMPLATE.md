## 📝 Descripción

<!-- Proporciona un resumen claro y conciso de los cambios que introduces -->

### ¿Qué hace este PR?

<!-- Describe qué problema resuelve o qué funcionalidad agrega -->

### ¿Por qué es necesario?

<!-- Explica el contexto y la motivación detrás de estos cambios -->

---

## 🔗 Issues Relacionados

<!-- Vincula los issues que este PR resuelve o está relacionado -->

Closes #
Related to #

---

## 🎯 Tipo de Cambio

<!-- Marca con una X las opciones que apliquen -->

- [ ] 🐛 Bug fix (cambio no-breaking que corrige un issue)
- [ ] ✨ Nueva funcionalidad (cambio no-breaking que agrega funcionalidad)
- [ ] 💥 Breaking change (fix o feature que causa que funcionalidad existente no funcione como se esperaba)
- [ ] 📝 Cambios en documentación
- [ ] 🎨 Cambios de estilo/formato (sin cambios en lógica)
- [ ] ♻️ Refactorización (sin cambios en funcionalidad)
- [ ] ⚡ Mejoras de performance
- [ ] ✅ Cambios en tests
- [ ] 🔧 Cambios en configuración o build
- [ ] 🔒 Cambios relacionados con seguridad

---

## 🧪 ¿Cómo se ha Testeado?

<!-- Describe las pruebas que realizaste para verificar tus cambios -->

### Tests Automatizados

- [ ] Tests unitarios agregados/actualizados
- [ ] Tests de integración agregados/actualizados
- [ ] Tests E2E agregados/actualizados
- [ ] Todos los tests existentes pasan

### Tests Manuales

<!-- Describe los escenarios que probaste manualmente -->

**Casos de prueba:**
1. 
2. 
3. 

**Ambientes probados:**
- [ ] Local
- [ ] Staging
- [ ] Otro: ___________

---

## 📸 Screenshots / Videos

<!-- Si aplica, agrega capturas de pantalla o videos que ayuden a entender los cambios visuales -->

### Antes

<!-- Screenshot/video del comportamiento anterior -->

### Después

<!-- Screenshot/video del nuevo comportamiento -->

---

## 📋 Checklist

### General

- [ ] Mi código sigue las guías de estilo de este proyecto
- [ ] He realizado un self-review de mi código
- [ ] He comentado mi código donde era necesario, especialmente en áreas complejas
- [ ] He actualizado la documentación correspondiente
- [ ] Mis cambios no generan nuevos warnings
- [ ] He actualizado el CHANGELOG.md (si aplica)

### Tests

- [ ] He agregado tests que prueban que mi fix es efectivo o que mi feature funciona
- [ ] Tests unitarios nuevos y existentes pasan localmente con mis cambios
- [ ] Coverage de tests se mantiene o mejora (mínimo 80%)

### Código

- [ ] He ejecutado el linter y corregido todos los errores (`npm run lint`)
- [ ] He formateado el código según el estándar del proyecto (`npm run format`)
- [ ] No hay console.logs u otros debugging code
- [ ] No hay código comentado innecesario
- [ ] He manejado apropiadamente los errores

### Base de Datos (si aplica)

- [ ] He creado/actualizado migraciones de base de datos
- [ ] Las migraciones se pueden ejecutar y revertir correctamente
- [ ] He actualizado seeders si es necesario
- [ ] He testeado las migraciones en ambiente local

### Dependencias (si aplica)

- [ ] He actualizado package.json con nuevas dependencias
- [ ] He documentado por qué se agregaron nuevas dependencias
- [ ] He verificado que no hay vulnerabilidades de seguridad (`npm audit`)
- [ ] He actualizado package-lock.json

### Breaking Changes

<!-- Si marcaste "Breaking change" arriba, responde lo siguiente -->

- [ ] He documentado claramente los breaking changes en el PR
- [ ] He actualizado la guía de migración (si existe)
- [ ] He notificado al equipo sobre estos cambios
- [ ] He actualizado la versión semver apropiadamente

### Otros

- [ ] He sincronizado mi branch con `develop` (o `main`)
- [ ] No hay conflictos de merge
- [ ] El build de producción se ejecuta correctamente (`npm run build`)
- [ ] He revisado el diff completo en GitHub

---

## 🔍 Notas para Reviewers

<!-- Información adicional que quieras que los reviewers sepan -->

### Áreas que requieren atención especial

<!-- Marca las áreas donde especialmente necesitas feedback -->

- [ ] Lógica de negocio compleja
- [ ] Performance
- [ ] Seguridad
- [ ] Arquitectura/Diseño
- [ ] Accesibilidad
- [ ] Otro: ___________

### Preguntas para el equipo

<!-- Si tienes dudas o necesitas discutir algo específico -->

1. 
2. 

---

## 📚 Documentación Adicional

<!-- Enlaces a documentación relevante, RFCs, diseños, etc. -->

- [Documentación técnica](link)
- [Diseño en Figma](link)
- [RFC o propuesta](link)
- [Ticket en Jira](link)

---

## 🚀 Plan de Deployment

<!-- Si este PR requiere pasos especiales para el deployment -->

### Pre-deployment

- [ ] Crear backup de base de datos
- [ ] Notificar a usuarios sobre mantenimiento (si aplica)
- [ ] Otro: ___________

### Deployment

- [ ] Ejecutar migraciones de base de datos
- [ ] Limpiar caché
- [ ] Reiniciar workers/servicios
- [ ] Otro: ___________

### Post-deployment

- [ ] Verificar logs por errores
- [ ] Monitorear métricas clave
- [ ] Smoke tests en producción
- [ ] Otro: ___________

---

## ⚠️ Riesgos

<!-- Identifica posibles riesgos asociados con este cambio -->

- [ ] Sin riesgos identificados
- [ ] Riesgo bajo
- [ ] Riesgo medio - Describir: ___________
- [ ] Riesgo alto - Describir: ___________

---

## 🎉 Información Adicional

<!-- Cualquier otra información que consideres relevante -->

---

<!-- 
NOTA PARA EL AUTOR DEL PR:

1. Asegúrate de completar TODAS las secciones relevantes
2. Remueve secciones que no apliquen a tu PR
3. Sé específico y detallado en tus respuestas
4. Si tienes dudas, pregunta antes de enviar el PR
5. Revisa que tu PR apunte a la branch correcta (develop, no main)

NOTA PARA REVIEWERS:

1. Verifica que el checklist esté completo
2. Haz checkout de la branch y prueba localmente si es posible
3. Sé constructivo en tus comentarios
4. Aprueba solo cuando todos los checks estén en verde
5. Si solicitas cambios, sé claro sobre qué es blocking vs. nice-to-have

¡Gracias por contribuir! 🙏
-->
