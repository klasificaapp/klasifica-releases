Entrega que recoge lo de todo el día. Lo nuevo de esta versión va primero.

### Nuevo en esta versión
- **La pantalla de carga ya no lleva la marca de Klasifica.** Al actualizar
  aparecía siempre su logo y su nombre, también dentro de la app de una
  organización con su propia marca. Ahora es un esqueleto gris neutro.
- **Un trozo de la aplicación que no carga se resuelve solo.** Antes salía una
  pantalla de «¡Nueva versión disponible!» con un botón; ahora se limpia la
  caché y se recarga una vez, sin pedir nada. La pantalla de error queda para
  cuando falla también el segundo intento.
- **«Partidos (9) (9)»**: los partidos de un equipo mostraban el número dos
  veces.

### Fichajes
- **Fichajes es una pantalla propia del menú principal**, debajo de Palmarés.
  Estaba como pestaña dentro del detalle de una competición, donde no se
  encontraba.
- Muestra arriba la **competición y la liga seleccionadas** en los filtros, con
  acceso directo a cambiarlas; la configuración que se abre desde ahí es la de
  esa selección. Sin competición elegida, invita a escogerla.
- **Se queda solo con lo que abre o cierra la entrada de gente nueva**: la
  bolsa y las inscripciones, con sus parámetros.
- El aviso **«Elige una liga o torneo…» sale arriba**, bajo los filtros.

### Alineaciones
- **Los permisos del gestor de equipo sobre los jugadores viven aquí**, que es
  donde se trabaja con plantillas ya inscritas: el valor de la competición y la
  excepción de la liga o torneo seleccionados. También se dejan puestos al
  crear o editar la competición y la liga o torneo, donde el nivel de liga
  admite «Heredar».

### Correcciones
- **Fichajes y Patrocinadores no aparecían en el panel de otra organización.**
  Las funcionalidades activas se pedían con la organización del usuario y, al
  fijar la del panel, se descartaban sin volver a pedirlas.
- **Si el servidor no responde al pedir qué funcionalidades están activas, se
  reintenta**, en vez de dejar el menú sin ellas.
- **Al editar una liga o torneo se guardan la bolsa y sus fechas.** No se
  enviaban: el formulario mostraba un valor y se guardaba otro.
- **Las páginas públicas dejan de quedarse cargando para siempre**: con caché o
  filtros inservibles se limpian los filtros y se vuelve a la portada.
- **El aviso de versión nueva** sale arriba, se puede cerrar y solo aparece
  cuando de verdad hay una versión nueva (antes salía también en la primera
  visita).
- **El acceso con Google** funciona en las organizaciones que lo tienen
  activado: se comprobaba contra la organización equivocada.
