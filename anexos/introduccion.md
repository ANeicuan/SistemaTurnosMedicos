# Anexo - Introducción al Diseño Orientado a Objetos

# Los cuatro fundamentos de POO

# Requisitos iniciales del sistema

# Casos de uso
 - **1** Gestion de Turnos: 
    - Crear turno: Registrar una cita asignando paciente, profesional, fecha, hora y tipo de consulta.
    - Reprogramar turnos: Mover una cita existente a un nuevo horario o fecha, asegurando que se notifique al paciente. 
    - Cancelación de turnos: Dar de baja un turno programado, registrando el motivo y notificando el cambio.
    - Autorizar sobreturno: Permitir la asignación de un paciente a un horario ya reservado. Esta es una decisión manual que debe ser autorizada por el profesional con un máximo de dos por día.
-  **2** Visualización y Control:
    - Visualizar agenda: Capacidad de consultar los turnos programados con una vista por día o por semana para cada profesional
    - Registrar Presencia: Registrar cuando un paciente llega físicamente al consultorio, con el horario de llegada real.
    - Historial de cambios: Registro de todas las modificaciones (creación, cambios y cancelaciones) con el fin de resolver disputas o dudas sobre la agenda.
- **3** Configuración de Disponibilidad:
    - Manejar disponibilidad base: Configurar horarios de atención habituales (Lunes a Viernes de 9-13 y 15-19).
    - Bloquear horarios: Inhabilitar turnos por motivos específicos como vacaciones, feriados, reuniones o guardias matutinas.
    - Definir restricciones de agenda: Establecer reglas específicas para no permitir primeras consultas los viernes a última hora o no programar procedimientos los lunes.
- **4** Funciones Automatizadas:
    - Evitar conflictos de agenda: Impedir automáticamente la superposición de dos turnos en el mismo horario, salvo que exista una autorización a dicho sobreturno.
    - Enviar notificaciones y recordatorios: Enviar avisos automáticos vía Whatsapp e Email al paciente el día anterior al turno y notificar inmediatamente ante cualquier cambio o cancelación.
- **5** Interacción del Paciente:
    - Notificar cancelación: Permitir que el paciente informe que no podrá asistir. Debe quedar registrado formalmente en el sistema.

# Boceto inicial del diseño de clases
