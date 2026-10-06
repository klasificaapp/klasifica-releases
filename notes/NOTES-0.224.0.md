Entrega grande: llega todo el bloque de **inscripciones, bolsa de equipos y jugadores y contabilidad interna**, que llevaba tiempo en una rama aparte.

Todo va **desactivado por defecto**: cada funcionalidad se activa por organización desde Superadmin → Feature flags. Hasta que las actives, la app funciona igual que antes.

## Inscripciones públicas
- Formulario público de **jugador**: enlace por equipo, verificación del correo con código, foto y documento, consentimientos y aviso de cuotas. Si recargas a media inscripción no pierdes lo escrito.
- Formulario público de **gestor de equipo**: hacerse cargo de un equipo existente o proponer uno nuevo, si la liga lo permite.
- **Bandeja de solicitudes**: aprobar, rechazar con plantillas de motivo, revertir un rechazo, notas internas, duplicados, aprobación en bloque y exportación a CSV.
- Aprobar **crea de verdad**: cuenta, ficha del jugador y alta en la plantilla con dorsal y posición.
- **Código de seguimiento** para que cada solicitante consulte su estado.
- **Ventanas de inscripción** por liga y **plantillas** reutilizables.
- **Permisos del gestor** sobre sus jugadores en cascada competición → liga → equipo. Borrar nunca: eso se solicita.
- **Reglamento** con editor visual, extras por liga y aceptación obligatoria.

## Bolsa de equipos y jugadores
- Quien no tiene equipo, o trae uno sin plaza, se apunta a la bolsa de la liga. No entra en nada por su cuenta.
- **El organizador decide**: al incluir a alguien elige el equipo, y ahí se aplican las cuotas de ese equipo.
- Se abre en dos niveles: la **competición** lo permite y cada **liga** decide si abre y **entre qué fechas**.
- **Aviso en la web pública** con tu mensaje, enlazando al formulario.

## Fichajes (menú nuevo)
- Las altas nuevas (bolsa y solicitudes) tienen su propio menú. **Alineaciones** se queda con la gente ya inscrita —plantillas, cambios de datos y bajas— y avisa de cuántos esperan en la bolsa.

## Contabilidad interna
- **Pagos por competición**: previsto, cobrado y pendiente, resumen por equipo y cargos extra con vencimiento.
- **Pagos por equipo**: nueva pestaña en la ficha del equipo.
- Marcar cobros indicando **método** (efectivo, transferencia, bizum), con registro de quién y cuándo, avisos de vencidos y CSV.

## Superadmin
- **Feature flags**: al elegir organización se ve qué tiene activado y qué ha decidido ella misma, para no duplicar excepciones. Las no desplegadas quedan al final y no se activan por error.
- Ya se pueden activar **Cuentas de aficionado y acceso con Google**.

## Correcciones
- **Los formularios públicos con adjuntos llegaban vacíos al servidor**: fallaba cualquier envío con foto o documento.
- **Suplantar a un usuario desde Superadmin no servía para navegar**: se rechazaba en la primera petición.
- La configuración de una liga borrada devolvía un error genérico.
