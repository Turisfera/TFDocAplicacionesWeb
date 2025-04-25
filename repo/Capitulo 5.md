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
En el primer sprint se implementó y desplegó la Landing Page.
#### 5.2.1.1 Sprint Planning 1

El Sprint Planning 1 es la reunión inicial de la iteración donde el equipo define la meta (Sprint Goal), revisa el Sprint anterior y selecciona los User Stories que abordará en este Sprint.

| **Sprint #**                        | **Sprint 1**                                                                                                                                          |
| ----------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Sprint Planning Background**      |                                                                                                                                                       |
| **Date**                            | 2025-04-19                                                                                                                                            |
| **Time**                            | 07:00 PM – 10:00 PM                                                                                                                                    |
| **Location / Platform**             | Discord                                                                                                                                               |
| **Prepared by**                     | Marcia Victoria Melgarejo Gomez – U20231C505                                                                                                          |
| **Attendees (to planning meeting)** | María Patricia Hernández Uchuya – U202311258<br>Britney Delhy Q. Rodríguez – U20211G671<br>Rodrigo Alaya Cabrera – U202219481<br>Ariadna G. Poma Muñoz – U20221D328<br>Jorge E. Guevara Tejada – U202316057<br>Raúl A. Medina Cruzado – U202210938 |
| **Sprint 0 Review Summary**         | Definición del Product Backlog inicial, creación de wireframes y prototipo de landing page en Figma, y feedback temprano de stakeholders.             |
| **Sprint 0 Retrospective Summary**  | Consolidación de roles (diseño vs. desarrollo), estandarización de estilos CSS y establecimiento de canales de comunicación (Discord, WhatsApp, GitHub). |
| **Sprint 1 Goal**                   | Nos centramos en una página de destino totalmente adaptable. Creemos que ofrece una primera impresión clara y una experiencia de registro sencilla para los nuevos usuarios. Esto se confirmará cuando las pruebas de control de calidad informen un 100 % de éxito en el registro de tickets en entornos de prueba.. |
| **Sprint 1 Velocity**               | 15                                                                                                                                                    |
| **Sum of Story Points**             | 15                                                                                                                                                    |
 
Los User Stories planificados (US01, US02, US03, US04, US06, US07, US15 y US10) y sus criterios de aceptación están detallados en la sección User Stories.

#### 5.2.1.2 Aspect Leaders and Collaborators

En el Sprint 1 se definieron los siguientes aspectos clave para la implementación del Landing Page:

1. **UI/UX Design**  
2. **Maquetación HTML/CSS**  
3. **Desarrollo JavaScript**  
4. **Documentación de Servicios**  
5. **Despliegue**  

A continuación la matriz de Liderazgo y Colaboración (LACX), donde “L” indica el líder de cada aspecto y “C” a sus colaboradores:

| **Team Member (Last Name, First Name)** | **GitHub Username** | **UI/UX Design** | **Maquetación HTML/CSS** | **Desarrollo JavaScript** | **Documentación de Servicios** | **Despliegue** |
|-----------------------------------------|---------------------|:----------------:|:------------------------:|:-------------------------:|:------------------------------:|:--------------:|
| Hernández Uchuya, María Patricia        | Bal2220             | C                | C                        | C                         | C                              | C              |
| Qqueso Rodríguez, Britney Delhy         | Brit2801            | C                | L                        | C                         | C                              | C              |
| Alaya Cabrera, Rodrigo                  | ALAYA1803           | C                | C                        | L                         | C                              | C              |
| Poma Muñoz, Ariadna Geraldine           | InAsui              | C                | C                        | C                         | L                              | C              |
| Guevara Tejada, Jorge Enrique           | Jorgito170          | C                | C                        | C                         | L                              | C              |
| Medina Cruzado, Raúl Adrián             | Necxuz18            | C                | C                        | C                         | C                              | L              |
| Melgarejo Gomez, Marcia Victoria        | Mevi1217            | L                | C                        | C                         | C                              | C              |

