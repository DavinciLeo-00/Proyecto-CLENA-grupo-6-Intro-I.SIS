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

## HU-06: Control y Registro de Préstamos Físicos en Sala de Consulta

Como personal del Archivo Histórico (C.L.E.N.A). Quiero registrar el préstamo y la devolución de documentos físicos dentro de la sala de consulta presencial mediante un sistema de control temporal. Para evitar extravíos, asegurar la trazabilidad de qué investigador manipuló el material y controlar los tiempos máximos de permanencia del documento fuera de su depósito.

Criterios de Aceptación
- Dado que un usuario público se presenta a su cita presencial aprobada, cuando el personal de archivo entrega los documentos físicos para su consulta, entonces registra en el sistema la hora de entrega, el código del documento y el número de identificación del investigador.
- Dado que el investigador finaliza su jornada de estudio o vence el tiempo estipulado, cuando devuelve el material, entonces el operador registra la devolución y el sistema cambia automáticamente el estado del documento a En Depósito / Disponible.
- Dado que un documento no ha sido devuelto a la hora límite del cierre de sala, entonces el sistema emite una alerta visual en el panel del operador marcando el préstamo como Vencido / Pendiente de Devolución.

## HU-07: Registro de Transferencias Documentales desde Entidades Externas

Como personal del Archivo Histórico(C.L.E.N.A). Quiero registrar formalmente el ingreso de transferencias documentales primarias o secundarias enviadas por entidades públicas o donantes particulares del departamento del Atlántico. Para mantener un inventario riguroso de las actas de entrega, la procedencia de los fondos y la ubicación topográfica inicial en los depósitos.

Criterios de Aceptación:
- Dado que se recibe un lote físico de documentos por parte de una entidad externa, cuando el personal ingresa al módulo de "Transferencias Documentales" y completa el formato de inventario (cajas, carpetas y fechas extremas), entonces el sistema genera un número único de radicado de transferencia y un acta descargable en PDF para la firma de las partes.
- Dado que el inventario ha sido radicado, cuando el personal asigna la ubicación física dentro de los estantes del archivo, entonces el sistema actualiza la signatura topográfica de cada expediente, facilitando su posterior búsqueda descriptiva.

# 2. Usuario Público - Usuario Externo

## HU-08: Formulario Guiado de Creación de Solicitudes

Como usuario público. Quiero disponer de una interfaz clara con instrucciones detalladas sobre los requisitos necesarios al momento de radicar una solicitud. Para ingresar los datos correctos (Ej: tipo de documento, parámetros de verificación) y evitar inconsistencias o rechazos.

Criterios de Aceptación:
- Dado que el usuario externo inicia una nueva solicitud, cuando selecciona el tipo de documento requerido, entonces el sistema despliega dinámicamente los campos obligatorios a diligenciar (Ej.: período histórico, nombre del archivo/fondo, datos de verificación).
- Dado que el usuario intenta enviar la solicitud sin completar los datos requeridos, cuando hace clic en "Enviar", entonces el sistema resalta los campos faltantes e impide la radicación hasta corregirlos.

## HU-09: Solicitud de Citas o Acceso a Documentación Digitalizada/Restringida

Como usuario público. Quiero solicitar la digitalización o agendar una cita de consulta presencial cuando el material solicitado tenga restricciones físicas de conservación. Para acceder al contenido sin comprometer el estado ni el valor del documento original.

Criterios de Aceptación:
- Dado que la documentación requerida posee restricciones de manipulación física por su estado de conservación, cuando el usuario selecciona "Solicitar Cita de Consulta en Sala" o "Solicitar Copia Digitalizada", entonces el sistema le permite seleccionar una fecha disponible de la agenda o registrar la justificación de la consulta.
- Dado que se procesa la solicitud de un documento digitalizado restringido, cuando la solicitud es aprobada, entonces el usuario recibe las indicaciones de acceso seguro o la confirmación de la cita agendada.

# 3. Administrador - Usuario Interno

## HU-10: Gestión de Usuarios y Roles del Sistema

Como Administrador del sistema. Quiero administrar el alta, baja y modificación de usuarios y sus niveles de acceso jerárquico. Para asegurar que solo el personal autorizado acceda a los módulos de gestión interna y a los datos sensibles.

Criterios de Aceptación:
- Dado que se requiere incorporar un nuevo miembro del equipo del C.L.E.N.A., cuando el administrador ingresa los datos y asigna un rol (Ej.: Operador de Archivo, Administrador), entonces el sistema genera la cuenta con las restricciones asociadas al rol seleccionado.
- Dado que un usuario deja de formar parte de la institución, cuando el administrador desactiva su cuenta, entonces se deniega inmediatamente su acceso a la plataforma.

## HU-11: Reportes Estadísticos y Cuadro de Mando Operativo

Como Administrador (o directivo) del Archivo Histórico del Atlántico. Quiero generar métricas y reportes sobre la cantidad de solicitudes recibidas, tipos de documentos y tiempos de respuesta. Para evaluar el cumplimiento de objetivos institucionales, tomar decisiones estratégicas y supervisar el funcionamiento del equipo.

Criterios de Aceptación:
- Dado que el administrador ingresa al módulo de reportes, cuando define un rango de fechas, entonces el sistema genera indicadores gráficos con la cantidad de solicitudes aprobadas, rechazadas y en proceso.
- Dado la necesidad de realizar auditorías externas o análisis internos, cuando el administrador hace clic en "Exportar Reporte", entonces el sistema descarga un archivo estructurado (CSV/Excel) con el resumen consolidado de las solicitudes y uso del archivo.

## HU-12: Gestión de Auditoría y Protecció de Datos Personales

Como Administrador. Quiero restringir y auditar las operaciones sobre información sensible y datos personales de los solicitantes. Para preservar la confiedencialidad, la trazabilidad del sistema y la alineación con la jerarquía laboral.

Criterios de Aceptación:
- Dado que un usuario interno consulta o modifica datos personales específicos de un solicitante, cuando realiza dicha acción, entonces el sistema registra en una bitácora de auditoría (logs) el ID del usuario, fecha, hora y acción ejecutada.
- Dado que un rol sin privilegios intenta acceder a la configuración del sistema o a datos restringidos, cuando intenta ingresar a la ruta, entonces el sistema bloquea el acceso y muestra un mensaje de permisos insuficientes.