# Capítulo 4: Product Design
## 4.1. Style Guidelines
Una Style Guidelines es un conjunto de lineamientos y criterios que establecen la forma en que deben redactarse, diseñarse o presentar documentos, contenido web, software u otros tipos de trabajos creativos. A continuación, se describen las especificaciones de los parámetros aplicados en la estructura del proyecto.

### 4.1.1. General Style Guidelines
__Branding:__
Para la creación del logo de nuestro producto TripMatch, se ha optado por un diseño representativo y amigable que transmite los valores de aventura, autenticidad y conexión con la naturaleza. El logotipo está compuesto por una tipografía redondeada y moderna, acompañada de un ícono que representa una montaña nevada dentro de un círculo, evocando destinos naturales, seguridad y dirección. Los colores utilizados son armónicos y cálidos, lo que refuerza la idea de un turismo responsable y accesible.

![logotipo TripMatch](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/cfaee8914fcfa6c0e9e9f3775cae670e8c539e20/repo/img/logo-TripMatch.png)

__Typography:__
Para la tipografía de TripMatch, se ha seleccionado una fuente moderna, clara y legible, ideal para dispositivos móviles y plataformas digitales. La tipografía principal es Poppins, una fuente amigable y versátil que refuerza el carácter accesible y dinámico de la plataforma. Para títulos y encabezados se puede emplear una versión más gruesa de la misma fuente, garantizando jerarquía visual sin perder coherencia estética.
A continuación, se presentan la tipografía seleccionadas para TripMatch:

![tipography TripMatch](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/cfaee8914fcfa6c0e9e9f3775cae670e8c539e20/repo/img/tipografia-poppins.png)

__Colors:__
La paleta de colores de TripMatch se compone de tonos que evocan calma, naturaleza y aventura. Los colores seleccionados son vibrantes pero equilibrados, lo cual permite captar la atención del usuario sin saturar visualmente la interfaz. A continuación, se presentan los colores seleccionados para TripMatch:

![colors TripMatch]([img/colors-TripMatch.png](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/cfaee8914fcfa6c0e9e9f3775cae670e8c539e20/repo/img/colors-TripMatch.png))

__Spacing:__
El espaciado es un elemento clave en el diseño de TripMatch, ya que permite mantener una interfaz ordenada, limpia y fácil de navegar. Se ha utilizado un espaciado generoso y coherente entre elementos, lo cual mejora la legibilidad y crea una sensación de equilibrio visual. El uso uniforme del espacio contribuye a una experiencia de usuario fluida y cómoda, tanto en dispositivos móviles como en escritorio.

![spacing TripMatch](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/cfaee8914fcfa6c0e9e9f3775cae670e8c539e20/repo/img/spacing-TripMatch.png)

### 4.1.2. Web Style Guidelines
La interfaz web de TripMatch está diseñada con un estilo moderno, limpio y totalmente adaptable a distintos dispositivos, asegurando una navegación fluida tanto en móviles como en pantallas de escritorio. Se emplean paletas de colores inspiradas en la naturaleza y la aventura, tipografías claras como Poppins, y componentes visuales amigables como botones redondeados e íconos intuitivos.

Además, se prioriza la experiencia del usuario mediante interacciones suaves, menús simplificados, tarjetas informativas y animaciones sutiles. Todo el diseño responde a criterios de accesibilidad, garantizando legibilidad, contraste adecuado y compatibilidad con lectores de pantalla.


## 4.2. Information Architecture
La arquitectura de información de Turisnap está diseñada para optimizar la experiencia de navegación de dos tipos principales de usuarios: turistas y anfitriones. La plataforma permite a los turistas descubrir experiencias personalizadas, planificar itinerarios y conectar con guías locales o grupos de viaje. A su vez, los anfitriones pueden registrar y ofrecer actividades o tours. La estructura de la información facilita la exploración del contenido, mejora la accesibilidad a las funciones principales y permite una experiencia fluida e intuitiva.

### 4.2.1. Organization Systems 
Turisnap aplica distintos tipos de organización según la naturaleza de la información y la interacción esperada de cada tipo de usuario:

**Organización jerárquica visual:** <br/>
Para una navegación intuitiva, tanto turistas como agencias cuentan con accesos laterales clave en la pantalla principal. Los turistas disponen de "Inicio", "Favoritos", "Itinerarios" y "Buscar", mientras que las agencias acceden a "Inicio", "Gestión de experiencias", "Reservas", "Consultas" y "Perfil de agencia".<br/>

