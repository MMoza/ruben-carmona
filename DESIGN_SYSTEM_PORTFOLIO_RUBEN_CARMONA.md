# DESIGN SYSTEM --- PORTFOLIO RUBÉN CARMONA

> **WEIRD, BUT INTENTIONAL.**
>
> Identidad visual para el portfolio personal de Rubén Carmona. Estética
> dark, editorial, brutalista y experimental, con una combinación
> controlada de amarillo ácido y azul eléctrico.

------------------------------------------------------------------------

## 1. Concepto visual

El portfolio debe sentirse como una **pieza editorial / póster
digital**, no como una web corporativa convencional.

La dirección artística combina:

-   Brutalismo web
-   Diseño editorial
-   Collage
-   Fotografía en blanco y negro
-   Texturas de papel / impresión
-   Tipografía display condensada
-   Elementos dibujados a mano
-   Composiciones asimétricas
-   Colores de alto contraste

La sensación general debe ser:

**RAW · CREATIVE · DIGITAL · PERSONAL · BOLD · FREAK**

### Principio fundamental

El diseño puede ser atrevido y ligeramente caótico, pero la estructura,
jerarquía y usabilidad deben permanecer perfectamente controladas.

> **CAOS VISUAL, ESTRUCTURA TÉCNICA.**

------------------------------------------------------------------------

# 2. Estructura cromática

La web es principalmente **dark**.

El fondo oscuro es la base de toda la identidad y debe utilizarse en la
mayoría de las secciones.

Las secciones con fondo claro se utilizan únicamente para generar
contraste y romper el ritmo visual.

### Distribución aproximada

-   70--80% fondo oscuro
-   20--30% fondo claro
-   Amarillo y azul únicamente como colores de acento

No crear nuevas familias cromáticas sin una razón de diseño clara.

------------------------------------------------------------------------

# 3. Paleta de colores

## 3.1 Dark Background

Color base:

``` css
--color-bg-dark: #090909;
```

Este es el fondo estructural principal.

Debe utilizarse junto con el **background oscuro oficial** proporcionado
para el proyecto.

No sustituir el background oficial por un gradiente genérico.

------------------------------------------------------------------------

## 3.2 Dark Surface

Para separar elementos dentro de las secciones oscuras:

``` css
--color-surface-dark: #111111;
--color-surface-dark-2: #181818;
```

Utilizar con moderación.

El portfolio debe mantener una apariencia predominantemente negra.

------------------------------------------------------------------------

## 3.3 Light Background

Las secciones claras utilizan el **background claro oficial**
proporcionado para el proyecto.

Como color de referencia:

``` css
--color-bg-light: #E2E0DC;
```

Este color es únicamente un fallback o referencia.

Cuando exista un asset de background oficial, debe utilizarse el asset.

------------------------------------------------------------------------

# 4. Colores de texto

## 4.1 Texto sobre fondo oscuro

### Primary Light

``` css
--color-text-light: #F2F0EA;
```

Utilizar para:

-   Headings
-   Texto principal
-   Navegación
-   Labels importantes
-   Información principal

Debe sustituir al blanco puro en la mayoría de los casos.

------------------------------------------------------------------------

### Secondary Light

``` css
--color-text-light-muted: #B8B6B0;
```

Utilizar para:

-   Descripciones
-   Metadatos
-   Texto secundario
-   Información auxiliar

------------------------------------------------------------------------

### White

``` css
--color-white: #FFFFFF;
```

Reservar para:

-   Iconos
-   Elementos de alto contraste
-   Logotipo cuando corresponda
-   Detalles gráficos

No utilizar blanco puro como color de texto general.

------------------------------------------------------------------------

# 5. Texto sobre fondo claro

## Primary Dark

``` css
--color-text-dark: #111111;
```

Utilizar para:

-   Headings
-   Texto principal
-   Navegación
-   Labels

------------------------------------------------------------------------

## Secondary Dark

``` css
--color-text-dark-muted: #454545;
```

Utilizar para:

-   Descripciones
-   Metadatos
-   Información secundaria

------------------------------------------------------------------------

# 6. Colores de acento

Los dos colores de acento oficiales son:

1.  **Amarillo ácido**
2.  **Azul eléctrico**

No introducir otros colores saturados como parte del sistema principal.

------------------------------------------------------------------------

## 6.1 Acid Yellow

Color principal de identidad:

``` css
--color-acid: #D7F821;
```

Es el color más importante después del negro.

Utilizar para:

