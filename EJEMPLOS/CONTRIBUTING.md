# Guía de Contribución

¡Gracias por tu interés en contribuir a este proyecto! Esta guía te ayudará a entender cómo puedes participar de manera efectiva.

---

## 📋 Tabla de Contenidos

- [Código de Conducta](#-código-de-conducta)
- [¿Cómo Puedo Contribuir?](#-cómo-puedo-contribuir)
- [Proceso de Contribución](#-proceso-de-contribución)
- [Estándares de Código](#-estándares-de-código)
- [Convención de Commits](#-convención-de-commits)
- [Convención de Branches](#-convención-de-branches)
- [Pull Request Process](#-pull-request-process)
- [Reportar Bugs](#-reportar-bugs)
- [Sugerir Mejoras](#-sugerir-mejoras)
- [Preguntas Frecuentes](#-preguntas-frecuentes)

---

## 📜 Código de Conducta

Este proyecto y todos los que participan en él se rigen por nuestro [Código de Conducta](CODE_OF_CONDUCT.md). Al participar, se espera que mantengas este código. Por favor reporta comportamientos inaceptables a [email@proyecto.com].

### Nuestros Estándares

**Comportamientos que contribuyen a crear un ambiente positivo:**

✅ Usar lenguaje acogedor e inclusivo
✅ Respetar diferentes puntos de vista y experiencias
✅ Aceptar críticas constructivas con gracia
✅ Enfocarse en lo que es mejor para la comunidad
✅ Mostrar empatía hacia otros miembros

**Comportamientos inaceptables:**

❌ Uso de lenguaje o imágenes sexualizadas
❌ Comentarios insultantes o despectivos (trolling)
❌ Acoso público o privado
❌ Publicar información privada de otros sin permiso
❌ Otras conductas no éticas o no profesionales

---

## 🤝 ¿Cómo Puedo Contribuir?

Hay muchas formas de contribuir a este proyecto:

### 1. 🐛 Reportar Bugs

Los bugs se rastrean como [GitHub Issues](../../issues). Cuando reportes un bug:

- **Usa un título claro y descriptivo**
- **Describe los pasos exactos para reproducir el problema**
- **Proporciona ejemplos específicos**
- **Describe el comportamiento observado vs. el esperado**
- **Incluye screenshots si es posible**
- **Especifica tu ambiente** (OS, versión, navegador, etc.)

Ver la [plantilla de Bug Report](PROPUESTA_ISSUES.md#-bug-report) para más detalles.

### 2. ✨ Sugerir Nuevas Funcionalidades

Las sugerencias de funcionalidades también se rastrean como [GitHub Issues](../../issues). Cuando sugieras una feature:

- **Usa un título claro y descriptivo**
- **Proporciona una descripción detallada de la funcionalidad**
- **Explica por qué esta funcionalidad sería útil**
- **Incluye ejemplos de uso si es posible**
- **Lista proyectos similares donde existe** (si aplica)

Ver la [plantilla de Feature Request](PROPUESTA_ISSUES.md#-feature-request) para más detalles.

### 3. 📝 Mejorar la Documentación

La documentación siempre puede mejorar. Puedes:

- Corregir errores tipográficos o gramaticales
- Agregar ejemplos o casos de uso
- Mejorar explicaciones existentes
- Traducir documentación a otros idiomas
- Crear tutoriales o guías

### 4. 💻 Contribuir con Código

Puedes contribuir con:

- Implementar nuevas funcionalidades
- Corregir bugs reportados
- Mejorar el rendimiento
- Refactorizar código existente
- Agregar tests
- Mejorar la accesibilidad

### 5. 🧪 Testing

Ayuda probando:

- Nuevas versiones antes del release
- Features en desarrollo
- Diferentes ambientes y configuraciones
- Reportar bugs encontrados

### 6. 🎨 Diseño

Contribuye con:

- Mejoras de UI/UX
- Diseños de nuevas features
- Iconos e ilustraciones
- Mejoras de accesibilidad

---

## 🔄 Proceso de Contribución

### Paso 1: Fork del Repositorio

1. Haz clic en el botón "Fork" en la esquina superior derecha
2. Clona tu fork localmente:

```bash
git clone https://github.com/TU_USUARIO/nombre-proyecto.git
cd nombre-proyecto
```

3. Agrega el repositorio original como remote:

```bash
git remote add upstream https://github.com/ORGANIZACION/nombre-proyecto.git
```

### Paso 2: Configurar el Ambiente de Desarrollo

1. Instala las dependencias:

```bash
npm install
```

2. Copia el archivo de configuración:

```bash
cp .env.example .env
```

3. Configura las variables de entorno necesarias

4. Ejecuta el proyecto localmente:

```bash
npm run dev
```

5. Ejecuta los tests para verificar que todo funciona:

```bash
npm test
```

### Paso 3: Crear una Branch

Crea una branch desde `develop` para tu trabajo:

```bash
git checkout develop
git pull upstream develop
git checkout -b tipo/descripcion-breve
```

Ver [Convención de Branches](#-convención-de-branches) para más detalles.

### Paso 4: Hacer tus Cambios

1. **Escribe código limpio y bien documentado**
2. **Sigue los estándares de código** del proyecto
3. **Agrega tests** para nuevas funcionalidades
4. **Actualiza la documentación** si es necesario
5. **Verifica que los tests pasen**:

```bash
npm test
npm run lint
```

### Paso 5: Commit de tus Cambios

Usa commits pequeños y descriptivos siguiendo la [Convención de Commits](#-convención-de-commits):

```bash
git add .
git commit -m "feat(auth): agregar autenticación con OAuth2"
```

### Paso 6: Mantén tu Branch Actualizada

Sincroniza regularmente con el repositorio upstream:

```bash
git fetch upstream
git rebase upstream/develop
```

Si hay conflictos, resuélvelos antes de continuar.

### Paso 7: Push a tu Fork

```bash
git push origin tipo/descripcion-breve
```

### Paso 8: Crear un Pull Request

1. Ve a tu fork en GitHub
2. Haz clic en "Pull Request"
3. Selecciona tu branch y la branch `develop` del repositorio original
4. Completa la plantilla de PR con:
   - Descripción clara de los cambios
   - Issues relacionados (usa `Fixes #123` o `Closes #123`)
   - Screenshots (si aplica)
   - Checklist completado
5. Asigna reviewers apropiados
6. Agrega labels relevantes

---

## 📏 Estándares de Código

### Estilo de Código

Seguimos guías de estilo estándar de la industria:

- **JavaScript/TypeScript**: [Airbnb Style Guide](https://github.com/airbnb/javascript)
- **Python**: [PEP 8](https://www.python.org/dev/peps/pep-0008/)
- **CSS**: [BEM Methodology](http://getbem.com/)

### Herramientas de Linting

El proyecto usa herramientas automáticas para mantener consistencia:

```bash
# Ejecutar linter
npm run lint

# Corregir automáticamente problemas de estilo
npm run lint:fix

# Formatear código
npm run format
```

### Buenas Prácticas

**General:**
- ✅ Código auto-documentado con nombres descriptivos
- ✅ Funciones pequeñas con una sola responsabilidad
- ✅ Evitar código duplicado (DRY - Don't Repeat Yourself)
- ✅ Comentarios solo cuando sea necesario explicar el "por qué"
- ✅ Manejo apropiado de errores

**JavaScript/TypeScript:**
```javascript
// ❌ Malo
function fn(x) {
  return x * 2;
}

// ✅ Bueno
function duplicateValue(value) {
  return value * 2;
}
```

**Componentes:**
```javascript
// ✅ Bueno: Componente pequeño, responsabilidad única
export function UserAvatar({ user, size = 'md' }) {
  return (
    <img 
      src={user.avatarUrl} 
      alt={`Avatar de ${user.name}`}
      className={`avatar avatar-${size}`}
    />
  );
}
```

### Testing

**Tests son obligatorios para:**
- ✅ Nuevas funcionalidades
- ✅ Correcciones de bugs
- ✅ Cambios en lógica de negocio

**Coverage mínimo:**
- Líneas: 80%
- Funciones: 80%
- Branches: 75%

```bash
# Ejecutar tests
npm test

# Tests con coverage
npm run test:coverage

# Tests en modo watch
npm run test:watch
```

**Ejemplo de test:**
```javascript
describe('duplicateValue', () => {
  it('debe duplicar números positivos', () => {
    expect(duplicateValue(5)).toBe(10);
  });

  it('debe manejar cero', () => {
    expect(duplicateValue(0)).toBe(0);
  });

  it('debe duplicar números negativos', () => {
    expect(duplicateValue(-3)).toBe(-6);
  });
});
```

### Documentación de Código

**JSDoc para funciones públicas:**
```javascript
/**
 * Calcula el precio total incluyendo impuestos
 * @param {number} basePrice - Precio base del producto
 * @param {number} taxRate - Tasa de impuesto (0.0 a 1.0)
 * @returns {number} Precio total con impuestos
 * @throws {Error} Si basePrice es negativo
 * @example
 * calculateTotalPrice(100, 0.19) // returns 119
 */
function calculateTotalPrice(basePrice, taxRate) {
  if (basePrice < 0) {
    throw new Error('El precio base no puede ser negativo');
  }
  return basePrice * (1 + taxRate);
}
```

---

## 📝 Convención de Commits

Seguimos [Conventional Commits](https://www.conventionalcommits.org/) para mantener un historial limpio y generar changelogs automáticamente.

### Formato

```
<tipo>(<scope>): <descripción corta>

[cuerpo opcional]

[footer opcional]
```

### Tipos de Commit

| Tipo | Descripción | Ejemplo |
|------|-------------|---------|
| `feat` | Nueva funcionalidad | `feat(auth): agregar login con Google` |
| `fix` | Corrección de bug | `fix(api): corregir error 500 en /users` |
| `docs` | Solo cambios en documentación | `docs(readme): actualizar guía de instalación` |
| `style` | Cambios de formato (espacios, comas, etc.) | `style(components): formatear código con prettier` |
| `refactor` | Refactorización sin cambiar funcionalidad | `refactor(auth): simplificar lógica de validación` |
| `perf` | Mejoras de performance | `perf(db): optimizar query de usuarios` |
| `test` | Agregar o modificar tests | `test(utils): agregar tests para formatDate` |
| `build` | Cambios en sistema de build o dependencias | `build(deps): actualizar react a v18` |
| `ci` | Cambios en configuración de CI/CD | `ci(github): agregar workflow para tests` |
| `chore` | Tareas de mantenimiento | `chore(deps): actualizar dependencias` |
| `revert` | Revertir commit anterior | `revert: feat(auth): agregar login con Google` |

### Scope

El scope es opcional pero recomendado. Indica la parte del código afectada:

- `auth` - Autenticación
- `api` - API endpoints
- `ui` - Interfaz de usuario
- `db` - Base de datos
- `config` - Configuración
- `tests` - Tests
- `docs` - Documentación

### Descripción

- Usa imperativo, presente: "agregar" no "agregado" ni "agrega"
- No capitalices la primera letra
- No uses punto al final
- Máximo 72 caracteres

### Body (Opcional)

Proporciona contexto adicional sobre los cambios:

```
feat(api): agregar endpoint para exportar reportes

Implementa nuevo endpoint POST /api/reports/export que permite
exportar reportes en formato PDF y Excel. Incluye validación
de permisos y límite de tamaño de datos.
```

### Footer (Opcional)

Usa el footer para:

- Referenciar issues: `Refs #123` o `Related to #456`
- Cerrar issues: `Fixes #123`, `Closes #456`, `Resolves #789`
- Breaking changes: `BREAKING CHANGE: descripción`

```
feat(api): cambiar formato de respuesta de /users

BREAKING CHANGE: El endpoint /users ahora devuelve un objeto
con paginación en lugar de un array directo.

Antes: { users: [...] }
Ahora: { data: [...], pagination: {...} }

Closes #234
```

### Ejemplos Completos

**Feature simple:**
```
feat(dashboard): agregar gráfico de estadísticas mensuales
```

**Bug fix con detalle:**
```
fix(auth): corregir validación de token expirado

El middleware de autenticación no manejaba correctamente
tokens JWT expirados, causando error 500 en lugar de 401.

Fixes #123
```

**Refactoring:**
```
refactor(services): extraer lógica de email a servicio dedicado

Se mueve toda la lógica de envío de emails desde controllers
a un nuevo EmailService para mejor separación de responsabilidades.
```

**Breaking change:**
```
feat(api): migrar de REST a GraphQL

BREAKING CHANGE: Todos los endpoints REST han sido removidos.
Ahora se debe usar el endpoint GraphQL /graphql para todas
las operaciones.

Migración: Ver docs/migration-graphql.md

Closes #456
```

---

## 🌿 Convención de Branches

Usa nombres descriptivos que indiquen el propósito de la branch.

### Formato

```
<tipo>/<descripcion-con-guiones>
```

### Tipos de Branch

| Tipo | Uso | Ejemplo |
|------|-----|---------|
| `feature/` | Nuevas funcionalidades | `feature/oauth-login` |
| `fix/` o `bugfix/` | Corrección de bugs | `fix/user-validation-error` |
| `hotfix/` | Correcciones urgentes en producción | `hotfix/security-patch` |
| `refactor/` | Refactorización | `refactor/extract-email-service` |
| `docs/` | Solo documentación | `docs/update-contributing-guide` |
| `test/` | Tests | `test/add-integration-tests` |
| `chore/` | Tareas de mantenimiento | `chore/update-dependencies` |
| `perf/` | Mejoras de performance | `perf/optimize-database-queries` |
| `style/` | Cambios de estilo/formato | `style/apply-new-design-system` |

### Reglas

1. **Usa minúsculas** y separa palabras con guiones
2. **Sé descriptivo** pero conciso (máximo 50 caracteres)
3. **Usa inglés** preferentemente para consistencia
4. **Referencia issues** si aplica: `feature/add-oauth-#123`
5. **Una branch por feature/fix**: No mezcles cambios no relacionados

### Ejemplos

```bash
# ✅ Buenos ejemplos
feature/user-authentication
fix/payment-validation-error
hotfix/csrf-vulnerability
refactor/simplify-api-client
docs/add-deployment-guide
test/user-service-unit-tests

# ❌ Malos ejemplos
my-changes              # No descriptivo
Feature/UserAuth        # No usar mayúsculas
fix-stuff               # Demasiado vague
feature-123             # Solo número sin descripción
```

### Flujo de Branches

```
main (producción - solo releases)
  ↑
develop (desarrollo - branch principal)
  ↑
feature/nueva-funcionalidad
fix/correccion-bug
hotfix/arreglo-urgente
```

**Flujo de trabajo estándar:**

```bash
# 1. Crear feature desde develop
git checkout develop
git pull origin develop
git checkout -b feature/mi-funcionalidad

# 2. Hacer commits y push
git push origin feature/mi-funcionalidad

# 3. Crear PR hacia develop (NO hacia main)
# El PR será revisado y mergeado a develop

# 4. Deploy a producción (solo maintainers)
# Los maintainers crearán un PR de develop → main cuando sea momento de release
git checkout main
git merge develop --no-ff
git tag -a v1.2.3 -m "Release version 1.2.3"
git push origin main --tags
```

**Para hotfixes urgentes en producción:**

```bash
# Crear hotfix desde main
git checkout main
git pull origin main
git checkout -b hotfix/arreglo-critico

# Después de arreglar, merge a AMBAS branches:
# 1. PR a main para fix inmediato en producción
# 2. PR a develop para mantener sincronizado
```

---

## 🔍 Pull Request Process

### Antes de Crear el PR

**Checklist:**

- [ ] Código cumple con estándares de estilo
- [ ] Tests agregados/actualizados y pasando
- [ ] Documentación actualizada
- [ ] Branch actualizada con `develop`
- [ ] No hay conflictos de merge
- [ ] Commit messages siguen convención
- [ ] Build local exitoso

```bash
# Verificar todo antes del PR
npm run lint
npm test
npm run build
```

### Crear el Pull Request

1. **Título descriptivo** siguiendo convención de commits:
   ```
   feat(auth): agregar autenticación con OAuth2
   ```

2. **Usar la plantilla de PR** (si existe)

3. **Descripción completa:**

```markdown
## 📝 Descripción

Implementa autenticación OAuth2 con Google y GitHub.

## 🔗 Issues Relacionados

Closes #123
Related to #456

## 🎯 Tipo de Cambio

- [x] Nueva funcionalidad (cambio no-breaking que agrega funcionalidad)
- [ ] Bug fix (cambio no-breaking que corrige un issue)
- [ ] Breaking change (fix o feature que causa que funcionalidad existente no funcione como se esperaba)
- [ ] Cambio de documentación

## 🧪 ¿Cómo se ha Testeado?

- [x] Tests unitarios
- [x] Tests de integración
- [x] Tests manuales en local
- [ ] Tests en staging

**Casos de prueba:**
1. Login con Google exitoso
2. Login con GitHub exitoso
3. Manejo de error cuando usuario cancela
4. Token refresh cuando expira

## 📸 Screenshots (si aplica)

[Agregar screenshots aquí]

## ✅ Checklist

- [x] Mi código sigue el estilo de este proyecto
- [x] He realizado un self-review de mi código
- [x] He comentado mi código donde era necesario
- [x] He actualizado la documentación
- [x] Mis cambios no generan nuevos warnings
- [x] He agregado tests que prueban que mi fix es efectivo o que mi feature funciona
- [x] Tests unitarios nuevos y existentes pasan localmente
- [x] Cualquier cambio dependiente ha sido mergeado y publicado
```

### Durante el Code Review

**Como autor:**

- ✅ Responde a comentarios de manera constructiva
- ✅ Haz cambios solicitados en commits separados (no force push)
- ✅ Marca conversaciones como resueltas cuando corresponda
- ✅ Agradece el feedback

**Como reviewer:**

- ✅ Sé respetuoso y constructivo
- ✅ Explica el "por qué" de tus sugerencias
- ✅ Diferencia entre bloqueos y sugerencias opcionales
- ✅ Aprueba cuando esté listo o solicita cambios claramente

**Tipos de comentarios:**

```markdown
# 🚨 Blocker - Debe corregirse antes del merge
Este código tiene un bug que causará error en producción.

# 💡 Sugerencia - Opcional pero recomendado
Considera usar `map()` en lugar de `forEach()` aquí para mejor performance.

# ❓ Pregunta - Necesita clarificación
¿Por qué elegiste este approach en lugar de usar la librería X?

# 🎓 Educacional - Información adicional
FYI: Este patrón se llama "Observer Pattern" y es útil porque...
```

### Criterios para Aprobar

El PR debe cumplir:

- ✅ Funcionalidad correcta
- ✅ Tests adecuados con buen coverage
- ✅ Código legible y mantenible
- ✅ Sin vulnerabilidades de seguridad
- ✅ Performance aceptable
- ✅ Documentación actualizada
- ✅ No introduce deuda técnica significativa

### Merge

**Quién puede hacer merge:**

- Maintainers del proyecto
- Contributors con permisos de write
- Autor del PR (solo después de aprobación)

**Estrategias de merge:**

1. **Squash and merge** (recomendado para features pequeñas):
   - Combina todos los commits en uno
   - Mantiene historial limpio
   - Usa cuando hay muchos commits pequeños

2. **Merge commit** (para features grandes):
   - Mantiene todo el historial de commits
   - Usa cuando los commits son significativos

3. **Rebase and merge** (para historial lineal):
   - Aplica commits uno por uno sin merge commit
   - Usa cuando quieres historial completamente lineal

**Después del merge:**

```bash
# Actualiza tu repo local
git checkout develop
git pull origin develop

# Borra la branch
git branch -d feature/mi-funcionalidad
git push origin --delete feature/mi-funcionalidad
```

---

## 🐛 Reportar Bugs

### Antes de Reportar

1. **Busca en issues existentes** para evitar duplicados
2. **Verifica que sea un bug** y no un malentendido
3. **Reproduce el bug** en la última versión
4. **Recolecta información** sobre el ambiente

### Crear el Issue

Usa la plantilla de [Bug Report](PROPUESTA_ISSUES.md#-bug-report) e incluye:

**Información esencial:**
- Descripción clara del bug
- Pasos para reproducir
- Comportamiento esperado vs. actual
- Screenshots o videos
- Ambiente (OS, versión, navegador)
- Logs o mensajes de error

**Ejemplo:**

```markdown
## 🐛 Descripción del Bug

El botón "Guardar" no responde en formularios con más de 10 campos.

## 📝 Pasos para Reproducir

1. Navegar a `/admin/products/new`
2. Completar todos los 12 campos del formulario
3. Hacer clic en "Guardar"
4. El botón no responde

## 🎯 Comportamiento Esperado

El formulario debería guardarse y mostrar mensaje de éxito.

## 🔴 Comportamiento Actual

El botón no hace nada, no hay feedback visual.

## 🖥️ Ambiente

- OS: Windows 11
- Navegador: Chrome 120
- Versión: 1.3.0
```

---

## 💡 Sugerir Mejoras

### Tipos de Mejoras

- **Nuevas funcionalidades**: Features completamente nuevas
- **Enhancements**: Mejoras a features existentes
- **Optimizaciones**: Mejoras de performance
- **UX**: Mejoras de experiencia de usuario

### Crear la Propuesta

Usa la plantilla de [Feature Request](PROPUESTA_ISSUES.md#-feature-request) e incluye:

**Información clave:**
- Descripción clara de la mejora
- Problema que resuelve
- Solución propuesta
- Alternativas consideradas
- Mockups o wireframes (si aplica)

**Justificación:**
- ¿Cuántos usuarios se beneficiarían?
- ¿Qué tan frecuente es la necesidad?
- ¿Alineado con visión del proyecto?

---

## ❓ Preguntas Frecuentes

### General

**P: ¿Necesito experiencia previa para contribuir?**
R: No necesariamente. Tenemos issues etiquetados como `good first issue` perfectos para comenzar.

**P: ¿Cuánto tiempo toma que revisen mi PR?**
R: Generalmente 2-5 días hábiles. Si es urgente, menciona a los maintainers.

**P: ¿Puedo trabajar en un issue que ya está asignado?**
R: Pregunta primero en el issue. Si no hay actividad reciente, probablemente puedas tomarlo.

**P: ¿Qué hago si mi PR tiene conflictos?**
R: Actualiza tu branch con `develop`:
```bash
git fetch upstream
git rebase upstream/develop
# Resolver conflictos
git push -f origin tu-branch
```

### Técnicas

**P: ¿Debo hacer squash de mis commits antes del PR?**
R: No es necesario. Lo haremos al hacer merge si es apropiado.

**P: ¿Qué coverage de tests es requerido?**
R: Mínimo 80% para líneas de código. Usa `npm run test:coverage` para verificar.

**P: ¿Puedo usar librerías de terceros?**
R: Consulta primero. Preferimos minimizar dependencias. Justifica por qué es necesaria.

**P: ¿Cómo manejo secrets en desarrollo?**
R: Nunca subas secrets al repo. Usa `.env` (que está en `.gitignore`) y documenta variables necesarias en `.env.example`.

### Proceso

**P: ¿Cuándo se deployean los cambios?**
R: Dependiendo del proyecto:
- Hot fixes: Inmediatamente
- Features: En el siguiente release (generalmente semanal/quincenal)

**P: Mi PR fue rechazado, ¿qué hago?**
R: Lee el feedback, haz las correcciones solicitadas, y actualiza el PR. No te desanimes.

**P: ¿Puedo contribuir sin saber programar?**
R: ¡Sí! Puedes ayudar con:
- Documentación
- Traducción
- Diseño
- Testing
- Reportar bugs

---

## 🎓 Recursos Adicionales

### Aprendizaje

- [GitHub Flow Guide](https://guides.github.com/introduction/flow/)
- [Pro Git Book](https://git-scm.com/book/en/v2)
- [Conventional Commits](https://www.conventionalcommits.org/)
- [How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/)
- [Code Review Best Practices](https://google.github.io/eng-practices/review/)

### Herramientas

- [GitHub CLI](https://cli.github.com/) - Gestiona PRs desde terminal
- [commitizen](https://github.com/commitizen/cz-cli) - Ayuda con commits convencionales
- [husky](https://typicode.github.io/husky/) - Git hooks automáticos
- [lint-staged](https://github.com/okonet/lint-staged) - Lint solo archivos staged

### Comunidad

- [Discord/Slack del proyecto] - Chat en tiempo real
- [GitHub Discussions](../../discussions) - Foro de discusión
- [Stack Overflow Tag] - Preguntas técnicas

---

**¡Gracias por contribuir! 🎉**

Tu tiempo y esfuerzo ayudan a hacer este proyecto mejor para todos.
