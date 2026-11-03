1. Personal del Archivo Histórico del Atlántico (C.L.E.N.A) - Usuario Interno

# HU-01: Visualización del Tablero de Solicitudes

Como personal del Archivo Histórico (C.L.E.N.A). Quiero visualizar en un panel interactivo todas las solicitudes de consulta o documentación generadas por los usuarios. Con el objetivo de llevar un control organizado, identificar su estado actual y gestionar la atención de forma oportuna.

Criterios de Aceptación:
- Dado que el usuario interno accede al módulo de solicitudes, cuando carga la pantalla principal, entonces se visualiza un tablero o lista con las solicitudes agrupadas por estado (Ej.: Pendiente, En Revisión, Aprobada, Rechazada).
- Dado el listado de solicitudes, cuando el usuario interno aplica un filtro por fecha, tipo de documento o estado, entonces la vista se actualiza mostrando únicamente las coincidencias.

# HU-02: Aprobación y Gestión de Solicitudes

Como personal de Archivo Histórico (C.L.E.N.A). Quiero evaluar los detalles de una solicitud recibida para aprobarla o rechazarla fundadamente. Para garantizar la viabilidad del trámite y el cumplimiento de las normativas de conservación.

Criterios de Aceptación:
- Dado que se inspecciona una solicitud específica, cuando el usuario interno selecciona la opción "Aprobar", entonces el sistema cambia el estado a Aprobada y habilita las acciones de seguimiento correspondiente.
- Dado que los datos ingresados son insuficientes o inviables, cuando se selecciona "Rechazar", entonces el sistema exige ingresar una causa de rechazo antes de confirmar el cambio de estado.

# HU-03: Contacto Directo y Notificación al Solicitante

Como personal del Archivo Histórico (C.L.E.N.A). Quiero disponer de un canal de comunicación integrado (o envió de notificaciones directas con el solicitante). Para solicitar aclaraciones sobre la búsqueda, coordinar entregas o comunicar el estado de su trámite.

Criterios de Aceptación:
- Dado una solicitud en estado de atención, cuando el usuario interno redacta un mensaje desde el detalle de la solicitud y hace clic en "Enviar", entonces el sistema envía una notificación vía correo electrónico (o sistema de alertas) al usuario público solicitante.
- Dado que el usuario responde o envía información adicional, cuando ingresa dicha respuesta, entonces el historial del mensaje queda trazado en el detalle de la solicitud dentro del sistema.