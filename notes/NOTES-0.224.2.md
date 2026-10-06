## Correcciones importantes

- **Se cruzaban datos entre ligas.** Dentro de una liga o torneo aparecían partidos y resultados de otras, y al entrar en una liga se veían los de toda la temporada. El filtro que acota a competición, liga o fase había dejado de aplicarse y las peticiones lo ignoraban en silencio. Afectaba a toda la API, así que también corrige listados que mostraban de más.
- **Los árbitros se filtraban por partidos arbitrados** en vez de por las competiciones en las que están inscritos: los recién inscritos no aparecían.
- **Los estadios se filtraban por sus partidos**: uno recién creado no salía hasta tener el primero. Ahora van por los grupos donde están dados de alta.
- **«Últimos resultados» mostraba partidos no jugados.** Bastaba con que tuvieran marcador, así que un aplazado con resultado antiguo se colaba. Ahora solo salen los finalizados.
- **Faltaban los escudos** de los equipos en los últimos resultados del resumen público.
- **El acceso con Google no aparecía en ninguna pantalla de login**: la clave no llegaba a la compilación de la web, así que el botón se ocultaba siempre aunque estuviera activado.

## Inscripciones

- **Una sola puerta de entrada.** Antes cada vía tenía su enlace suelto, así que quien llegaba desde la web pública solo veía una opción y no podía cambiarla. Ahora se elige con tarjetas: jugador o representante de equipo y, después, el destino concreto.
  - **Jugador**: equipos con inscripción abierta **y plazas libres** (indicando cuántas quedan) o la bolsa.
  - **Representante**: equipos sin representante o proponer uno nuevo, si la competición y la liga lo permiten.
  - Solo se ofrece lo que está realmente abierto; con una única vía se entra directo sin preguntar.
- **Un equipo con la plantilla llena ya no se ofrece**: inscribirse ahí era un rechazo seguro. Antes un límite de 0 plazas se interpretaba como «sin límite».
- Las páginas públicas de inscripción y de bolsa llevan el **pie completo** de la web pública, respetando el diseño propio de la organización, y recuperan el guiño de la lluvia de balones al pulsar la cabecera.

## Panel

- **Fichajes** pasa a ir debajo de Palmarés en el menú de la competición.
- Los logins recortaban por arriba desde que se añadió el acceso con Google: el logo quedaba pegado al borde y bajo el selector de tipo de usuario.
- El aviso «Sigue lo que te interesa, sin registrarte» se muestra encima de los resultados oficiales.
- **Feature flags**: el desplegable de funcionalidades se ve bien en móvil.

## Listado de partidos
- **Los partidos de cada equipo muestran la hora, el estadio y el árbitro** sin tener que entrar en cada uno. En móvil, estadio y árbitro se muestran bajo la fecha para que quepan.

## Acceso con Google
- **Entrar con Google ya no crea cuentas en el panel ni en la app de árbitro.** Un correo sin cuenta recibía una de aficionado recién creada y acababa dentro de una app que no le corresponde; ahora se le avisa de que no existe. Desde la web pública sí se da de alta, como aficionado.
- **Los aficionados quedan asociados a la organización** desde cuya web pública se registraron, así que el organizador puede verlos y contarlos.

## Usuarios
- **Los aficionados se pueden consultar** en Usuarios y en Superadmin. No salen por defecto —son muchos y taparían a la gente de la organización— pero se filtran por su rol.
- **Superadmin → Resumen** muestra cuántos aficionados hay.
- **Los desplegables de filtros se salían de la pantalla en móvil**: copiaban el ancho y la posición del botón, así que quedaban estrechos y desplazados.

---

Las funcionalidades de inscripciones, bolsa y contabilidad interna siguen **desactivadas por defecto**: se activan por organización desde Superadmin → Feature flags.
