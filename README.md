# 🎨 Portafolio de Rubén Carmona

Bienvenido al repositorio del portafolio personal. Este proyecto es un sitio web construido con **Astro** que puedes modificar y mejorar siguiendo este flujo de trabajo.

---

## 📋 Índice

1. [Requisitos previos](#requisitos-previos)
2. [Herramientas sugeridas](#herramientas-sugeridas)
3. [Clonar el proyecto](#clonar-el-proyecto)
4. [Levantar el proyecto en local](#levantar-el-proyecto-en-local)
5. [Flujo de trabajo (Git + GitHub)](#flujo-de-trabajo-git--github)
6. [Reglas de Naming y Branching](#reglas-de-naming-y-branching)
7. [Crear una rama](#crear-una-rama)
8. [Comandos Git básicos](#comandos-git-básicos)
9. [Crear un Issue](#crear-un-issue)
10. [Crear una Pull Request (PR)](#crear-una-pull-request-pr)
11. [Aprobación y merge](#aprobación-y-merge)

---

## 📌 Requisitos previos

Necesitas tener instalado:

- **Git**: [Descargar Git](https://git-scm.com/)
- **Node.js** (versión 22.12.0 o superior): [Descargar Node.js](https://nodejs.org/)

Para verificar que están instalados, abre la terminal y escribe:

```bash
git --version
node --version
```

---

## 🛠️ Herramientas sugeridas

Se recomienda usar las siguientes herramientas para una experiencia de desarrollo óptima:

### **OpenCode**
Agente de IA de código abierto para asistencia en desarrollo.
- [OpenCode.ai](https://opencode.ai/)
- Ideal para obtener ayuda con generación de código y refactorización

### **Warp**
Terminal moderna y potente con características avanzadas.
- [Descargar Warp](https://www.warp.dev/)
- Facilita el trabajo con Git y comandos

### **Visual Studio Code (VS Code)**
El editor más popular para desarrollo web.
- [Descargar VS Code](https://code.visualstudio.com/)
- Recomendado: Instala las extensiones "Astro" y "Git Graph" para mejor experiencia

**Extensiones recomendadas para VS Code:**
```
- Astro (Official)
- Prettier - Code formatter
- Git Graph
- Tailwind CSS IntelliSense
- Thunder Client (o Postman)
```

---

## 🔄 Clonar el proyecto

1. Abre la terminal en la carpeta donde quieras guardar el proyecto
2. Ejecuta este comando:

```bash
git clone https://github.com/MMoza/ruben-carmona.git
```

3. Entra en la carpeta del proyecto:

```bash
cd ruben-carmona
```

¡Listo! Ya tienes el código en tu computadora.

---

## 🚀 Levantar el proyecto en local

1. Instala las dependencias (solo la primera vez):

```bash
npm install
```

2. Inicia el servidor de desarrollo:

```bash
npm run dev
```

3. Abre tu navegador y ve a:

```
http://localhost:3000
```

Verás el portafolio en tu computadora. Cualquier cambio que hagas se actualizará automáticamente.

4. Para detener el servidor, presiona `Ctrl + C` en la terminal.

---

## 🌳 Flujo de trabajo (Git + GitHub)

Este es el proceso recomendado para trabajar:

```
┌─────────────────────────────────────────┐
│ 1. Crear un Issue                       │
│    (describe qué quieres cambiar)       │
└──────────────┬──────────────────────────┘
               │
┌──────────────▼──────────────────────────┐
│ 2. Crear una rama (branch)              │
│    (basada en el Issue)                 │
└──────────────┬──────────────────────────┘
               │
┌──────────────▼──────────────────────────┐
│ 3. Hacer cambios y commits             │
│    (trabajar en tu rama)                │
└──────────────┬──────────────────────────┘
               │
┌──────────────▼──────────────────────────┐
│ 4. Crear un Pull Request (PR)           │
│    (proponer tus cambios)               │
└──────────────┬──────────────────────────┘
               │
┌──────────────▼──────────────────────────┐
│ 5. Revisar y Merge ✅                   │
│    (solo MMoza acepta la PR)            │
└─────────────────────────────────────────┘
```

---

## 📐 Reglas de Naming y Branching

Para mantener un historial limpio y legible, seguimos estas convenciones:

### **Nombres de Ramas (Branch Naming)**

Las ramas deben seguir este formato:

```
<tipo>/<descripción>
```

#### **Tipos de rama permitidos:**

| Tipo | Uso | Ejemplo |
|------|-----|---------|
| `feature/` | Nuevas funcionalidades | `feature/agregar-seccion-blog` |
| `fix/` | Corrección de bugs | `fix/corregir-responsive-mobile` |
| `docs/` | Cambios en documentación | `docs/actualizar-readme` |
| `style/` | Cambios de estilos/CSS | `style/mejorar-colores-footer` |
| `refactor/` | Refactorización de código | `refactor/optimizar-componentes` |
| `perf/` | Mejoras de rendimiento | `perf/optimizar-imagenes` |
| `test/` | Cambios en tests | `test/agregar-tests-componentes` |

#### **Reglas para el nombre:**

- ✅ Usa guiones `-` para separar palabras (NO espacios)
- ✅ Usa minúsculas
- ✅ Sé descriptivo pero conciso (máximo 50 caracteres)
- ✅ Evita caracteres especiales
- ❌ NO uses mayúsculas: `Feature/Agregar-Blog`
- ❌ NO uses espacios: `feature/agregar seccion`
- ❌ NO uses números al inicio: `feature/1-agregar-blog`

#### **Ejemplos correctos:**

```bash
feature/agregar-experiencia-laboral
fix/corregir-estilos-mobile
docs/mejorar-readme
style/actualizar-paleta-colores
refactor/simplificar-logica-componentes
perf/optimizar-imagenes-portafolio
```

---

### **Mensajes de Commits (Commit Naming)**

Los commits deben seguir este formato:

```
<tipo>(<alcance>): <descripción>
```

#### **Estructura detallada:**

```
<tipo>(<alcance>): <descripción breve>

<descripción detallada (opcional)>

<referencias (opcional)>
```

#### **Tipos de commit permitidos:**

| Tipo | Descripción | Ejemplo |
|------|-------------|---------|
| `feat` | Nueva funcionalidad | `feat(portfolio): agregar sección de certificados` |
| `fix` | Corrección de bug | `fix(navbar): corregir alineación en móvil` |
| `docs` | Cambios en documentación | `docs(readme): actualizar instrucciones` |
| `style` | Cambios de formato/CSS | `style(footer): mejorar espaciado` |
| `refactor` | Refactorización de código | `refactor(components): simplificar lógica` |
| `perf` | Mejoras de rendimiento | `perf(images): comprimir imágenes` |
| `test` | Agregación de tests | `test(api): agregar tests de autenticación` |
| `chore` | Cambios en deps o config | `chore(deps): actualizar astro a v5` |

#### **Reglas para commits:**

- ✅ Usa presente imperativo: "agregar" no "agregué" o "agregado"
- ✅ No termines con punto
- ✅ Primera letra minúscula
- ✅ Máximo 50 caracteres en la descripción
- ✅ Si es complejo, agrega descripción detallada después de línea en blanco
- ❌ NO hagas commits genéricos: `fix: cosas` o `update: varias cosas`

#### **Ejemplos correctos:**

```bash
feat(hero): agregar animación al banner principal
fix(mobile): corregir altura de las tarjetas en dispositivos pequeños
docs(contributing): agregar guía de contribución
style(theme): actualizar colores principales de la paleta
refactor(utils): extraer lógica repetida en funciones reutilizables
perf(lazy-loading): implementar lazy loading en imágenes
test(components): agregar tests unitarios para Button.astro
chore(deps): actualizar dependencias de seguridad
```

#### **Commits con descripción detallada:**

```bash
feat(blog): agregar sistema de categorías

- Crear modelo de categorías
- Actualizar componentes de blog
- Agregar filtrado por categoría
- Validar en tests

Closes #42
```

---

### **Alcances (Scope) comunes:**

Algunos alcances sugeridos:

```
portfolio    → Cambios generales del portafolio
navbar       → Barra de navegación
hero         → Sección de presentación
projects     → Sección de proyectos
skills       → Sección de habilidades
contact      → Formulario de contacto
footer       → Pie de página
components   → Componentes reutilizables
styles       → Estilos globales
config       → Configuración del proyecto
deps         → Dependencias
docs         → Documentación
tests        → Tests
```

---

## 🎯 Crear una rama

Antes de hacer cualquier cambio, crea una rama nueva. Esto te permite trabajar sin afectar la rama `main` (producción).

### 1. Asegúrate de estar en `main`:

```bash
git checkout main
```

### 2. Actualiza la rama `main` con los últimos cambios:

```bash
git pull origin main
```

### 3. Crea una rama nueva con un nombre descriptivo (siguiendo las reglas):

```bash
git checkout -b feature/nombre-del-cambio
```

**Ejemplos de nombres buenos:**
- `feature/agregar-experiencia-laboral`
- `fix/corregir-estilos-mobile`
- `feature/actualizar-foto-perfil`
- `docs/mejorar-readme`

### 4. Verifica que estés en la rama correcta:

```bash
git branch
```

Verás algo como:
```
  main
* feature/nombre-del-cambio
```

El `*` indica en qué rama estás.

---

## 🛠️ Comandos Git básicos

### Ver el estado de tus cambios:

```bash
git status
```

Te muestra qué archivos has modificado.

### Agregar cambios al "staging" (preparar para guardar):

```bash
# Agregar un archivo específico
git add nombre-del-archivo.txt

# Agregar todos los cambios
git add .
```

### Hacer un commit (guardar tus cambios):

```bash
git commit -m "tipo(alcance): descripción breve"
```

**Ejemplos siguiendo las reglas:**
```bash
git commit -m "feat(portfolio): agregar nueva sección de proyectos"
git commit -m "fix(mobile): corregir espaciado en dispositivos pequeños"
git commit -m "docs(readme): actualizar instrucciones de instalación"
```

### Subir tus cambios a GitHub:

```bash
git push origin feature/nombre-del-cambio
```

### Ver historial de cambios:

```bash
git log --oneline
```

---

## 📝 Crear un Issue

Un **Issue** es como una "tarea" o "propuesta" que describes antes de hacer cambios.

### Pasos:

1. Ve a la página del repositorio en GitHub
2. Haz clic en la pestaña **"Issues"** (abajo a la derecha de "Code")
3. Haz clic en el botón verde **"New issue"**
4. Completa:
   - **Title**: Título corto (ej: "Agregar sección de habilidades")
   - **Description**: Explica qué quieres hacer y por qué

**Ejemplo:**

```markdown
**Título:** Agregar sección de certificados

**Descripción:**
Quiero agregar una nueva sección en el portafolio para mostrar 
los certificados y cursos completados.

Cambios:
- Crear componente de certificados
- Agregar datos de ejemplo
- Verificar que se vea bien en móvil
```

5. Haz clic en **"Submit new issue"**

### ¿Por qué crear un Issue primero?

- Describes lo que vas a hacer antes de hacerlo
- MMoza puede darte feedback antes de que empieces
- Está documentado el "por qué" de cada cambio
- Puedes conectar tu PR al Issue

---

## 🔀 Crear una Pull Request (PR)

Una **Pull Request** es tu propuesta de cambios para que los revise y acepte MMoza.

### Pasos:

1. **Sube tu rama a GitHub:**

```bash
git push origin feature/nombre-del-cambio
```

2. **Ve a GitHub** y verás un botón **"Compare & pull request"** (amarillo)

3. **Haz clic** en ese botón

4. **Completa el formulario:**
   - **Title**: Resumen de qué cambiaste
   - **Description**: Explica los cambios (puedes conectar el Issue escribiendo `Closes #numero`)

**Ejemplo:**

```markdown
## 🎯 Descripción
Agregué la sección de certificados al portafolio.

## 🔗 Conectado a
Closes #5

## ✅ Cambios realizados
- [ ] Creé el componente `Certificate.astro`
- [ ] Agregué datos de ejemplo en `certificates.json`
- [ ] Revisé que se vea bien en móvil
- [ ] Sin errores en la consola

## 📸 Pantalla (opcional)
[Puedes pegar una captura si lo deseas]
```

5. **Haz clic en "Create pull request"**

### ¿Qué pasa después?

- MMoza recibirá una notificación
- Revisará tu código
- Puede pedir cambios o aprobar
- Una vez aprobado, mergea tu rama con `main`
- Tu código estará en producción ✨

---

## ✅ Aprobación y Merge

### Cuando MMoza revisa tu PR:

**Si todo está bien:**
- Le verás un ✅ verde
- Hará clic en "Merge pull request"
- Tu rama se fusionará con `main`
- Tu código estará VIVO en el portafolio

**Si hay que cambiar algo:**
- Verás comentarios en tu PR
- Haces los cambios en tu rama local
- Haces `git add .`, `git commit -m "..."`, `git push origin feature/...`
- Los cambios se actualizarán automáticamente en la PR
- Cuando esté listo, MMoza da merge ✅

### Después de merge:

Limpia tu rama local:

```bash
git checkout main
git pull origin main
git branch -d feature/nombre-del-cambio
```

¡Listo! Ya estás listo para el siguiente cambio.

---

## 📚 Resumen rápido del flujo

```bash
# 1. Clonar
git clone https://github.com/MMoza/ruben-carmona.git

# 2. Entrar
cd ruben-carmona

# 3. Instalar
npm install

# 4. Iniciar desarrollo
npm run dev

# 5. Crear rama (siguiendo las reglas)
git checkout main
git pull origin main
git checkout -b feature/tu-cambio

# 6. Hacer cambios y commitear (con reglas)
git status
git add .
git commit -m "tipo(alcance): descripción"

# 7. Subir
git push origin feature/tu-cambio

# 8. Crear PR en GitHub (web)

# 9. Esperar a MMoza ✨

# 10. Limpiar después de merge
git checkout main
git pull origin main
git branch -d feature/tu-cambio
```

---

## 🤔 Errores comunes

### "fatal: not a git repository"
→ Verifica que estés en la carpeta correcta: `cd ruben-carmona`

### "Your branch is behind origin/main"
→ Haz: `git pull origin main`

### "Changes not staged for commit"
→ Haz: `git add .` seguido de `git commit -m "mensaje"`

### "Everything up-to-date"
→ Ya todos tus cambios están en GitHub, ¡bien hecho!

---

## 📞 Necesitas ayuda?

Si algo no funciona:
1. Crea un **Issue** describiendo el problema
2. MMoza te ayudará

¡Ahora estás listo para colaborar! 🚀
