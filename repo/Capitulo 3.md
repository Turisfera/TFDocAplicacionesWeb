# Capítulo 3: Requirements Specifications
## 3.1. To-Be Scenario Mapping  
>Segmento 1: Turistas

![TO-BE - segmento 1](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/d41e472b5b48cbcdc28645e4b56808b4ae963e8c/repo/img/TO-BE%20-%20Segmento%201.jpg)

>Segmento 2: Agencias de Turismo

![TO-BE - segmento 2](https://github.com/Turisfera/TFDocAplicacionesWeb/blob/d41e472b5b48cbcdc28645e4b56808b4ae963e8c/repo/img/TO-BE%20-%20Segmento%202.jpg)

## 3.2. User Stories

|Épica : 01||||
| :- | :- | :- | :- |
|ID - HU|01|Owner|Turisfera|
|Título HU|Registro de usuario|||
|Descripción HU:<br>**Como** usuario, **quiero** registrarme en la aplicación **para** poder acceder a sus funcionalidades y planificar mis viajes.||||
|<p>Escenario : Validación de registro de usuario</p><p></p><p>**Dado que** el sistema verifica que el correo electrónico no esté registrado</p><p>**Y** el usuario selecciona "Crear cuenta"</p><p>**Cuando** el usuario ingresa todos los campos requeridos y hace clic en "Registrar"</p><p>**Entonces** el sistema valida los datos y crea la cuenta del usuario</p><p>**Y** muestra un mensaje de éxito en el registro</p>||||

|Épica : 01||||
| :- | :- | :- | :- |
|ID - HU|02|Owner|Turisfera|
|Título HU|Validación de datos de registro|||
|Descripción HU: **Como** usuario, **quiero** que el sistema valide mis datos correctamente al registrarme **para** evitar errores.||||
|<p>Escenario : Validación de campos obligatorios</p><p>**Dado que** el usuario intenta registrarse<br>` `**Y** el sistema detecta campos vacíos o mal ingresados<br>` `**Cuando** el usuario hace clic en "Registrar"<br>` `**Entonces** el sistema muestra mensajes de error junto a los campos incorrectos<br>` `**Y** evita que se complete el registro hasta que todos los campos sean válidos</p><p></p>||||

|Épica : 01||||
| :- | :- | :- | :- |
|ID - HU|03|Owner|Turisfera|
|Título HU|Confirmación de contraseña|||
|Descripción HU:<br>**Como** usuario, **quiero** confirmar mi contraseña durante el registro **para** asegurarme de que la escribí correctamente.||||
|<p>Escenario: Comparación de contraseña y confirmación</p><p></p><p>**Dado que** el usuario ingresa su contraseña en dos campos distintos</p><p>**Y** el sistema debe comparar ambas</p><p>**Cuando** el usuario hace clic en "Registrar"</p><p>**Entonces** el sistema valida que ambas contraseñas coincidan</p><p>**Y** muestra un mensaje de error si son diferente</p>||||

|Épica : 01||||
| :- | :- | :- | :- |
|ID - HU|04|Owner|Turisfera|
|Título HU|Mensaje de bienvenida|||
|Descripción HU:<br>**Como** usuario, **quiero** recibir un mensaje de bienvenida después de registrarme **para** sentirme valorado.||||
|<p>Escenario: Registro exitoso con saludo inicial</p><p></p><p>**Dado que** el usuario ha completado exitosamente el proceso de registro</p><p>**Y** el sistema crea su cuenta</p><p>**Cuando** se redirige al usuario a la pantalla principal</p><p>**Entonces** el sistema muestra un mensaje de bienvenida con su nombre</p>||||

|Épica : 01||||
| :- | :- | :- | :- |
|ID - HU|05|Owner|Turisfera|
|Título HU|Registro con redes sociales|||
|Descripción HU:<br>**Como** usuario, **quiero** poder registrarme con mi cuenta de Google o Facebook **para** ahorrar tiempo.||||
|<p>Escenario: Registro mediante cuenta social</p><p></p><p>**Dado que** el usuario selecciona "Registrarse con Google/Facebook"</p><p>**Y** concede los permisos necesarios</p><p>**Cuando** se completa la autenticación externa</p><p>**Entonces** el sistema crea una cuenta en Turisfera con los datos recibidos</p><p>**Y** redirige al usuario a la pantalla principal</p>||||

|Épica : 01||||
| :- | :- | :- | :- |
|ID - HU|06|Owner|Turisfera|
|Título HU|Confirmación por correo electrónico|||
|Descripción HU:<br>**Como** usuario, **quiero** recibir un correo de confirmación después de registrarme **para** validar mi cuenta.||||
|<p>Escenario: Envío de correo de confirmación</p><p></p><p>**Dado que** el usuario ha completado el formulario de registro</p><p>**Y** ha ingresado un correo electrónico válido</p><p>**Cuando** el sistema crea la cuenta</p><p>**Entonces** se envía un correo con un enlace de verificación</p><p>**Y** el usuario debe hacer clic en el enlace para activar su cuenta</p>||||

|Épica : 02||||
| :- | :- | :- | :- |
|ID - HU|07|Owner|Turisfera|
|Título HU|Búsqueda de destinos turísticos|||
|Descripción HU:<br>**Como** usuario, **quiero** buscar destinos turísticos dentro de la aplicación **para** explorar opciones de viaje que se ajusten a mis intereses.||||
|<p>Escenario: Búsqueda por nombre del destino</p><p></p><p>**Dado que** el usuario se encuentra en la sección de búsqueda</p><p>**Y** desea encontrar un destino específico</p><p>**Cuando** el usuario escribe el nombre del destino en la barra de búsqueda</p><p>**Entonces** el sistema muestra resultados relacionados con el nombre ingresado</p><p>**Y** permite al usuario seleccionar uno para ver más detalles</p>||||

|Épica : 02||||
| :- | :- | :- | :- |
|ID - HU|08|Owner|Turisfera|
|Título HU|Filtros de búsqueda|||
|Descripción HU:<br>**Como** usuario, **quiero** usar filtros al buscar destinos **para** encontrar los que se ajusten a mis preferencias.||||
|<p>Escenario: Aplicación de filtros de búsqueda</p><p></p><p>**Dado que** el usuario está explorando destinos turísticos</p><p>**Y** desea ajustar los resultados</p><p>**Cuando** selecciona filtros como tipo de destino, clima o presupuesto</p><p>**Entonces** el sistema actualiza los resultados según los filtros seleccionados</p>||||

|Épica : 02||||
| :- | :- | :- | :- |
|ID - HU|09|Owner|Turisfera|
|Título HU|Resultados relevantes de búsqueda|||
|Descripción HU:<br>**Como** usuario, **quiero** que los resultados de búsqueda sean relevantes **para** no perder tiempo revisando opciones irrelevantes||||
|<p>Escenario: Resultados personalizados por preferencia</p><p></p><p>**Dado que** el usuario ha ingresado un término de búsqueda</p><p>**Y** ha configurado previamente sus intereses</p><p>**Cuando** se realiza la búsqueda</p><p>**Entonces** el sistema ordena los resultados según relevancia y preferencias del usuario</p>||||

|Épica : 02||||
| :- | :- | :- | :- |
|ID - HU|10|Owner|Turisfera|
|Título HU|Vista previa de destinos|||
|Descripción HU:<br>**Como** usuario, **quiero** ver una vista previa de cada destino **para** decidir rápidamente cuál me interesa explorar.||||
|<p>Escenario: Mostrar resumen de destinos en resultados</p><p></p><p>**Dado que** el usuario visualiza la lista de resultados</p><p>**Y** está explorando varias opciones</p><p>**Cuando** se muestra cada destino</p><p>**Entonces** el sistema incluye nombre, imagen, calificación y breve descripción en la vista previa</p>||||

|Épica : 02||||
| :- | :- | :- | :- |
|ID - HU|11|Owner|Turisfera|
|Título HU|Acceso rápido a destino favorito|||
|Descripción HU:<br>**Como** usuario, **quiero** poder marcar destinos como favoritos **para** acceder a ellos rápidamente más adelante.||||
|<p>Escenario: Agregar destino a favoritos</p><p>**<br>` `**Dado que** el usuario ha encontrado un destino interesante<br>` `**Y** desea guardarlo<br>` `**Cuando** hace clic en el ícono de favorito<br>` `**Entonces** el sistema lo agrega a la lista de favoritos del usuario<br>` `**Y** permite consultarlo fácilmente desde su perfil</p><p></p>||||

|Épica : 02||||
| :- | :- | :- | :- |
|ID - HU|12|Owner|Turisfera|
|Título HU|Búsqueda por región o país|||
|Descripción HU:<br>**Como** usuario, **quiero** buscar destinos por país o región **para** explorar zonas específicas que me interesen.||||
|<p>Escenario: Filtro de región geográfica</p><p></p><p>**Dado que** el usuario quiere ver destinos dentro de una región específica</p><p>**Y** selecciona la región desde un menú desplegable</p><p>**Cuando** aplica el filtro</p><p>**Entonces** el sistema muestra únicamente los destinos que pertenecen a esa región o país seleccionado</p>||||

|Épica : 03||||
| :- | :- | :- | :- |
|ID - HU|13|Owner|Turisfera|
|Título HU|Crear nuevo itinerario de viaje|||
|Descripción HU:<br>**Como** usuario, **quiero** crear un itinerario **para** organizar mis actividades y lugares a visitar durante el viaje.||||
|<p>Escenario: Creación de un itinerario nuevo</p><p>**<br>` `**Dado que** el usuario ha elegido un destino<br>` `**Y** desea planificar su viaje<br>` `**Cuando** selecciona la opción "Crear itinerario"<br>` `**Entonces** el sistema permite ingresar fechas, actividades y lugares para cada día<br>` `**Y** guarda el itinerario en el perfil del usuario</p><p></p>||||

|Épica : 03||||
| :- | :- | :- | :- |
|ID - HU|14|Owner|Turisfera|
|Título HU|Editar itinerario existente|||
|Descripción HU:<br>**Como** usuario, **quiero** editar mis itinerarios **para** ajustarlos en caso de cambios en mis planes.||||
|<p>Escenario: Edición de un itinerario guardado</p><p></p><p>**Dado que** el usuario ya tiene un itinerario creado</p><p>**Y** desea modificarlo</p><p>**Cuando** selecciona el itinerario y edita alguna actividad</p><p>**Entonces** el sistema actualiza la información modificada</p><p>**Y** guarda los cambios automáticamente</p>||||

|Épica : 03||||
| :- | :- | :- | :- |
|ID - HU|15|Owner|Turisfera|
|Título HU|Eliminar itinerario|||
|<p>Descripción HU:<br>**Como** usuario, **quiero** eliminar un itinerario que ya no necesito **para** mantener mi cuenta organizada.</p><p></p>||||
|<p>Escenario: Eliminación de itinerario</p><p>**<br>` `**Dado que** el usuario ha accedido a su lista de itinerarios<br>` `**Y** desea eliminar uno<br>` `**Cuando** selecciona "Eliminar"<br>` `**Entonces** el sistema solicita confirmación<br>` `**Y** elimina el itinerario seleccionado si el usuario acepta</p><p></p>||||

|Épica : 03||||
| :- | :- | :- | :- |
|ID - HU|16|Owner|Turisfera|
|Título HU|Visualizar itinerario completo|||
|<p>Descripción HU:<br>**Como** usuario, **quiero** visualizar todos los detalles de mi itinerario **para** revisarlo antes y durante el viaje.</p><p></p>||||
|<p>Escenario: Visualización de detalles del itinerario</p><p>**<br>` `**Dado que** el usuario tiene itinerarios guardados<br>` `**Y** desea consultarlos<br>` `**Cuando** selecciona un itinerario<br>` `**Entonces** el sistema muestra toda la información detallada por día, hora y actividad</p><p></p>||||

|Épica : 03||||
| :- | :- | :- | :- |
|ID - HU|17|Owner|Turisfera|
|Título HU|Añadir lugares sugeridos al itinerario|||
|<p>Descripción HU:<br>**Como** usuario, **quiero** añadir lugares recomendados por la app a mi itinerario **para** enriquecer mi experiencia.</p><p></p>||||
|<p>Escenario: Agregar lugares sugeridos</p><p></p><p>**Dado que** el usuario explora recomendaciones de la app</p><p>**Y** desea incluir una en su itinerario</p><p>**Cuando** hace clic en "Añadir al itinerario"</p><p>**Entonces** el sistema agrega el lugar en la fecha y hora seleccionada del itinerario</p>||||

|Épica : 03||||
| :- | :- | :- | :- |
|ID - HU|18|Owner|Turisfera|
|Título HU|Compartir itinerario con otros usuarios|||
|Descripción HU:<br>**Como** usuario, **quiero** compartir mi itinerario con amigos o familiares **para** que puedan verlo o sugerir cambios.||||
|<p>Escenario: Compartir itinerario por enlace</p><p>**<br>` `**Dado que** el usuario tiene un itinerario creado<br>` `**Y** desea compartirlo<br>` `**Cuando** hace clic en "Compartir"<br>` `**Entonces** el sistema genera un enlace o permite enviarlo por redes sociales<br>` `**Y** las personas con el enlace pueden visualizar el itinerario</p><p></p>||||

|Épica : 04||||
| :- | :- | :- | :- |
|ID - HU|19|Owner|Turisfera|
|Título HU|Enviar solicitud de amistad a otros usuarios|||
|Descripción HU:<br>**Como** usuario, **quiero** enviar solicitudes de amistad a otros viajeros **para** poder conectarme con personas con intereses similares.||||
|<p>Escenario: Enviar solicitud de amistad</p><p></p><p>**Dado que** el usuario ha encontrado otro perfil interesante</p><p>**Y** desea conectarse</p><p>**Cuando** hace clic en "Agregar amigo"</p><p>**Entonces** el sistema envía una solicitud de amistad al otro usuario</p><p>**Y** este podrá aceptarla o rechazarla</p>||||

|Épica : 04||||
| :- | :- | :- | :- |
|ID - HU|20|Owner|Turisfera|
|Título HU|Aceptar o rechazar solicitudes de amistad|||
|Descripción HU:<br>**Como** usuario, **quiero** aceptar o rechazar solicitudes de amistad **para** controlar con quién me conecto.||||
|<p>Escenario: Gestión de solicitudes de amistad</p><p></p><p>**Dado que** el usuario recibe una solicitud</p><p>**Cuando** accede a la sección de notificaciones</p><p>**Entonces** el sistema le permite aceptar o rechazar la solicitud</p><p>**Y** actualiza la lista de amigos según la acción tomada</p>||||

|Épica : 04||||
| :- | :- | :- | :- |
|ID - HU|21|Owner|Turisfera|
|Título HU|Ver perfiles de amigos|||
|Descripción HU:<br>**Como** usuario, **quiero** ver los perfiles de mis amigos **para** conocer sus intereses y próximos viajes.||||
|<p>Escenario: Visualización del perfil de un amigo</p><p>**<br>` `**Dado que** el usuario ya tiene amigos agregados<br>` `**Cuando** accede a su lista de amigos y selecciona uno<br>` `**Entonces** el sistema muestra el perfil público del amigo con sus datos, itinerarios compartidos y lugares visitados</p><p></p>||||

|Épica : 04||||
| :- | :- | :- | :- |
|ID - HU|22|Owner|Turisfera|
|Título HU|Enviar mensajes a amigos|||
|Descripción HU:<br>**Como** usuario, **quiero** enviar mensajes privados a mis amigos **para** coordinar viajes o compartir recomendaciones.||||
|<p>Escenario: Enviar mensaje privado</p><p></p><p>**Dado que** el usuario ya tiene amigos agregados</p><p>**Y** desea iniciar una conversación</p><p>**Cuando** selecciona a un amigo y abre el chat</p><p>**Entonces** el sistema permite enviar y recibir mensajes en tiempo real</p>||||

|Épica : 04||||
| :- | :- | :- | :- |
|ID - HU|23|Owner|Turisfera|
|Título HU|Comentar en itinerarios compartidos|||
|Descripción HU:<br>**Como** usuario, **quiero** comentar en los itinerarios de mis amigos **para** dar sugerencias o felicitarlos por su planificación.||||
|<p>Escenario: Comentar en itinerarios</p><p></p><p>**Dado que** el usuario visualiza un itinerario compartido</p><p>**Y** desea dejar un comentario</p><p>**Cuando** escribe y publica su comentario</p><p>**Entonces** el sistema lo muestra en la sección correspondiente del itinerario compartido</p>||||

|Épica : 04||||
| :- | :- | :- | :- |
|ID - HU|24|Owner|Turisfera|
|Título HU|Recibir notificaciones de actividad de amigos|||
|Descripción HU:<br>**Como** usuario, **quiero** recibir notificaciones cuando mis amigos creen itinerarios o compartan contenido, **para** mantenerme al tanto.||||
|<p>Escenario: Notificación de actividad de amigos</p><p>**<br>` `**Dado que** el usuario tiene amigos en su red<br>` `**Cuando** uno de ellos crea un nuevo itinerario o publica contenido<br>` `**Entonces** el sistema envía una notificación al usuario<br>` `**Y** le permite acceder directamente a ese contenido desde la notificación</p><p></p>||||

|Épica : 05||||
| :- | :- | :- | :- |
|ID - HU|25|Owner|Turisfera|
|Título HU|Buscar destinos turísticos por nombre|||
|Descripción HU:<br>**Como** usuario, **quiero** buscar destinos turísticos por nombre **para** encontrar rápidamente el lugar que deseo visitar.||||
|<p>Escenario: Búsqueda por nombre de destino</p><p>**<br>` `**Dado que** el usuario está en la sección de búsqueda<br>` `**Cuando** ingresa el nombre de un destino en el buscador<br>` `**Entonces** el sistema muestra una lista de coincidencias relacionadas con el término ingresado</p><p></p>||||

|Épica : 05||||
| :- | :- | :- | :- |
|ID - HU|26|Owner|Turisfera|
|Título HU|Filtrar destinos por tipo de experiencia|||
|Descripción HU:<br>**Como** usuario, **quiero** filtrar los destinos por tipo de experiencia (aventura, relax, cultura, etc.) **para** encontrar opciones que se alineen con mis intereses.||||
|<p>Escenario: Filtrar destinos</p><p></p><p>**Dado que** el usuario accede a la búsqueda avanzada</p><p>**Cuando** selecciona una o varias categorías de experiencia</p><p>**Entonces** el sistema muestra solo aquellos destinos que coincidan con los filtros seleccionados</p>||||

|Épica : 05||||
| :- | :- | :- | :- |
|ID - HU|27|Owner|Turisfera|
|Título HU|Explorar destinos por ubicación geográfica|||
|Descripción HU:<br>**Como** usuario, **quiero** explorar destinos utilizando un mapa interactivo **para** descubrir lugares de interés visualmente.||||
|<p>Escenario: Navegar por mapa interactivo</p><p></p><p>**Dado que** el usuario accede al mapa de exploración</p><p>**Cuando** selecciona una región o país</p><p>**Entonces** el sistema muestra los destinos disponibles en esa zona y permite ver detalles adicionales</p>||||

|Épica : 05||||
| :- | :- | :- | :- |
|ID - HU|28|Owner|Turisfera|
|Título HU|Ver detalles de un destino turístico|||
|Descripción HU:<br>**Como** usuario, **quiero** ver la información completa de un destino (fotos, descripción, actividades disponibles) **para** decidir si me interesa visitarlo.||||
|<p>Escenario: Visualización del destino</p><p></p><p>**Dado que** el usuario ha seleccionado un destino de la lista</p><p>**Cuando** hace clic en su nombre o imagen</p><p>**Entonces** el sistema muestra una página con todos los detalles del destino y opciones relacionadas</p>||||

|Épica : 05||||
| :- | :- | :- | :- |
|ID - HU|29|Owner|Turisfera|
|Título HU|Guardar destinos favoritos|||
|Descripción HU:<br>**Como** usuario, **quiero** guardar destinos como favoritos **para** poder acceder rápidamente a ellos en el futuro.||||
|<p>Escenario: Agregar a favoritos</p><p></p><p>**Dado que** el usuario ve un destino interesante</p><p>**Cuando** presiona el botón "Guardar como favorito"</p><p>**Entonces** el sistema añade ese destino a su lista personal de favoritos y lo confirma con un mensaje</p>||||

|Épica : 05||||
| :- | :- | :- | :- |
|ID - HU|30|Owner|Turisfera|
|Título HU|Ver recomendaciones de destinos según preferencias|||
|Descripción HU:<br>**Como** usuario, **quiero** recibir recomendaciones de destinos según mis búsquedas y preferencias **para** descubrir nuevas opciones personalizadas.||||
|<p>Escenario: Sugerencias personalizadas</p><p></p><p>**Dado que** el usuario ha interactuado con el sistema (búsquedas, favoritos, filtros)</p><p>**Cuando** accede a la sección de recomendaciones</p><p>**Entonces** el sistema muestra una lista de destinos sugeridos que se alinean con sus intereses y comportamientos anteriores</p>||||


## 3.3. Impact Mapping

El Impact Mapping es una metodología visual y ágil que permite a las organizaciones enfocar el desarrollo de productos y servicios en función de sus metas estratégicas. Esta técnica facilita la identificación de una relación directa entre los objetivos del negocio, las acciones esperadas de los usuarios clave y las soluciones o funcionalidades que deben implementarse para lograr dichos objetivos.![Impact Mapping](img/Impact-map-Turisfera.png)

## 3.4. Product Backlog

|# Orden|User Story Id|Description|Story Points (1 /3 /5 /8)|
| :-: | :-: | :-: | :-: |
|1|US01|**Como** usuario, **quiero** registrarme en la aplicación **para** poder acceder a sus funcionalidades y planificar mis viajes.|8|
|2|US02|**Como** usuario, **quiero** que el sistema valide mis datos correctamente al registrarme **para** evitar errores.|5|
|3|US03|**Como** usuario, **quiero** confirmar mi contraseña durante el registro **para** asegurarme de que la escribí correctamente.|3|
|4|US04|**Como** usuario, **quiero** recibir un mensaje de bienvenida después de registrarme **para** sentirme valorado.|8|
|5|US05|**Como** usuario, **quiero** poder registrarme con mi cuenta de Google o Facebook **para** ahorrar tiempo.|8|
|6|US06|**Como** usuario, **quiero** recibir un correo de confirmación después de registrarme **para** validar mi cuenta.|8|
|7|US07|**Como** usuario, **quiero** buscar destinos turísticos dentro de la aplicación **para** explorar opciones de viaje que se ajusten a mis intereses.|5|
|8|US08|**Como** usuario, **quiero** usar filtros al buscar destinos **para** encontrar los que se ajusten a mis preferencias.|5|
|9|US09|**Como** usuario, **quiero** que los resultados de búsqueda sean relevantes **para** no perder tiempo revisando opciones irrelevantes|3|
|10|US10|**Como** usuario, **quiero** ver una vista previa de cada destino **para** decidir rápidamente cuál me interesa explorar.|5|
|11|US11|**Como** usuario, **quiero** poder marcar destinos como favoritos **para** acceder a ellos rápidamente más adelante.|8|
|12|US12|**Como** usuario, **quiero** buscar destinos por país o región **para** explorar zonas específicas que me interesen.|8|
|13|US13|**Como** usuario, **quiero** crear un itinerario **para** organizar mis actividades y lugares a visitar durante el viaje.|5|
|14|US14|**Como** usuario, **quiero** editar mis itinerarios **para** ajustarlos en caso de cambios en mis planes.|5|
|15|US15|**Como** usuario, **quiero** eliminar un itinerario que ya no necesito **para** mantener mi cuenta organizada.|3|
|16|US16|<p>**Como** usuario, **quiero** visualizar todos los detalles de mi itinerario **para** revisarlo antes y durante el viaje.</p><p></p>|5|
|17|US17|**Como** usuario, **quiero** añadir lugares recomendados por la app a mi itinerario **para** enriquecer mi experiencia.|5|
|18|US18|**Como** usuario, **quiero** compartir mi itinerario con amigos o familiares **para** que puedan verlo o sugerir cambios.|8|
|19|US19|**Como** usuario, **quiero** enviar solicitudes de amistad a otros viajeros **para** poder conectarme con personas con intereses similares.|3|
|20|US20|**Como** usuario, **quiero** aceptar o rechazar solicitudes de amistad **para** controlar con quién me conecto.|3|
|21|US21|**Como** usuario, **quiero** ver los perfiles de mis amigos **para** conocer sus intereses y próximos viajes.|3|
|22|US22|**Como** usuario, **quiero** enviar mensajes privados a mis amigos **para** coordinar viajes o compartir recomendaciones.|5|
|23|US23|**Como** usuario, **quiero** comentar en los itinerarios de mis amigos **para** dar sugerencias o felicitarlos por su planificación.|5|
|24|US24|**Como** usuario, **quiero** recibir notificaciones cuando mis amigos creen itinerarios o compartan contenido, **para** mantenerme al tanto.|5|
|25|US25|**Como** usuario, **quiero** buscar destinos turísticos por nombre **para** encontrar rápidamente el lugar que deseo visitar.|5|
|26|US26|**Como** usuario, **quiero** filtrar los destinos por tipo de experiencia (aventura, relax, cultura, etc.) **para** encontrar opciones que se alineen con mis intereses.|5|
|27|US27|**Como** usuario, **quiero** explorar destinos utilizando un mapa interactivo **para** descubrir lugares de interés visualmente.|3|
|28|US28|**Como** usuario, **quiero** ver la información completa de un destino (fotos, descripción, actividades disponibles) **para** decidir si me interesa visitarlo.|3|
|29|US29|**Como** usuario, **quiero** guardar destinos como favoritos **para** poder acceder rápidamente a ellos en el futuro.|1|
|30|US30|**Como** usuario, **quiero** recibir recomendaciones de destinos según mis búsquedas y preferencias **para** descubrir nuevas opciones personalizadas.|3|