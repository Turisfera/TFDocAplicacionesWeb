# Capítulo V: Product Implementation, Validation & Deployment
## 5.1. Software Configuration Management
### 5.1.1 Configuración del Entorno de Desarrollo de Software

**Requirements Management**  
1. <img src="./img/icons/trello.svg" alt="Trello" width="20" style="vertical-align:middle; margin-right:8px;"> **[Trello](https://trello.com/)**: Tablero Kanban web para planificar y hacer seguimiento de historias de usuario y tareas por sprint. Permite asignar responsables, fechas de entrega y checklists para cada tarjeta.  
2. <img src="./img/icons/discord.svg" alt="Discord" width="20" style="vertical-align:middle; margin-right:8px;"> **[Discord](https://discord.com/)**: Plataforma de chat y voz VoIP con canales temáticos, notificaciones y bots. Se utiliza como canal principal de comunicación en tiempo real, para compartir pantallazos de código, coordinar reuniones flash y notificar despliegues.  
3. <img src="./img/icons/vertabelo.svg" alt="Vertabelo" width="20" style="vertical-align:middle; margin-right:8px;"> **[Vertabelo](https://vertabelo.com/)**: Herramienta SaaS para diseño y modelado de bases de datos relacionales. Facilita la creación de diagramas ER, versionado de esquemas y generación de scripts SQL.

**Product UX/UI Design**  
1. <img src="./img/icons/figma.svg" alt="Figma" width="20" style="vertical-align:middle; margin-right:8px;"> **[Figma](https://www.figma.com/)**: Editor de interfaces colaborativo en la nube. Soporta diseño vectorial, prototipado interactivo y comentarios en tiempo real. Usado para iterar wireframes y mock-ups de Desktop y Mobile Web.  
2. <img src="./img/icons/lucidchart.svg" alt="Lucidchart" width="20" style="vertical-align:middle; margin-right:8px;"> **[Lucidchart](https://www.lucidchart.com/)**: Aplicación web para diagramas de flujo, wireflows y diagramas de clases. Permite conectar objetos con líneas inteligentes y exportar en múltiples formatos.  
3. <img src="./img/icons/uxpressia.svg" alt="Uxpressia" width="20" style="vertical-align:middle; margin-right:8px;"> **[Uxpressia](https://uxpressia.com/)**: Plataforma online para mapas de empatía, Customer Journey y escenarios As-Is / To-Be. Estandariza hallazgos de entrevistas y visualiza puntos de dolor.  
4. <img src="./img/icons/visual-paradigm.svg" alt="Visual Paradigm" width="20" style="vertical-align:middle; margin-right:8px;"> **[Visual Paradigm](https://www.visual-paradigm.com/)**: Suite de modelado UML y C4 para diagramas de contenedores, componentes y despliegue. Genera documentación técnica que facilita la comunicación entre analistas y desarrolladores.

**Software Development**  
1. <img src="./img/icons/webstorm.svg" alt="WebStorm" width="20" style="vertical-align:middle; margin-right:8px;"> **[WebStorm](https://www.jetbrains.com/webstorm/)**: IDE de JetBrains con autocompletado inteligente, refactorización segura, depurador integrado y plugins de linters/formateadores.  
2. <img src="./img/icons/html5.svg" alt="HTML5" width="20" style="vertical-align:middle; margin-right:8px;"> **HTML5**: Lenguaje de marcado semántico para estructurar contenido y mejorar accesibilidad (etiquetas `<header>`, `<nav>`, `<main>`, `<footer>`).  
3. <img src="./img/icons/css.svg" alt="CSS3" width="20" style="vertical-align:middle; margin-right:8px;"> **CSS3**: Hojas de estilo en cascada para layouts, media queries y variables CSS, siguiendo la convención BEM ligero.  
4. <img src="./img/icons/javascript.svg" alt="JavaScript" width="20" style="vertical-align:middle; margin-right:8px;"> **[JavaScript](https://developer.mozilla.org/docs/Web/JavaScript)**: Lenguaje de scripting para manipular el DOM, manejar eventos y validar formularios en `script.js` (por ejemplo, validación de campos antes de enviar).

**Software Deployment**  
1. <img src="./img/icons/git.svg" alt="Git" width="20" style="vertical-align:middle; margin-right:8px;"> **[Git](https://git-scm.com/)**: Sistema de control de versiones distribuido. Utilizamos GitFlow para crear ramas `feature/`, `release/` y `hotfix/`, facilitar merges y revertir cambios si es necesario.  
2. <img src="./img/icons/github-pages.svg" alt="GitHub Pages" width="20" style="vertical-align:middle; margin-right:8px;"> **[GitHub Pages](https://pages.github.com/)**: Servicio de hosting estático gratuito. Configuramos la carpeta `/docs` en `main` para publicar automáticamente la landing page tras cada push.

**Software Documentation and Project Management**  
1. <img src="./img/icons/github.svg" alt="GitHub" width="20" style="vertical-align:middle; margin-right:8px;"> **[GitHub](https://github.com/)** (Wiki / `README.md`): Documentación técnica centralizada con guías de estilo, convenciones de commits y manuales de despliegue.  
2. <img src="./img/icons/google-drive.svg" alt="Google Drive" width="20" style="vertical-align:middle; margin-right:8px;"> **[Google Drive](https://drive.google.com/)** /**[Google Docs](https://docs.google.com/)**: Repositorio de requisitos, actas de reunión y borradores de informes con control de versiones de documento y comentarios colaborativos.  


### 5.1.2 Source Code Management

Para garantizar trazabilidad y control de versiones claros, adoptamos el modelo **GitFlow** de Vincent Driessen (https://nvie.com/posts/a-successful-git-branching-model/):

**Branching Model (GitFlow)**
1. **main**: contiene siempre el código listo para producción.
2. **develop**: integración continua de todas las _features_ terminadas; funciona como base para nuevos desarrollos.
3. **feature/<name>**: ramas derivadas de `develop` para cada funcionalidad.
```bash
git checkout develop
git checkout -b feature/user-auth
```
Al completarla, abrimos un Pull Request hacia `develop`.

4. **release/vMAJOR.MINOR.PATCH**: se crea desde `develop` para preparar una nueva versión; en ella corregimos bugs menores, actualizamos documentación y realizamos el bump de versión.
5. **hotfix/vMAJOR.MINOR.PATCH**: correcciones urgentes derivadas de `main`; tras aplicarlas, se fusiona tanto a `main` como a `develop`.

**Versionado Semántico & Conventional Commits**
- **Semantic Versioning** (`MAJOR.MINOR.PATCH`):
  - **MAJOR**: cambios incompatibles con versiones anteriores.
  - **MINOR**: añadidos de funcionalidades sin romper API.
  - **PATCH**: correcciones de bugs y mejoras menores.
- **Conventional Commits**: mensajes de commit con estructura:
  ```text
  docs(report): actualizar sección 5.1.2 de Source Code Management
  feat(landing-page): centrar iconos sociales y mejorar CSS de formulario
  fix(form-validation): impedir envío si hay errores de validación
  chore(assets): agregar diagramas UML de C4 en carpeta img
Esto facilita la generación de _changelogs_ automáticos y una lectura rápida del historial.

**Etiquetado de Releases**
Al finalizar el testing de una _release_ branch, generamos la etiqueta con:
```bash
git tag -a v1.0.0 -m "release: v1.0.0"
git push origin v1.0.0
```

**Repositorios & Enlaces**
- **Landing Page**: https://github.com/Turisfera/Landing-Page
- **Repository**: https://github.com/Turisfera/TFDocAplicacionesWeb

Cada repositorio sigue el mismo flujo GitFlow y cumple con las convenciones de naming y commits descritas.

### 5.1.3 Source Code Style Guide & Conventions

Para garantizar código limpio, consistente y mantenible, adoptamos las siguientes convenciones (todas en inglés):

**HTML**  
- **Semantics first**: usar etiquetas `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>` según el propósito del contenido.  
- **Lowercase & closing tags**: nombres de elementos y atributos siempre en minúsculas, cerrar explícitamente todas las etiquetas (incluyendo `<img />`, `<input />`).  
- **Attribute order**: primero `id`, luego `class`, después otros atributos (`name`, `src`, `alt`, `aria-*`).  
- **Indentation**: 2 spaces por nivel de anidamiento.  
- **Comments**: `<!-- Comment -->` en una línea o multilínea, sin abreviaturas.

**CSS**  
- **Naming**: kebab-case para clases y selectores (`.btn-primary`, `.card-header`).  
- **BEM‐inspired**: bloques, elementos y modificadores (`.block`, `.block__element`, `.block--modifier`).  
- **Property order**:  
  1. Positioning (`position`, `top`, `left`, `z-index`)  
  2. Box Model (`display`, `margin`, `padding`, `width`, `height`)  
  3. Typography (`font`, `line-height`, `color`)  
  4. Visual (`background`, `border`, `box-shadow`)  
  5. States and interactions (`:hover`, `:focus`, `:active`)  
- **Formatting**: 2 spaces por nivel, un selector por línea, llave de apertura en la misma línea, cierre en nueva línea.  
- **Comments**: `/* Section name */` para separar bloques lógicos.

**JavaScript**  
- **Naming**:  
  - `camelCase` para variables y funciones (`myFunction`, `userName`).  
  - `PascalCase` para clases y constructores (`UserService`, `DataModel`).  
- **Syntax**:  
  - Siempre `;` al final de declaraciones.  
  - Comillas simples para strings (`'hello'`), salvo cuando el contenido requiere comillas dobles.  
- **Indentation**: 2 spaces, no tabs.  
- **Modern ES**: usar `const`/`let` en lugar de `var`, arrow functions para callbacks.  
- **Modules**: `import { something } from './module.js';`  
- **Comments & JSDoc**:  
  ```js
  /**
   * Fetch user data by ID.
   * @param {string} id
   * @returns {Promise<User>}
   */
  export async function fetchUser(id) { … }

  
### 5.1.4 Software Deployment Configuration

Para el despliegue de la **Landing Page** en GitHub Pages, hemos seguido estos pasos:

1. **Repositorio**  
   - URL: https://github.com/Turisfera/Landing-Page  
   - Rama principal: `main`  

2. **Estructura de archivos**  
   - `index.html` en la raíz  
   - Carpetas:  
     - `styles/` (CSS)  
     - `scripts/` (JavaScript)  
     - `img/` (imágenes y assets)  

3. **Configuración de GitHub Pages**  
   - En el repositorio, ir a **Settings → Pages**  
   - Seleccionar fuente de despliegue:  
     - **Branch**: `main`  
     - **Folder**: `/ (root)`  
   - Guardar los cambios  

4. **Publicación automática**  
   Cada vez que hacemos `git push origin main`, GitHub reconstruye y publica la página sin intervención manual.

5. **URL pública**  
   https://turisfera.github.io/Landing-Page/

Con esta configuración, cualquier actualización en `main`—ya sea HTML, CSS, JS o imágenes—se refleja automáticamente en el sitio publicado.




## 5.2. Landing Page, Services & Applications Implementation
### 5.2.1. Sprint 1
#### 5.2.1.1. Sprint Planning 1
<table style="border-collapse: collapse; width: 100%;">
<tbody>
<tr><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;"><strong>Sprint #</strong></td><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;"><strong>Sprint 1</strong></td></tr>
<tr><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;" colspan="2"><strong>Sprint Planning Backlog</strong></td></tr>
<tr><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;">Date</td><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;">19/04/2025</td></tr>
<tr><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;">Time</td><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;">3 horas</td></tr>
<tr><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;">Location o Platform</td><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;">Discord</td></tr>
<tr><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;">Prepared By</td><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;">Marcia Victoria Melgarejo Gomez-U20231C505</td></tr>
<tr><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;">Attendees</td><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;">María Patricia Hernández Uchuya-U202311258</br> Britney Delhy Qqueso Rodriguez-U20211G671</br> Rodrigo Alaya Cabrera-U202219481</br> Ariadna Geraldine Poma Muñoz-U20221D328</br> Jorge Enrique Guevara Tejada-U202316057</br> Raúl Adrian Medina Cruzado-U202210938</td></tr>
<tr><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;" colspan="2"><strong>Sprint Goal &amp; User Stories</strong></td></tr>
<tr><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;">Sprint 1 Goal</td><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;">Diseñp y desarrollo del landing page</td></tr>
<tr><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;">Sprint 1 Velocity</td><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;">15<strong></strong></td></tr>
<tr><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;">Sum of Story Points</td><td style="border:1pt solid #000000;padding:5pt;vertical-align:top;">15<strong></strong></td></tr>
</tbody>
</table>

#### 5.2.1.2. Aspect Leaders and Collaborators
#### 5.2.1.3. Sprint Backlog 1
|**Sprint #**|Sprint 1|||||||
|User Story|Work-Itrm/Task|||||||
|**Id**|**Title**|**Id**|**Title**|**Description**|**Estimation** (Hours)|**Assigned To**|**Status** (To-do/In Process/ToReview/Done)|

#### 5.2.1.4. Development Evidence for Sprint Review
#### 5.2.1.5. Execution Evidence for Sprint Review
#### 5.2.1.6. Services Documentation Evidence for Sprint Review
#### 5.2.1.7. Software Deployment Evidence for Sprint Review
#### 5.2.1.8. Team Collaboration Insights during Sprint