**Organización secuencial:** <br/>
En la planificación del itinerario personalizado para turistas, la secuencia comienza con la elección del destino, seguida por la selección de fechas, intereses y tipo de experiencia, culminando con la confirmación del itinerario. De manera similar, el registro de una nueva experiencia por parte de las agencias sigue este orden: selección de la experiencia, llenado de los campos requeridos (ubicación, horarios, etc.) y, finalmente, se guarda la informacion. <br/>

**Organización matricial:** <br/>
En la sección de resultados o búsqueda de experiencias, los usuarios refinan su búsqueda mediante filtros combinables por destino, día, presupuesto y tipo de experiencia. Los resultados se actualizan dinámicamente en función de las selecciones aplicadas. <br/>

**Sistemas de categorización:**

- **Por tópicos:** actividades, anfitriones, turistas, destinos, experiencias recomendadas, favoritos, historial de viajes.

- **Cronológica:** ordenamiento de experiencias según la fecha de publicación o según las fechas de viaje elegidas.

- **Alfabética:** búsqueda por tipo de experiencia, destino, o nombre de la agencia.

- **Por audiencia:** se presentan interfaces diferenciadas para turistas (busqueda y planificación de itinerarios) y agencias (gestión de experiencias ofrecidas y reservas).

### 4.2.2. Labeling Systems
Para garantizar una experiencia intuitiva y sin confusiones, las etiquetas empleadas en TripMatch han sido diseñadas con base en principios de simplicidad, claridad y consistencia.

**Etiquetas para la navegación principal (menú lateral):**
* **Inicio:** Página principal con acceso a destinos sugeridos y novedades.
* **Busqueda:** Sección para descubrir nuevos lugares mediante filtros o búsqueda.
* **Itinerario:** Espacio donde el usuario puede planificar, visualizar y editar sus viajes.
* **Perfil:** Acceso a la información personal y configuraciones.

**Etiquetas para acciones:**
* **Buscar:** Entrada para realizar búsquedas de destinos o usuarios.
* **Agregar al itinerario:** Acción rápida para incluir un destino en un viaje.
* **Editar / Eliminar:** Gestión de elementos guardados por el usuario.
* **Guardar cambios:** Confirmación de edición o creación de itinerario.

**Etiquetas asociativas para categorías:**
* **Populares, Culturales, Naturaleza, Aventura, Relax:** Categorías que agrupan destinos según intereses.
* **Hoy, Próximo destino, Favoritos:** Agrupaciones cronológicas y personalizadas que facilitan el acceso a información relevante.

### 4.2.3. SEO Tags and Meta Tags 
En TripMatch, el uso de etiquetas SEO y metaetiquetas se ha diseñado con el objetivo de mejorar la visibilidad de la plataforma en motores de búsqueda y garantizar una representación clara, concisa y coherente de la información. Se prioriza la simplicidad en la redacción de etiquetas, asegurando que los términos utilizados reflejen con precisión los intereses de los usuarios y las categorías de contenido disponibles. <br/>

**Landing Page:**
- **Title:** TripMatch | Donde viajar se combina con la facilidad digital con TripMatch.
- **Meta Description:** Plataforma para descubrir experiencias, crear itinerarios a medida y conectar con guías locales.
- **Meta Keywords:** About us, befefits, how does it work, frequently asked questions, contact.
- **Meta Author:** Turisnap 

**Aplicación Web:**
- **Title:** TripMatch
- **Meta Description:** Crea y personaliza itinerarios, descubre actividades y vive nuevas experiencias en tus destinos favoritos.
- **Meta Keywords:** Home, favoritos, planificación de itinerarios, busqueda por categoria, turismo inteligente, reservas y gestion de experiencias.
- **Meta Author:** Turisnap 

### 4.2.4. Searching Systems
Para garantizar una experiencia de usuario fluida y eficiente, se ha definido un sistema de búsqueda que facilite el acceso a la información dentro de TripMatch. 
* **Búsqueda de destinos turísticos:** con filtros por tipo de lugar (playa, ciudad, naturaleza), presupuesto, temporada y popularidad.
* **Búsqueda de experiencias:** por categoría (aventura, cultura, gastronomía), ubicación y duración.
* **Búsqueda por palabras clave:** desde cualquier pantalla, para encontrar rápidamente destinos, usuarios o actividades relacionadas.
* **Historial y búsquedas guardadas:** los usuarios podrán revisar búsquedas recientes y guardar filtros frecuentes para agilizar futuras consultas.

