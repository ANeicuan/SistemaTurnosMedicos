# Requisitos iniciales del sistema
## Requisitos funcionales
- RF1 El sistema debe crear, reprogramar y cancelar turnos de manera ágil.
- RF2 Tener la capacidad de visualizar la agenda por día y semana.
- RF3 El sistema debe evitar que se generen conflictos con la agenda (doble turno en un mismo horario).
- RF4 Tiene que permitir configurar el horario base del profesional (Lunes a viernes de 9-13 y 15-19) y bloquear horarios por vacaciones, feriados, clases o reuniones.
- RF5 No debe permitir sobreturnos automáticos. Debe ser de forma manual por parte del profesional (máximo de dos por día).
- RF6 Debe tener diferentes duraciones predefinidas: 15 min para controles y 30 min para primera consulta. Debe contemplar que la duración real puede diferir de la predefinida.
- RF7 Debe incluirse la funcionalidad para marcar cuando un paciente llega físicamente al consultorio, registrando la hora real de llegada.
- RF8 Debe tener un registro OBLIGATORIO de todas las modificaciones y cancelaciones para resolver cualquier disputa sobre quien cambió un turno.
- RF9 Debe incluir entidades bien definidas para Paciente (Nombre, Teléfono, ID), Profesional, Turno (Estado, fecha, hora, tipo) y registro de presencia.
- RF10 El sistema debe permitir configurar restricciones particulares del profesional:
    - No atender los jueves.
    - No agendar primeras consultas los viernes a última hora.
    - No programar procedimientos los lunes.
    - Manejar una tolerancia de llegada de 10 min para decidir que hacer con el turno.
## Requisitos no funcionales

- RNF1 Debe enviar notificaciones automáticas el día anterior al turno, via WhatsApp (principal) y Mail.
- RNF2 La interfaz debe ser simple e intuitiva para que el profesional pueda utilizarla sin requerir un aprendizaje complejo.
- RNF3 El sistema debe ser diseñado de forma que permita el crecimiento futuro a múltiples medicos y consultorios sin romper el modelo base.
- RNF4 El sistema debe impedir usos incorrectos mediante un buen encapsulamiento de la lógica de negocio. Objetivo primordial es garantizar que no se superpongan turnos(salvo excepciones autorizadas).
- RNF5 El equipo de desarrollo tiene que priorizar un modelo inicial correcto y un diseño estable. No se deben realizar "parches", sino trabajar con referencias minimas para asegurar la mantenibilidad.
- RNF6 El sistema debe ser funcional para principios de Julio.
- RNF7 El modelo debe manejar conceptos del dominio ("intervalos de tiempo", "disponibilidad") de forma abstracta, no solo como datos técnicos o números sueltos, para reflejar fielmente el funcionamiento real del consultorio.
