## Estado de una competición

- **Cambiar el estado al editar no se guardaba.** La ficha que llega del servidor no traía el dato «oculta», así que al guardar se reenviaba siempre «no oculta»: elegir «Oculta» no se conservaba y una competición oculta se desocultaba sola al tocar cualquier otra cosa.
- **Una competición oculta ya no sale en «resultados oficiales»** de la portada pública.

## Acceso al panel

- **El acceso de organizador de la web pública no llevaba a ninguna parte.** Cuando no se sabe de qué organización es quien entra —un superadmin no pertenece a una concreta— el enlace va a la pantalla de acceso, y esa pantalla no hacía nada si ya había sesión. Ahora lleva directo al panel.
- **En la app de árbitro faltaba el acceso al panel** para administradores sin organización guardada.
