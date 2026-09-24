# Requisitos del Sistema de Gestión de Biblioteca Universitaria

## Requisitos funcionales

1. El sistema debe permitir registrar libros con título, autor, ISBN y disponibilidad.
2. El sistema debe permitir registrar usuarios (estudiantes, profesores y personal administrativo).
3. El sistema debe permitir realizar préstamos de libros según el tipo de usuario.
4. El sistema debe permitir registrar devoluciones y calcular retrasos.
5. El sistema debe permitir consultar el historial de préstamos por usuario.



\## Requisitos no funcionales



1\. El sistema debe ser accesible desde navegador web.

2\. El sistema debe responder en menos de 3 segundos por consulta.

3\. El sistema debe resguardar los datos personales de los usuarios.

4\. El sistema debe estar disponible al menos 95% del tiempo en horario escolar.



\## Nota del Ejercicio 5


Este documento fue modificado localmente sin actualizar main,

para simular el escenario de una copia desactualizada.

\## Políticas de préstamo por tipo de usuario



A partir de la solicitud del cliente, la biblioteca atenderá a tres tipos

de usuario con políticas diferenciadas: 



\- Estudiantes: hasta 3 libros por 10 días.

\- Profesores: hasta 5 libros por 15 días.

\- Personal administrativo: hasta 2 libros por 5 días.



\### Requisitos funcionales asociados



1\. El sistema debe identificar el tipo de usuario al momento del préstamo.

2\. El sistema debe aplicar automáticamente la política correspondiente.

3\. El sistema debe registrar el tipo de usuario en cada préstamo.



\### Excepciones a las políticas



\- Los profesores con antigüedad mayor a 5 años podrán solicitar hasta 7 libros.

\- El personal administrativo podrá renovar préstamos una vez si no hay lista de espera.

## Módulo de Reservas

### Reglas de negocio

- **RBR-01:** Solo se permite reservar un libro cuando su disponibilidad sea 0 (stock agotado).
- **RBR-02:** Al confirmar la reserva, el sistema debe registrar automáticamente la fecha de la solicitud.
- **RBR-03:** El sistema debe registrar el usuario que realizó la reserva.
- **RBR-04:** Una reserva queda en estado "pendiente" hasta que el libro esté disponible nuevamente.
- **RBR-05:** El sistema debe notificar al usuario cuando el libro reservado esté disponible.

### Requisitos funcionales del módulo de reservas

- **RF-01:** El sistema debe permitir al usuario solicitar una reserva desde la ficha del libro.
- **RF-02:** El sistema debe validar que el libro no tenga disponibilidad antes de aceptar la reserva.
- **RF-03:** El sistema debe guardar la fecha y hora exacta de la solicitud.
- **RF-04:** El sistema debe asociar la reserva al usuario autenticado.
- **RF-05:** El sistema debe listar las reservas activas del usuario en su perfil.