-   CTA principales
-   Links destacados
-   Underlines
-   Elementos gráficos
-   Corona
-   Tachones
-   Highlights
-   Badges
-   Detalles de navegación
-   Hover states
-   Bloques de énfasis

El amarillo debe sentirse **eléctrico, agresivo y reconocible**.

### Regla

El amarillo es el **color de acción y personalidad**.

No utilizarlo indiscriminadamente en grandes cantidades.

------------------------------------------------------------------------

## 6.2 Electric Blue

Color secundario de contraste:

``` css
--color-electric-blue: #4827FD;
```

Utilizar para:

-   Destacados puntuales
-   Stickers
-   Bloques gráficos
-   Proyectos
-   Hover alternativo
-   Elementos inesperados dentro de composiciones

El azul debe aparecer con menor frecuencia que el amarillo.

### Regla

El azul aporta **ruptura y sorpresa**.

El amarillo aporta **identidad**.

------------------------------------------------------------------------

# 7. Jerarquía cromática

Orden de prioridad:

``` text
01 — BLACK / DARK
02 — ACID YELLOW
03 — OFF WHITE
04 — ELECTRIC BLUE
05 — GRAYS
```

El amarillo debe ser más frecuente que el azul.

El azul debe utilizarse como contraste y sorpresa, no como segundo color
estructural.

### Evitar

No utilizar simultáneamente amarillo + azul + blanco + gris en cada
componente.

Cada composición debe tener un color dominante y uno o dos colores
secundarios como máximo.

------------------------------------------------------------------------

# 8. Backgrounds oficiales

El proyecto dispone de dos backgrounds gráficos oficiales:

``` text
dark background
light background
```

Estos assets forman parte de la identidad visual.

### Dark sections

La mayoría de las secciones utilizan:

``` text
dark background + light typography
```

### Light sections

Algunas secciones utilizan:

``` text
light background + dark typography
```

Su objetivo es generar contraste visual y evitar que toda la página
tenga el mismo ritmo.

### Importante

El agente NO debe:

-   Generar nuevos backgrounds sin necesidad.
-   Sustituir los backgrounds oficiales por gradientes.
-   Aplicar glassmorphism.
-   Crear fondos abstractos de estilo SaaS.
-   Añadir ruido visual que compita con la textura existente.

------------------------------------------------------------------------

# 9. Tipografía

La tipografía es uno de los elementos principales de identidad.

Se utilizarán **dos familias tipográficas**.

------------------------------------------------------------------------

## 9.1 Display / Headings

### Bebas Neue

``` css
font-family: "Bebas Neue", sans-serif;
```

Uso:

-   H1
-   H2
-   H3
-   Grandes titulares
-   Títulos de sección
-   Números destacados
-   Claims
-   Texto gráfico

Características:

-   Condensada
-   Vertical
-   Impactante
-   Editorial
-   Fácil de combinar con composiciones tipo póster

Los titulares deben tener una presencia muy importante dentro del
layout.

### Ejemplo

``` text
IDEAS
CÓDIGO
Y ALGO DE
CAFÉ
```

Los headings pueden ocupar varias líneas y funcionar como elemento
visual.

------------------------------------------------------------------------

# 10. Tipografía de texto

### Space Mono

``` css
font-family: "Space Mono", monospace;
```

Uso:

-   Body
-   Descripciones
-   Navegación
-   Metadata
-   Tags
-   Tecnologías
-   Fechas
-   Información profesional
-   Microcopy

Space Mono aporta el carácter técnico / developer que contrasta con la
tipografía display.

------------------------------------------------------------------------

# 11. Relación tipográfica

La combinación debe ser:

``` text
BEBAS NEUE
        +
SPACE MONO
```

### Concepto

**Bebas Neue = personalidad**

**Space Mono = código / tecnología**

La combinación debe utilizarse de forma consistente durante toda la web.

No introducir una tercera fuente salvo que exista una necesidad
excepcional y justificada.

------------------------------------------------------------------------

# 12. Escala tipográfica

La escala debe ser deliberadamente grande.

``` css
--font-size-xs: 0.7rem;
--font-size-sm: 0.8rem;
--font-size-md: 1rem;
--font-size-lg: 1.25rem;
--font-size-xl: 1.75rem;
--font-size-2xl: 2.5rem;
--font-size-3xl: 4rem;
--font-size-4xl: 6rem;
--font-size-display: clamp(4rem, 11vw, 11rem);
```

Los valores pueden adaptarse al viewport, pero se debe mantener una
sensación de **tipografía grande y dominante**.