#### 5.2.1.3. Sprint Backlog 1
<table style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <td style="border:1pt solid #000000;padding:5pt;vertical-align:top;"><strong>N°</strong></td>
      <td style="border:1pt solid #000000;padding:5pt;vertical-align:top;"><strong>User Story ID</strong></td>
      <td style="border:1pt solid #000000;padding:5pt;vertical-align:top;"><strong>Título</strong></td>
      <td style="border:1pt solid #000000;padding:5pt;vertical-align:top;"><strong>Story Points</strong></td>
      <td style="border:1pt solid #000000;padding:5pt;vertical-align:top;"><strong>Prioridad</strong></td>
      <td style="border:1pt solid #000000;padding:5pt;vertical-align:top;"><strong>Estado</strong></td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="border:1pt solid #000000;padding:5pt;">1</td>
      <td style="border:1pt solid #000000;padding:5pt;">US01</td>
      <td style="border:1pt solid #000000;padding:5pt;">Registro de usuario</td>
      <td style="border:1pt solid #000000;padding:5pt;">8</td>
      <td style="border:1pt solid #000000;padding:5pt;">Alta</td>
      <td style="border:1pt solid #000000;padding:5pt;">Por hacer</td>
    </tr>
    <tr>
      <td style="border:1pt solid #000000;padding:5pt;">2</td>
      <td style="border:1pt solid #000000;padding:5pt;">US02</td>
      <td style="border:1pt solid #000000;padding:5pt;">Validación de datos de registro</td>
      <td style="border:1pt solid #000000;padding:5pt;">5</td>
      <td style="border:1pt solid #000000;padding:5pt;">Alta</td>
      <td style="border:1pt solid #000000;padding:5pt;">Por hacer</td>
    </tr>
    <tr>
      <td style="border:1pt solid #000000;padding:5pt;">3</td>
      <td style="border:1pt solid #000000;padding:5pt;">US03</td>
      <td style="border:1pt solid #000000;padding:5pt;">Confirmación de contraseña</td>
      <td style="border:1pt solid #000000;padding:5pt;">3</td>
      <td style="border:1pt solid #000000;padding:5pt;">Alta</td>
      <td style="border:1pt solid #000000;padding:5pt;">Por hacer</td>
    </tr>
    <tr>
      <td style="border:1pt solid #000000;padding:5pt;">4</td>
      <td style="border:1pt solid #000000;padding:5pt;">US04</td>
      <td style="border:1pt solid #000000;padding:5pt;">Mensaje de bienvenida</td>
      <td style="border:1pt solid #000000;padding:5pt;">8</td>
      <td style="border:1pt solid #000000;padding:5pt;">Media</td>
      <td style="border:1pt solid #000000;padding:5pt;">Por hacer</td>
    </tr>
    <tr>
      <td style="border:1pt solid #000000;padding:5pt;">5</td>
      <td style="border:1pt solid #000000;padding:5pt;">US06</td>
      <td style="border:1pt solid #000000;padding:5pt;">Confirmación por correo electrónico</td>
      <td style="border:1pt solid #000000;padding:5pt;">8</td>
      <td style="border:1pt solid #000000;padding:5pt;">Alta</td>
      <td style="border:1pt solid #000000;padding:5pt;">Por hacer</td>
    </tr>
    <tr>
      <td style="border:1pt solid #000000;padding:5pt;">6</td>
      <td style="border:1pt solid #000000;padding:5pt;">US07</td>
      <td style="border:1pt solid #000000;padding:5pt;">Búsqueda de destinos turísticos</td>
      <td style="border:1pt solid #000000;padding:5pt;">5</td>
      <td style="border:1pt solid #000000;padding:5pt;">Alta</td>
      <td style="border:1pt solid #000000;padding:5pt;">Por hacer</td>
    </tr>
    <tr>
      <td style="border:1pt solid #000000;padding:5pt;">7</td>
      <td style="border:1pt solid #000000;padding:5pt;">US15</td>
      <td style="border:1pt solid #000000;padding:5pt;">Buscar destinos turísticos por nombre</td>
      <td style="border:1pt solid #000000;padding:5pt;">3</td>
      <td style="border:1pt solid #000000;padding:5pt;">Media</td>
      <td style="border:1pt solid #000000;padding:5pt;">Por hacer</td>
    </tr>
    <tr>
      <td style="border:1pt solid #000000;padding:5pt;">8</td>
      <td style="border:1pt solid #000000;padding:5pt;">US10</td>
      <td style="border:1pt solid #000000;padding:5pt;">Vista previa de destinos</td>
      <td style="border:1pt solid #000000;padding:5pt;">5</td>
      <td style="border:1pt solid #000000;padding:5pt;">Media</td>
      <td style="border:1pt solid #000000;padding:5pt;">Por hacer</td>
    </tr>
  </tbody>
</table>

#### 5.2.1.4. Development Evidence for Sprint Review

Durante el Sprint 1, se desarrolló la **landing page** del sistema.  
Las principales actividades incluyeron:
- Diseño del prototipo en Figma (adjuntar enlace si hay uno)
- Maquetación HTML y CSS del landing
- Estructura básica con estilos iniciales responsivos
- Uso de componentes reutilizables en JavaScript (si aplica)
📂 **Commits relevantes:**
- `feat: diseño base del landing`
- `style: mejoras visuales en el home`
- `fix: corrección de márgenes y fuentes`
📁 **Ubicación en el repositorio:**
- `/src/pages/Landing.html`
- `/src/assets/styles/landing.css`

#### 5.2.1.5. Execution Evidence for Sprint Review

La ejecución se validó de la siguiente forma:
- Visualización del landing en distintos navegadores (Chrome, Firefox, Edge)
- Pruebas básicas de carga y visual responsiva
- Validación de código HTML y CSS, [TripMach](https://turisfera.github.io/Landing-Page/)

🧪 **Resultado:** La página carga correctamente, presenta un diseño alineado al prototipo y es navegable desde escritorio y móvil.

#### 5.2.1.6. Services Documentation Evidence for Sprint Review

En este primer sprint se documentaron los siguientes aspectos:
- Estructura base de archivos del proyecto (README)
- Documentación de los estilos CSS utilizados
- Guía para colaborar en la maquetación

📄 **Ubicación de la documentación:**
- `docs/estilos.md`
- `README.md` → sección “Instalación y visualización del landing”

#### 5.2.1.7. Software Deployment Evidence for Sprint Review


#### 5.2.1.8. Team Collaboration Insights during Sprint

Durante este sprint, el equipo mantuvo una colaboración efectiva a través de:
- Reuniones virtuales semanales por Discord
- Uso de GitHub Projects para tareas (tablero Kanban)
- Comunicación constante por grupo de WhatsApp
- Roles definidos: diseño, maquetación, revisión

🗣️ **Observaciones del trabajo en equipo:**
- Buena participación y cumplimiento de tareas asignadas
- Se dio apoyo mutuo ante dudas técnicas
- Todos los miembros participaron activamente en la revisión del landing page