### 4.2.5. Navigation Systems 
El sistema de navegación de TripMatch ha sido diseñado para ofrecer una experiencia fluida, adaptada a los distintos perfiles de usuario: turistas y agencias. La interfaz presenta una navegación lateral que permite un acceso rápido a las funciones principales, y mantiene una estructura coherente en toda la plataforma.

**Navegación principal para turistas:**

- **Inicio:** Punto de partida que muestra recomendaciones, novedades y experiencias destacadas.
- **Buscar:** Permite explorar destinos y actividades mediante filtros avanzados.
- **Itinerario:** Sección donde se visualizan, editan o crean nuevos itinerarios personalizados.
- **Favoritos:** Muestra actividades o lugares marcados previamente por el usuario.
- **Perfil:** Configuraciones personales, historial de viajes y preferencias.

**Navegación principal para anfitriones/agencias:**

- **Inicio:** Resumen de actividades programadas, métricas de interacción y novedades del sistema.
- **Gestión de experiencias:** Sección dedicada a registrar, editar o eliminar experiencias ofrecidas.
- **Reservas:** Visualización y administración de las reservas generadas por los turistas.
- **Consultas:** Interacción con usuarios interesados, resolución de dudas o solicitud de detalles.
- **Perfil de agencia:** Modificación de datos institucionales, fotos y verificación de identidad.

## 4.3. Landing Page UI Design
### 4.3.1. Landing Page Wireframe    

La navegación principal está compuesta por secciones clave: Home, About Us, Benefits, How Does It Work?, FAQs, Contact, complementadas por botones visibles de Login y Sign Up, ubicados estratégicamente para facilitar el acceso de los usuarios según su necesidad. La estructura de la landing page fue pensada para acompañar al visitante de forma progresiva, desde entender qué ofrece la aplicación, hasta generar confianza e impulsar la acción de registro.  

**Desktop Web Browser** 
Se presentan las siguientes secciones:  

+ Navbar: Fijo en la parte superior con todas las secciones del sitio y botones a la derecha para iniciar sesión o registrarse.
+ Hero Section: Imagen destacada, con un eslogan directo y botón de llamada a la acción que invita al usuario a unirse.
+ About Us: Breve sección que explica la misión y vision de nuestra aplicación.
+ Benefits: Cards visuales donde se muestran los beneficios clave de la plataforma tanto para agencias como turistas, con íconos y descripciones breves.
+ How Does It Work?: Sección paso a paso explicando el funcionamiento de la plataforma tanto para turistas y agencias.
+ FAQs: Preguntas frecuentes en formato acordeón, de fácil lectura y con foco en resolver dudas comunes.
+ Contact: Formulario básico para consultas o sugerencias, junto con correo electrónico y numero de contacto.
+ Footer: Redes sociales y accesos rápidos adicionales.

![Landing Page-Wireframe](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/678f981f0169c5a2ac6b3c842fbcddf71422b732/repo/img/Landing%20Page-Wireframe.png)

**Mobile Web Browser**    
En la versión móvil se incorpora un menú hamburguesa que al desplegarse permite acceder fácilmente a las secciones: Home, About Us, Benefits, How Does It Work?, FAQs, Contact, así como botones de Login y Sign Up.  

![Landing Page- Wireframe- Mobile- Menu](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/5947df7ea421ae74c31bc68d3101b1f22d542ebb/repo/img/Landing%20Page-%20Wireframe-%20Mobile-%20Menu.png)

Se mantiene una estructura vertical sencilla, optimizada para pantallas pequeñas, priorizando la legibilidad, la navegación por scroll y el toque con el dedo. Las secciones siguen el mismo orden y contenido que en la versión desktop.

![Landing Page- Wireframe- Mobile](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/bf744d951a38e32a5e0fad68ddd75ed8f76ee302/repo/img/Landing%20Page-%20Wireframe-%20Mobile.png)


### 4.3.2. Landing Page Mock-up  

El mock-up de la landing page presenta un diseño limpio, moderno y enfocado en la experiencia del usuario. Se emplea una estructura clara y jerárquica que guía al visitante desde la propuesta de valor hasta la acción de registro, utilizando una paleta de colores coherente con la identidad visual del proyecto. Se prioriza la legibilidad, el contraste visual y la accesibilidad, adaptando el contenido tanto para pantallas de escritorio como para móviles, asegurando una experiencia fluida y responsiva en cualquier dispositivo.  

![Landing Page- Mock Up](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/4f8afc52f1a370bde296fec5e8ecc92ab0a01c52/repo/img/Landing%20Page-%20Mock%20Up.png)