------------------------------------------------------------------------

# 13. Letter spacing

## Display

Los títulos pueden utilizar tracking negativo:

``` css
letter-spacing: -0.02em;
```

En tipografías muy condensadas no exagerar el tracking negativo.

## Mono / Labels

Para labels uppercase:

``` css
letter-spacing: 0.04em;
```

Los pequeños textos técnicos pueden utilizar tracking ligeramente
positivo.

------------------------------------------------------------------------

# 14. Mayúsculas

Los títulos de sección deben utilizar principalmente mayúsculas.

Ejemplo:

``` text
PROYECTOS DESTACADOS
SOBRE MÍ
EXPERIENCIA
CONTACTO
```

Los textos descriptivos permanecen en sentence case.

Las mayúsculas deben utilizarse para crear impacto, no para todo el
contenido.

------------------------------------------------------------------------

# 15. Logo oficial

El proyecto dispone de un **logo oficial de Rubén Carmona**.

El logo es un asset de identidad y debe utilizarse directamente.

No:

-   Redibujar el logo.
-   Sustituirlo por texto.
-   Cambiar sus proporciones.
-   Aplicar filtros arbitrarios.
-   Cambiar sus colores sin una variante definida.

Mantener siempre el aspecto y proporciones originales.

------------------------------------------------------------------------

# 16. Elementos gráficos oficiales

Existen dos elementos gráficos oficiales:

### Corona

Elemento gráfico asociado directamente a la identidad de Rubén.

Color principal:

``` css
--color-acid
```

### Tachón

Elemento gráfico decorativo / editorial.

Color principal:

``` css
--color-acid
```

Ambos assets deben utilizarse como recursos recurrentes de identidad.

No sustituirlos por:

-   Emojis
-   Iconos genéricos
-   SVGs improvisados
-   Dibujos generados mediante CSS
-   Ilustraciones de librerías externas

------------------------------------------------------------------------

# 17. Uso de elementos gráficos

Los elementos pueden:

-   Rotarse ligeramente
-   Escalarse
-   Superponerse
-   Salirse parcialmente del grid
-   Aparecer sobre fotografías
-   Utilizarse como subrayado
-   Utilizarse para enfatizar palabras

Rotaciones recomendadas:

``` css
rotate(-2deg)
rotate(2deg)
rotate(-4deg)
rotate(4deg)
```

Evitar rotaciones excesivas.

La sensación debe ser de **collage editorial controlado**.

------------------------------------------------------------------------

# 18. Fotografía

Las fotografías deben mantener preferentemente:

-   Blanco y negro
-   Alto contraste
-   Textura
-   Grano
-   Recorte agresivo
-   Composición editorial

La fotografía de Rubén debe funcionar como un elemento gráfico, no
necesariamente como un retrato convencional.

Puede:

-   Salirse del grid
-   Superponerse
-   Recortarse
-   Mezclarse con formas
-   Tener elementos gráficos encima

------------------------------------------------------------------------

# 19. Layout

El layout debe estar basado en un grid sólido.

Sobre ese grid se pueden introducir elementos que rompan ligeramente la
estructura.

### Principio

``` text
GRID → ESTRUCTURA
COLLAGE → PERSONALIDAD
```

Se permite:

-   Asimetría
-   Superposición
-   Elementos desplazados
-   Grandes espacios
-   Texto gigante
-   Elementos fuera del grid

No se permite que la composición perjudique:

-   Legibilidad
-   Navegación
-   Responsive
-   Accesibilidad

------------------------------------------------------------------------

# 20. Bordes

Los bordes deben ser visibles y contundentes.

Preferencia:

``` css
border: 1px solid var(--color-text-light);
```

o:

``` css
border: 2px solid var(--color-text-light);
```

En elementos de impacto puede utilizarse el amarillo.

Evitar bordes extremadamente finos y delicados.

------------------------------------------------------------------------

# 21. Border radius

La estética general es cuadrada / editorial.

Preferir:

``` css
border-radius: 0;
```

o valores pequeños:

``` css
border-radius: 2px;
border-radius: 4px;
```

Evitar cards excesivamente redondeadas.

No utilizar `border-radius: 999px` salvo para elementos muy concretos
como badges.

------------------------------------------------------------------------

# 22. Sombras

Las sombras suaves no forman parte de la identidad principal.

Evitar:

``` css
box-shadow: 0 10px 30px rgba(0,0,0,.2);
```

