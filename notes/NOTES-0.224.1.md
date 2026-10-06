Correcciones sobre la 0.224.0.

## Correcciones
- **El acceso con Google no aparecía en las pantallas de login** (organizador y árbitro) aunque estuviera activado. Las funcionalidades que se deciden por organización no llegaban a resolverse en páginas sin sesión iniciada, así que quedaban apagadas justo donde hacían falta.

## Superadmin
- **Feature flags**: el desplegable de funcionalidades muestra el estado de cada una directamente en la lista —activada, desactivada, excepción de la organización o aún no desplegada—, así que se ve de un vistazo qué se puede activar y no se duplican excepciones. El panel de estado aparte ya no hace falta.

---

Recordatorio de lo que llegó en la **0.224.0** (todo desactivado por defecto, se activa por organización desde Superadmin → Feature flags): inscripciones públicas de jugadores y gestores, bolsa de equipos y jugadores por liga con ventana de fechas, menú Fichajes y contabilidad interna por competición y equipo.