## 4.4. Web Applications UX/UI Design
### 4.4.1. Web Applications Wireframes  
La propuesta de wireframes fue desarrollada aplicando los principios de diseño inclusivo, accesibilidad, jerarquía visual y usabilidad. Se busca asegurar una navegación clara y coherente, tanto para turistas como para agencias, adaptando la estructura y contenido de la interfaz según el tipo de usuario para optimizar su experiencia.  

Estructura General  
La interfaz cuenta con una barra de navegación dinámica que varía según el perfil del usuario (turista o agencia). Las secciones están organizadas para facilitar el acceso rápido a las funcionalidades más importantes para cada rol.

**Para turistas**  
Se divide en Inicio, favoritos, itinerarios y una barra de busqueda rapida, donde podra buscar agencias y experiencias por nombre.

**Inicio**  
Esta sección presenta un buscador con filtros (por tipo, lugar, precio y dia) que permite a los usuarios explorar experiencias turísticas de manera rápida. También se muestran recomendaciones personalizadas según intereses y tendencias.  

![Wireframe-home-tourits](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/60055f00da2f08bfc72e5b672a2a93ac2f9ec49e/repo/img/Wireframe-home-tourits.png)

*Favoritos*
Aquí se almacenan todas las experiencias marcadas como favoritas por el turista, permitiendo un acceso rápido a opciones que desea considerar más adelante.   

![Wireframe-favorites-tourits](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/60055f00da2f08bfc72e5b672a2a93ac2f9ec49e/repo/img/Wireframe-favorites-tourits.png)

**Itinerarios**  

Se muestra el historial de reservas del usuario, permitiéndole ver detalles de sus próximas experiencias y acceder fácilmente a la información necesaria para cada actividad.    

![Wireframe-itinerary-tourits](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/60055f00da2f08bfc72e5b672a2a93ac2f9ec49e/repo/img/Wireframe-itinerary-tourits.png)

**Resultados de la busqueda**  
Aqui se mostraran los resultados de las busquedas que el usuario realice.   

![Wireframe-search-tourits](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/60055f00da2f08bfc72e5b672a2a93ac2f9ec49e/repo/img/Wireframe-search-tourits.png)

**visualización de perfil de agencias para Turistas**  

Aquí se muestran los datos públicos de la agencia (nombre, descripcion, contacto, etc.), con opción de editar su información cuando sea necesario.  
![Wireframe-agency-profile-tourits](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/2d313351d5e938869d86695983c970985068b092/repo/img/Wireframe-agency-profile-tourits.png) 

**Para Agencias de Turismo**  

**Inicio**  

Brinda una vista general del estado actual de la agencia, incluyendo un resumen, comentarios o reseñas recientes de sus experiencias, y algunas reservas recientes.    

![Wireframe-home-agency](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/a95d44f93bd9e52eba59b1e95ea86f7dc78c247e/repo/img/Wireframe-home-agency.png)  


**Gestión de experiencias**  

Permite a la agencia crear, editar o eliminar experiencias turísticas.  

![Wireframe-Experience-Management-agency](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/a95d44f93bd9e52eba59b1e95ea86f7dc78c247e/repo/img/Wireframe-Experience-Management-agency.png)   


**Reservas**   

En esta sección se listan todas las reservas hechas por los turistas, con información detallada por experiencia y fecha. Incluye filtros para facilitar la gestión.    

![Wireframe-Reservations-agency](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/60055f00da2f08bfc72e5b672a2a93ac2f9ec49e/repo/img/Wireframe-Reservations-agency.png)  


**Consultas**  

Las agencias pueden ver preguntas o dudas realizadas por los usuarios respecto a sus experiencias y responderlas desde esta misma vista.  

![Wireframe-Consultations-agency](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/60055f00da2f08bfc72e5b672a2a93ac2f9ec49e/repo/img/Wireframe-Consultations-agency.png)  


**Perfil de agencia**  

Aquí se muestran los datos públicos de la agencia (nombre, descripcion, contacto, etc.), con opción de editar su información cuando sea necesario.  

![Wireframe-agency-profile-agency](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/2d313351d5e938869d86695983c970985068b092/repo/img/Wireframe-agency-profile-agency.png) 


### 4.4.2. Web Applications Wireflow Diagrams  
Esta sección presenta los Wireflows propuestos para los principales objetivos de usuario identificados en la plataforma, considerando tanto el perfil del turista como el de la agencia.  

Los diagramas reflejan visualmente cómo evoluciona cada pantalla en función de las acciones del usuario, mostrando tanto los estados iniciales como los cambios posteriores. Estos flujos no solo ilustran la navegación paso a paso, sino que también evidencian cómo se aplican principios de diseño centrado en el usuario, arquitectura de información y consistencia en la interfaz.    