Cuando una sombra tenga función gráfica, utilizar sombras duras:

``` css
box-shadow: 6px 6px 0 var(--color-acid);
```

La sombra debe sentirse como un recurso de diseño editorial.

------------------------------------------------------------------------

# 23. Botones

Los botones deben ser contundentes.

Ejemplo:

``` text
LET'S BUILD
SOMETHING →
```

Características:

-   Tipografía fuerte
-   Alto contraste
-   Bordes visibles
-   Poco o ningún border-radius
-   Mucha presencia

### CTA principal

``` css
background: var(--color-acid);
color: var(--color-text-dark);
```

### Hover

El hover puede:

-   Desplazar el botón
-   Cambiar el color
-   Añadir sombra dura
-   Cambiar ligeramente su escala

Ejemplo:

``` css
transform: translate(-3px, -3px);
box-shadow: 6px 6px 0 var(--color-electric-blue);
```

------------------------------------------------------------------------

# 24. Cards

Evitar la típica card SaaS.

No utilizar sistemáticamente:

``` text
┌──────────────────────┐
│ icon                 │
│ title                │
│ description          │
│ button               │
└──────────────────────┘
```

Los proyectos deben sentirse como **piezas editoriales**.

Utilizar:

-   Imagen dominante
-   Título
-   Descripción breve
-   Tags
-   Flecha
-   Bordes
-   Color
-   Composición variable

------------------------------------------------------------------------

# 25. Tags

Los tags tecnológicos pueden utilizar un tratamiento técnico:

``` text
#ASTRO
#NODE
#POSTGRES
#JAVASCRIPT
```

Preferencia:

-   Monospace
-   Uppercase
-   Tamaño pequeño
-   Bordes
-   Fondo oscuro o claro según la sección

No convertirlos en grandes pills redondeadas.

------------------------------------------------------------------------

# 26. Secciones

Cada sección debe tener una identidad ligeramente diferente, pero
pertenecer al mismo sistema.

### Dark

``` text
Dark background
Light typography
Acid yellow
Electric blue puntual
```

### Light

``` text
Light background
Dark typography
Acid yellow
Electric blue puntual
```

El cambio dark/light debe utilizarse como **herramienta narrativa**.

------------------------------------------------------------------------

# 27. Hero

El Hero debe ser el punto de máxima intensidad visual.

Debe combinar:

-   Logo
-   Navegación
-   Claim
-   Tipografía gigante
-   Fotografía
-   Corona
-   Tachón
-   Amarillo
-   Textura
-   Composición editorial

El Hero no debe parecer una típica landing de desarrollador.

Debe parecer la portada de una revista / póster.

------------------------------------------------------------------------

# 28. Proyectos

Los proyectos deben ser uno de los elementos más visuales del portfolio.

Cada proyecto debe mostrar:

1.  Imagen
2.  Nombre
3.  Tipo de proyecto
4.  Descripción breve
5.  Tecnologías
6.  Acción / enlace

El color de cada proyecto puede variar ligeramente mediante amarillo o
azul, pero debe seguir siendo reconocible como parte del sistema.

------------------------------------------------------------------------

# 29. Sobre mí

La sección "Sobre mí" utiliza preferentemente fondo claro para generar
contraste.

Tratamiento:

``` text
LIGHT BACKGROUND
+
DARK TYPOGRAPHY
+
ACID YELLOW
+
PHOTOGRAPHY
+
HAND-DRAWN ELEMENTS
```

Debe sentirse más editorial y humana que técnica.

------------------------------------------------------------------------

# 30. Experiencia

La experiencia debe evitar parecer un CV tradicional.

Utilizar:

-   Timeline
-   Fechas
-   Grandes números
-   Tipografía display
-   Separadores
-   Elementos gráficos

La información debe poder escanearse rápidamente.

------------------------------------------------------------------------

# 31. Contacto

El contacto vuelve al universo dark.

Debe ser una sección visualmente potente.

El mensaje puede utilizar tipografía display de gran tamaño.

Ejemplo conceptual:

``` text
GOOD PEOPLE
BUILD
GREAT
THINGS
```

La información de contacto debe ser clara y accesible.

------------------------------------------------------------------------

# 32. Animaciones

Las animaciones deben ser rápidas, físicas y ligeramente impredecibles.

Preferir:

-   `translate`
-   `rotate`
-   `scale`
-   `clip-path`
-   Reveals
-   Marquee
-   Hover interactions

Evitar animaciones lentas y excesivamente elegantes.

