## Acceso con Google en la app instalada

- La app usa ahora el **acceso de Android**, con la cuenta del propio teléfono. El botón web no podía funcionar ahí porque la app no se sirve desde un dominio autorizado.
- **Pendiente de configuración**: hay que crear el cliente de Android en Google Cloud (paquete `com.klasifica.app` + huella de firma). Hasta entonces, el botón dará error al pulsarlo.

## Sesiones a medias

- **Si quedaban credenciales guardadas sin usuario, la aplicación se quedaba en tierra de nadie**: ni mostraba la cuenta ni ofrecía entrar, y el acceso con Google desaparecía porque creía que ya había sesión. Al arrancar se recupera el perfil o se limpia todo.
- Tras entrar con Google se completa el perfil (nombre y apellidos), que no viene en la respuesta del acceso y dejaba el menú de la cuenta vacío.