**Turistas**  

Buscar experiencias turisticas

![Wireflow-BuscarExperiencia](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/dbbfda72981dfeb881f50f9a9da1804e8e7fb187/repo/img/Wireflow-BuscarExperiencia.png)    

Cancelar reserva 

![Wireflow- Cancelar reserva](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/dbbfda72981dfeb881f50f9a9da1804e8e7fb187/repo/img/Wireflow-%20Cancelar%20reserva.png)     

Dejar una reseña

![Wireflow- Dejar Reseña](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/dbbfda72981dfeb881f50f9a9da1804e8e7fb187/repo/img/Wireflow-%20Dejar%20Rese%C3%B1a.png)  

Realizar una consulta

![Wireflow- Realizar una consulta](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/dbbfda72981dfeb881f50f9a9da1804e8e7fb187/repo/img/Wireflow-%20Realizar%20una%20consulta.png)  

Realizar una reserva

![Wireflow- Realizar reserva](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/dbbfda72981dfeb881f50f9a9da1804e8e7fb187/repo/img/Wireflow-%20Realizar%20reserva.png) 

Seleccionar como experiencias como favoritas

![Wireflow- Seleccionar Favoritas](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/dbbfda72981dfeb881f50f9a9da1804e8e7fb187/repo/img/Wireflow-%20Seleccionar%20Favoritas.png)    

**Para Agencias de Turismo**    

Registrar una experiencia turística  

![Wireflow-RegistrarExperiencia](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/dbbfda72981dfeb881f50f9a9da1804e8e7fb187/repo/img/Wireflow-RegistrarExperiencia.png)   

Editar una experiencia ya creada

![Wireflow-EditarExperiencia](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/dbbfda72981dfeb881f50f9a9da1804e8e7fb187/repo/img/Wireflow-EditarExperiencia.png)    

Eliminar una experiencia ya creada 

![Wireflow- Eliminar experiencia](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/dbbfda72981dfeb881f50f9a9da1804e8e7fb187/repo/img/Wireflow-%20Eliminar%20experiencia.png)    

Editar perfil de agencia  

![Wireflow-EditarPerfil](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/dbbfda72981dfeb881f50f9a9da1804e8e7fb187/repo/img/Wireflow-EditarPerfil.png)    

Ver reservas  

![Wireflow- Cancelar reserva](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/dbbfda72981dfeb881f50f9a9da1804e8e7fb187/repo/img/Wireflow-%20Ver%20reservas.png)  

Responder consultas a los clientes

![Wireflow- Responder consultas](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/dbbfda72981dfeb881f50f9a9da1804e8e7fb187/repo/img/Wireflow-%20Responder%20consultas.png)    


Ver reseñas  

![Wireflow- Ver reseñas](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/dbbfda72981dfeb881f50f9a9da1804e8e7fb187/repo/img/Wireflow-%20Ver%20rese%C3%B1as.png)  


### 4.4.2. Web Applications Mock-ups  

La propuesta de Mock-ups busca representar visualmente la experiencia final de la aplicación web, integrando los principios de diseño inclusivo, jerarquía informativa, accesibilidad y consistencia visual. El diseño responde a las necesidades diferenciadas de turistas y agencias, priorizando la claridad en la navegación, la eficiencia en las tareas y la estética alineada al propósito del proyecto.  
Se utilizó un diseño que incluye una paleta de colores asociada al turismo sostenible, íconos comprensibles, tipografía legible y componentes reutilizables que aseguran coherencia y escalabilidad. 

**Turistas**  
Los mock-ups para turistas presentan una interfaz enfocada en la exploración de experiencias, con una sección de inicio que destaca filtros intuitivos y recomendaciones personalizadas. Las secciones de favoritos e itinerarios permiten un acceso rápido al contenido guardado o reservado. La barra de búsqueda se presenta de forma accesible en todo momento, facilitando la localización de agencias o experiencias específicas.  

**Inicio**    

![Mockup-home-tourits](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/2d313351d5e938869d86695983c970985068b092/repo/img/Mockup-home-tourits.png)

**Favoritos**  

![Mockup-favorites-tourits](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/2d313351d5e938869d86695983c970985068b092/repo/img/Mockup-favorites-tourits.png) 
 
**Itinerarios**    
![Mockup-itinerary-tourits](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/2d313351d5e938869d86695983c970985068b092/repo/img/Mockup-itinerary-tourits.png) 
 