Duración recomendada:

``` css
180ms — 300ms
```

------------------------------------------------------------------------

# 33. Marquee

Puede utilizarse texto en movimiento como recurso gráfico.

Ejemplo:

``` text
WEB DEVELOPMENT ✦ DESIGN ✦ IDEAS ✦ CODE ✦ COFFEE ✦
```

Debe ser decorativo.

Nunca utilizar un marquee para información esencial.

------------------------------------------------------------------------

# 34. Accesibilidad

La estética no debe comprometer la accesibilidad.

Obligatorio:

-   Contraste suficiente
-   Focus states visibles
-   HTML semántico
-   Navegación por teclado
-   Alt text en imágenes relevantes
-   Targets táctiles adecuados
-   `prefers-reduced-motion`

Las animaciones deben poder reducirse cuando el usuario tenga activada
la preferencia correspondiente.

------------------------------------------------------------------------

# 35. Responsive

El diseño móvil debe ser una adaptación real de la composición.

No limitarse a reducir tamaños.

En mobile:

-   Simplificar composiciones
-   Reordenar elementos
-   Reducir decoración cuando interfiera
-   Mantener titulares grandes
-   Evitar overflow horizontal
-   Mantener el contraste dark/light
-   Mantener amarillo y azul como elementos de identidad

La personalidad debe sobrevivir al cambio de viewport.

------------------------------------------------------------------------

# 36. Reglas para el agente IA

Estas reglas son prioritarias.

## DO

-   Respetar la paleta oficial.
-   Utilizar exclusivamente las dos familias tipográficas definidas.
-   Utilizar los backgrounds oficiales.
-   Utilizar el logo oficial.
-   Utilizar corona y tachón oficiales.
-   Mantener el amarillo como color de identidad.
-   Utilizar azul como contraste puntual.
-   Mantener la web predominantemente dark.
-   Utilizar las secciones light para contraste.
-   Crear composiciones editoriales.
-   Utilizar la tipografía como elemento visual.
-   Mantener una estructura técnica limpia.
-   Priorizar accesibilidad y responsive.

## DON'T

-   Añadir colores arbitrarios.
-   Añadir nuevas fuentes.
-   Convertir el diseño en SaaS.
-   Usar glassmorphism.
-   Abusar de gradientes.
-   Utilizar cards genéricas.
-   Redondear todos los componentes.
-   Usar sombras suaves como recurso dominante.
-   Sustituir los assets oficiales.
-   Generar nuevos logos.
-   Añadir iconografía decorativa innecesaria.
-   Sobrecargar cada sección con elementos freak.
-   Sacrificar legibilidad por estética.

------------------------------------------------------------------------

# 37. Regla de intensidad

No todos los elementos deben llamar la atención.

La página debe tener una jerarquía clara:

``` text
FOCAL POINT
    ↓
PRIMARY ELEMENT
    ↓
SECONDARY ELEMENTS
    ↓
DETAILS
```

Si todo es llamativo, nada es llamativo.

El diseño freak debe estar **controlado mediante jerarquía visual**.

------------------------------------------------------------------------

# 38. Design tokens

Referencia central para implementación:

``` css
:root {
  /* Backgrounds */
  --color-bg-dark: #090909;
  --color-surface-dark: #111111;
  --color-surface-dark-2: #181818;
  --color-bg-light: #E2E0DC;

  /* Text */
  --color-text-light: #F2F0EA;
  --color-text-light-muted: #B8B6B0;
  --color-white: #FFFFFF;

  --color-text-dark: #111111;
  --color-text-dark-muted: #454545;

  /* Accent */
  --color-acid: #D7F821;
  --color-electric-blue: #4827FD;

  /* Typography */
  --font-display: "Bebas Neue", sans-serif;
  --font-body: "Space Mono", monospace;

  /* Radius */
  --radius-sm: 2px;
  --radius-md: 4px;
  --radius-none: 0;

  /* Motion */
  --transition-fast: 180ms;
  --transition-normal: 300ms;
}
```

------------------------------------------------------------------------

# 39. Decisión visual definitiva

Ante cualquier decisión de diseño, priorizar en este orden:

1.  **Identidad**
2.  **Legibilidad**
3.  **Jerarquía**
4.  **Usabilidad**
5.  **Accesibilidad**
6.  **Experimentación**

La web debe ser atrevida, pero nunca parecer accidental.

> **MAKE IT LOUD.**
>
> **KEEP IT SMART.**
>
> **MAKE IT RUBÉN.**
