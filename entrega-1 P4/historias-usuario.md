# 1. Personal del Archivo Histórico del Atlántico (C.L.E.N.A) - Usuario Interno

## HU-01: Visualización del Tablero de Solicitudes

Como personal del Archivo Histórico (C.L.E.N.A). Quiero visualizar en un panel interactivo todas las solicitudes de consulta o documentación generadas por los usuarios. Con el objetivo de llevar un control organizado, identificar su estado actual y gestionar la atención de forma oportuna.

Criterios de Aceptación:
- Dado que el usuario interno accede al módulo de solicitudes, cuando carga la pantalla principal, entonces se visualiza un tablero o lista con las solicitudes agrupadas por estado (Ej.: Pendiente, En Revisión, Aprobada, Rechazada).
- Dado el listado de solicitudes, cuando el usuario interno aplica un filtro por fecha, tipo de documento o estado, entonces la vista se actualiza mostrando únicamente las coincidencias.

## HU-02: Aprobación y Gestión de Solicitudes

Como personal de Archivo Histórico (C.L.E.N.A). Quiero evaluar los detalles de una solicitud recibida para aprobarla o rechazarla fundadamente. Para garantizar la viabilidad del trámite y el cumplimiento de las normativas de conservación.

Criterios de Aceptación:
- Dado que se inspecciona una solicitud específica, cuando el usuario interno selecciona la opción "Aprobar", entonces el sistema cambia el estado a Aprobada y habilita las acciones de seguimiento correspondiente.
- Dado que los datos ingresados son insuficientes o inviables, cuando se selecciona "Rechazar", entonces el sistema exige ingresar una causa de rechazo antes de confirmar el cambio de estado.

## HU-03: Contacto Directo y Notificación al Solicitante

Como personal del Archivo Histórico (C.L.E.N.A). Quiero disponer de un canal de comunicación integrado (o envió de notificaciones directas con el solicitante). Para solicitar aclaraciones sobre la búsqueda, coordinar entregas o comunicar el estado de su trámite.

Criterios de Aceptación:
- Dado una solicitud en estado de atención, cuando el usuario interno redacta un mensaje desde el detalle de la solicitud y hace clic en "Enviar", entonces el sistema envía una notificación vía correo electrónico (o sistema de alertas) al usuario público solicitante.
- Dado que el usuario responde o envía información adicional, cuando ingresa dicha respuesta, entonces el historial del mensaje queda trazado en el detalle de la solicitud dentro del sistema.

## HU-04: Verificación de Datos Solicitante vía Correo Electrónico

Como personal del Archivo Histórico (C.L.E.N.A). Quiero enviar una solicitud formal de verficación o confirmación de datos de identidad e interés académico/legal al correo electrónico del usuario. Para validar la autenticidad de la solicitud y asegurar que e trámite cumpla con los requisitos antes de procesar o autorizar el acceso a la documentación.

Criterios de Aceptación:
- Dado que el usuario interno está revisando una solicitud en estado Pendiente, cuando selecciona la opción "Solicitar Verificación de Datos", entonces el sistema despliega una plantilla de correo parametrizable donde se indican los datos específicos a confirmar o los documentos de soporte requeridos.
- Dado que el mensaje es enviado, cuando el sistema procesa la acción, entonces el estado de la solicitud cambia automáticamente a En Espera de Verificación por Correo y se registra la fecha y hora de la notificación.
- Dado que el usuario externo responde al correo de verificación o adjunta los soportes requeridos desde el enlace enviado, cuando el sistema recibe la respuesta, entonces notifica al personal de archivo y actualiza el estado a Datos Verificados para continuar con el flujo de aprobación.

## HU-05: Búsqueda Descriptiva Avanzada de Documentos e Información

Como personal del Archivo Histórico (C.L.E.N.A). Quiero realizar búsquedas en el fondo documental utilizando descriptores temáticos, palabras clave, contextos históricos, eventos o fragmentos de contenido. Para verificar la existencia de un texto o documento en el acervo cuando el solicitante desconoce el título exacto, el autor o la signatura topográfica.

Criterios de Aceptación:
- Dado que el usuario interno accede al módulo de búsqueda de documentos, cuando selecciona la opción "Búsqueda por Descripción / Palabras Clave", entonces el sistema habilita campos de búsqueda por contexto histórico, temas, fechas aproximadas o términos presentes en el resumen/transcripción del documento.
- Dado que se ingresa una consulta descriptiva (ej. "decretos sobre navegación en el río Magdalena a finales del siglo XIX"), cuando se ejecuta la búsqueda, entonces el sistema retorna una lista de coincidencias jerarquizada por nivel de relevancia conceptual o temático.
- Dado el resultado de la búsqueda descriptiva, cuando el personal selecciona un documento de la lista, entonces puede visualizar sus metadatos detallados y vincularlo directamente a la solicitud del usuario público para su posterior atención.

# 2. Usuario Público - Usuario Externo

## HU-06: Formulario Guiado de Creación de Solicitudes

Como usuario público. Quiero disponer de una interfaz clara con instrucciones detalladas sobre los requisitos necesarios al momento de radicar una solicitud. Para ingresar los datos correctos (Ej: tipo de documento, parámetros de verificación) y evitar inconsistencias o rechazos.

Criterios de Aceptación:
- Dado que el usuario externo inicia una nueva solicitud, cuando selecciona el tipo de documento requerido, entonces el sistema despliega dinámicamente los campos obligatorios a diligenciar (Ej.: período histórico, nombre del archivo/fondo, datos de verificación).
- Dado que el usuario intenta enviar la solicitud sin completar los datos requeridos, cuando hace clic en "Enviar", entonces el sistema resalta los campos faltantes e impide la radicación hasta corregirlos.

## HU-07: Solicitud de Citas o Acceso a Documentación Digitalizada/Restringida

Como usuario público. Quiero solicitar la digitalización o agendar una cita de consulta presencial cuando el material solicitado tenga restricciones físicas de conservación. Para acceder al contenido sin comprometer el estado ni el valor del documento original.

Criterios de Aceptación:
- Dado que la documentación requerida posee restricciones de manipulación física por su estado de conservación, cuando el usuario selecciona "Solicitar Cita de Consulta en Sala" o "Solicitar Copia Digitalizada", entonces el sistema le permite seleccionar una fecha disponible de la agenda o registrar la justificación de la consulta.
- Dado que se procesa la solicitud de un documento digitalizado restringido, cuando la solicitud es aprobada, entonces el usuario recibe las indicaciones de acceso seguro o la confirmación de la cita agendada.

# 3. Administrador - Usuario Interno

## HU-08: Gestión de Usuarios y Roles del Sistema

Como Administrador del sistema. Quiero administrar el alta, baja y modificación de usuarios y sus niveles de acceso jerárquico. Para asegurar que solo el personal autorizado acceda a los módulos de gestión interna y a los datos sensibles.

Criterios de Aceptación:
- Dado que se requiere incorporar un nuevo miembro del equipo del C.L.E.N.A., cuando el administrador ingresa los datos y asigna un rol (Ej.: Operador de Archivo, Administrador), entonces el sistema genera la cuenta con las restricciones asociadas al rol seleccionado.
- Dado que un usuario deja de formar parte de la institución, cuando el administrador desactiva su cuenta, entonces se deniega inmediatamente su acceso a la plataforma.