**Resultados de la busqueda**  

![Mockup-search-tourits](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/2d313351d5e938869d86695983c970985068b092/repo/img/Mockup-search-tourits.png)

**visualización de perfil de agencias para Turistas**  

![Mockup-agency-profile-tourits](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/2d313351d5e938869d86695983c970985068b092/repo/img/Mockup-agency-profile-tourits.png) 

**Para Agencias de Turismo**    
En el caso de las agencias, los mock-ups reflejan una interfaz orientada a la gestión eficiente. En el inicio se muestran métricas clave, últimas reservas y reseñas recientes. Las secciones de gestión de experiencias y reservas cuentan con formularios organizados, tablas y botones de acción bien jerarquizados. Se prioriza la claridad en los procesos de edición, respuesta a consultas y mantenimiento del perfil público de la agencia.

Ambas interfaces fueron diseñadas pensando en una experiencia fluida tanto en pantallas de escritorio como en dispositivos con distintas resoluciones, asegurando una estructura responsive y accesible para todos los usuarios.

**Inicio**    

![Mockup-home-agency](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/d3cb25cddbb2b987d03de52888ac8b784b142851/repo/img/Mockup-home-agency.png)  


**Gestión de experiencias**  

![Mockup-Experience-Management-agency](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/d3cb25cddbb2b987d03de52888ac8b784b142851/repo/img/Mockup-Experience-Management-agency.png)   


**Reservas**       

![Mockup-Reservations-agency](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/d3cb25cddbb2b987d03de52888ac8b784b142851/repo/img/Mockup-Reservations-agency.png)  


**Consultas**      

![Mockup-Consultations-agency](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/d3cb25cddbb2b987d03de52888ac8b784b142851/repo/img/Mockup-Consultations-agency.png)  


**Perfil de agencia**   

![Mockup-agency-profile-agency](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/d3cb25cddbb2b987d03de52888ac8b784b142851/repo/img/Mockup-agency-profile-agency.png) 

### 4.4.3. Web Applications User Flow Diagrams    
Esta sección presenta los User Flows diseñados para las aplicaciones web en su versión de escritorio, con el objetivo de cubrir rutas clave de interacción para cada tipo de usuario: turista y agencia. Cada flujo muestra visualmente el recorrido que realiza el usuario a través de la aplicación, integrando los mock-ups de las pantallas involucradas. Se consideran tanto rutas exitosas (happy path) como posibles rutas alternativas (unhappy path), asegurando que la navegación sea intuitiva, inclusiva y coherente con la arquitectura de información planteada.  

**Turistas**  

Como turista, quiero poder buscar experiencias turísticas.

![User Flow- Buscar Experiencias](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/7ccc87cf2815964f6e1206a4a0527c4d4cb28478/repo/img/User%20Flow-%20Buscar%20Experiencias.png) 

Como turista, quiero poder realizar una reserva.

![User Flow- Realizar reserva](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/7ccc87cf2815964f6e1206a4a0527c4d4cb28478/repo/img/User%20Flow-%20Realizar%20reserva.png) 

Como turista, quiero poder cancelar una reserva.

![User Flow- Cancelar Reserva](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/7ccc87cf2815964f6e1206a4a0527c4d4cb28478/repo/img/User%20Flow-%20Cancelar%20Reserva.png) 

Como turista, quiero poder dejar una reseña sobre una experiencia realizada.

![User Flow- Dejar reseña](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/7ccc87cf2815964f6e1206a4a0527c4d4cb28478/repo/img/User%20Flow-%20Dejar%20rese%C3%B1a.png) 

Como turista, quiero poder realizar una consulta a una agencia.

![User Flow- Realizar consulta](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/7ccc87cf2815964f6e1206a4a0527c4d4cb28478/repo/img/User%20Flow-%20Realizar%20consulta.png) 

**Para Agencias de Turismo**   

Como agencia, quiero poder registrar una nueva experiencia turística.

![User Flow- Añadir experiencia](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/f191cc6947bce2b8b64c5d30abe2870922079e2c/repo/img/User%20Flow-%20A%C3%B1adir%20experiencia.png) 

Como agencia, quiero poder editar una experiencia ya creada.

![User Flow- Editar Experiencia](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/f191cc6947bce2b8b64c5d30abe2870922079e2c/repo/img/User%20Flow-%20Editar%20Experiencia.png) 

Como agencia, quiero poder eliminar una experiencia ya creada.

![User Flow- Eliminar experiencia](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/f191cc6947bce2b8b64c5d30abe2870922079e2c/repo/img/User%20Flow-%20Eliminar%20experiencia.png) 

