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

