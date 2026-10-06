## Fichajes

- **Fichajes pasa a ser una pantalla propia del menú principal**, debajo de Palmarés. Estaba como pestaña dentro del detalle de una competición, donde no se encontraba: se consulta por sí misma, igual que Equipos o Jugadores.
- La pantalla **muestra arriba la competición y la liga seleccionadas** en los filtros, y la configuración que se abre desde ahí es siempre la de esa selección. Sin competición elegida, invita a escogerla.
- **Si el servidor no responde al pedir qué funcionalidades están activas, se reintenta.** Un fallo puntual las apagaba todas y los menús que dependen de ellas —Fichajes entre otros— desaparecían sin explicación.

## Avisos y recuperación

- **Un solo aviso de versión nueva, y se puede cerrar.** Cuando fallaba la carga de un trozo de la aplicación salía además una pantalla de «¡Nueva versión disponible!»: aparecían las dos. Esa situación ahora se resuelve sola (limpia la caché y recarga una vez) y la pantalla queda para errores de verdad.
- **Las páginas públicas dejan de quedarse cargando para siempre.** Con caché o filtros inservibles el esqueleto se quedaba fijo: pasados unos segundos se limpian los filtros y se vuelve a la portada.

---

Sin cambios de servidor en esta versión.