Como agencia, quiero poder ver las reservas recibidas.

![User Flow- Reservas](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/f191cc6947bce2b8b64c5d30abe2870922079e2c/repo/img/User%20Flow-%20Reservas.png) 

Como agencia, quiero poder responder consultas de los turistas.

![User Flow- Añadir respuesta](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/f191cc6947bce2b8b64c5d30abe2870922079e2c/repo/img/User%20Flow-%20A%C3%B1adir%20respuesta.png) 

Como agencia, quiero poder ver las respuestas enviadas.

![User Flow- Ver respuestas](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/f191cc6947bce2b8b64c5d30abe2870922079e2c/repo/img/User%20Flow-%20Ver%20respuestas.png) 

Como agencia, quiero poder editar mi perfil.

![User Flow- Editar perfil de agencia](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/f191cc6947bce2b8b64c5d30abe2870922079e2c/repo/img/User%20Flow-%20Editar%20perfil%20de%20agencia.png) 


## 4.5. Web Applications Prototyping  
En esta sección se presentan los prototipos de interfaz de usuario desarrollados para la versión web en navegadores de escritorio, tanto para turistas como para agencias. Estos prototipos simulan la navegación e interacción con las principales funcionalidades, en base a los flujos definidos previamente en los Wireflow Diagrams.

Las decisiones de interacción se tomaron considerando principios de usabilidad, claridad visual, diseño inclusivo y una arquitectura de información coherente. Se priorizó una navegación intuitiva, adaptada al perfil y objetivos de cada usuario. El sistema de navegación, las jerarquías visuales y los tipos de interacción fueron diseñados para facilitar la exploración de contenido, la gestión de experiencias y la reserva de actividades turísticas.

Los prototipos permiten visualizar el comportamiento del sistema ante las principales tareas definidas, asegurando una experiencia consistente y funcional. Se incluye una captura de pantalla y un enlace al video en Microsoft Stream donde se muestra la simulación de interacción correspondiente.

![Web applications Prototyping](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/70941c8f2719e5708a2e09d475ae0fc0a3c823c6/repo/img/Web%20applications%20Prototyping%20.png)   

Link del video: https://upcedupe-my.sharepoint.com/:v:/g/personal/u20231c505_upc_edu_pe/EWCB3XE4nJhNpKf_2ovj8msB2RBu4poQh48oS5TLIKm62w?e=7f7JKE&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D



## 4.6. Domain-Driven Software Architecture
### 4.6.1. Software Architecture Context Diagram
Este diagrama muestra el sistema TripMatch dentro de su entorno, identificando cómo interactúa con usuarios y otros sistemas externos.

![Context Diagram TripMatch](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/24f26df0194624dd22d187b0970bfe8789b22c93/repo/img/SystemContext-TripMatch.png)

### 4.6.2. Software Architecture Container Diagrams
Este diagrama detalla los principales contenedores (aplicaciones o servicios ejecutables) que componen el sistema y cómo se comunican entre sí.

![Component Diagram TripMatch](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/24f26df0194624dd22d187b0970bfe8789b22c93/repo/img/DiagramadeContenedores-TripMatch.png)

### 4.6.3. Software Architecture Components Diagrams
Este diagrama profundiza en los componentes internos del contenedor principal

![Container Diagram TripMatch](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/24f26df0194624dd22d187b0970bfe8789b22c93/repo/img/DiagramadeComponentes-TripMatch.png)

## 4.7. Software Object-Oriented Design
### 4.7.1. Class Diagrams   

![Diagrama de Clase](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/304aabc577cdb5cc4438162d01076c550aa6284e/repo/img/Aplicaciones%20Web%20-%20P%C3%A1gina%201%20(12).png)

### 4.7.2. Class Dictionary  

**User**

Entidad base que representa a cualquier usuario de la plataforma.

| Campo     | Tipo de dato | Descripción                        |
|-----------|--------------|------------------------------------|
| _id       | UUID         | Identificador único del usuario    |
| firstName | String       | Nombre del usuario                 |
| lastName  | String       | Apellido del usuario               |
| number    | String       | Número de contacto                 |
| email     | Email        | Correo del usuario                 |
| password  | Password     | Contraseña del usuario             |

**AgencyUser**

Usuario que representa a una agencia, hereda de User.

| Campo         | Tipo de dato     | Descripción                                |
|---------------|------------------|--------------------------------------------|
| agencyName    | String           | Nombre de la agencia                        |
| ruc           | String           | Registro Único de Contribuyente             |
| contactInfo   | String           | Información de contacto adicional           |
| publicProfile | PublicProfile    | Perfil público visible de la agencia        |
| location      | Location         | Ubicación física de la agencia              |

**TouristUser**

Usuario con rol de turista, hereda de `User`.

| Campo       | Tipo de dato | Descripción                         |
|-------------|--------------|-------------------------------------|
| preferences | String[]     | Preferencias del turista            |

**PublicProfile**

Perfil público de una agencia.

| Campo       | Tipo de dato | Descripción               |
|-------------|--------------|---------------------------|
| bio         | String       | Biografía o presentación  |
| website     | String       | Página web oficial        |
| socialLinks | List<String> | Redes sociales asociadas  |

**Booking**

Reserva hecha por un usuario para una experiencia.

| Campo          | Tipo de dato | Descripción                              |
|----------------|--------------|------------------------------------------|
| id             | UUID         | ID de la reserva                         |
| experienceId   | UUID         | ID de la experiencia reservada           |
| userId         | UUID         | ID del usuario que reserva               |
| bookingDate    | DateTime     | Fecha y hora de la reserva               |
| numberOfPeople | Int          | Número de personas incluidas en la reserva |

**Inquiry**

Consulta hecha por un turista a una agencia.

| Campo          | Tipo de dato | Descripción                          |
|----------------|--------------|--------------------------------------|
| id             | UUID         | ID de la consulta                    |
| experienceId   | UUID         | ID de la experiencia consultada      |
| fromUserId     | UUID         | ID del usuario que consulta          |
| toAgencyUserId | UUID         | ID de la agencia consultada          |
| question       | String       | Pregunta del usuario                 |
| answer         | String       | Respuesta de la agencia              |
| askedAt        | DateTime     | Fecha de consulta                    |
| answeredAt     | DateTime     | Fecha de respuesta                   |

**Review**

Reseña hecha por un usuario sobre una experiencia.

| Campo        | Tipo de dato | Descripción                            |
|--------------|--------------|----------------------------------------|
| id           | UUID         | ID de la reseña                        |
| userId       | UUID         | ID del usuario que realizó la reseña   |
| rating       | Number       | Calificación otorgada                  |
| comment      | String       | Comentario de la reseña                |
| createdAt    | DateTime     | Fecha de creación                      |
| favorite     | Boolean      | Marca si es una reseña destacada       |

**Experience**

Experiencia publicada por una agencia.

| Campo          | Tipo de dato   | Descripción                             |
|----------------|----------------|-----------------------------------------|
| id             | UUID           | ID de la experiencia                    |
| title          | String         | Título de la experiencia                |
| description    | String         | Descripción detallada                   |
| location       | Location       | Ubicación de la experiencia             |
| price          | Money          | Precio de la experiencia                |
| duration       | String         | Duración estimada                       |
| meetingPoint   | String         | Punto de encuentro                      |
| schedule       | Schedule[]     | Horarios disponibles                    |
| categories     | Category[]     | Categorías de la experiencia            |
| photos         | Photo[]        | Imágenes relacionadas                   |
| availableDates | AvailableDate[]| Fechas disponibles                      |

**Category**

Categoría asociada a una experiencia.

| Campo | Tipo de dato | Descripción               |
|-------|--------------|---------------------------|
| _id   | UUID         | Identificador único       |
| name  | String       | Nombre de la categoría    |

**Schedule**

Días y horarios disponibles para una experiencia.

| Campo     | Tipo de dato | Descripción                  |
|-----------|--------------|------------------------------|
| dayOfWeek | String       | Día de la semana             |
| times     | String[]     | Horarios disponibles         |

**Photo**

Imagen de una experiencia.

| Campo   | Tipo de dato | Descripción               |
|---------|--------------|---------------------------|
| url     | String       | URL de la imagen          |
| caption | String       | Descripción de la imagen  |

**PriceRange**

Rango de precios usado en filtros de búsqueda.

| Campo | Tipo de dato | Descripción         |
|-------|--------------|---------------------|
| min   | Number       | Precio mínimo       |
| max   | Number       | Precio máximo       |

**Location**

Ubicación geográfica.

| Campo       | Tipo de dato | Descripción                 |
|-------------|--------------|-----------------------------|
| country     | String       | País                        |
| city        | String       | Ciudad                      |

## 4.8. Database Design
### 4.8.1. Database Diagram
![Database-Diagram](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/9a9b262a3d89d0c8b172d7cd74b30bc24068da9c/repo/img/Turisfera-Database-Diagram.png)
