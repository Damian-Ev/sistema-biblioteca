# Prototipo: confirmación de reserva

## 1. Objetivo

Describir el flujo y la interfaz del modal de confirmación de reserva de libros del sistema de biblioteca universitaria.

Este modal permitirá al usuario revisar la información del libro seleccionado antes de confirmar o cancelar su reserva.

## 2. Interfaz del modal

El modal aparecerá sobre la pantalla del catálogo de libros y contendrá los siguientes elementos:

- **Título:** Confirmar reserva.
- **Información del libro:** título, autor e ISBN.
- **Mensaje de confirmación:** "¿Deseas confirmar la reserva de este libro?".
- **Botón Confirmar reserva:** permite continuar con la operación.
- **Botón Cancelar:** cierra el modal sin realizar la reserva.

## 3. Flujo de interacción

1. El usuario consulta el catálogo y selecciona un libro.
2. Presiona el botón "Reservar".
3. El sistema muestra el modal con la información del libro seleccionado.
4. El usuario revisa la información y elige una de las siguientes opciones:
   - **Confirmar reserva:** el sistema procesa la solicitud y comprueba si puede realizarse.
   - **Cancelar:** el modal se cierra y el usuario regresa al catálogo sin modificar la información.
5. Si la reserva se realiza correctamente, el sistema muestra un mensaje de confirmación.
6. Si la reserva no puede realizarse, el sistema muestra un mensaje de error explicando el motivo.

## 4. Consideraciones de la interfaz

- El modal deberá mostrar claramente la información del libro.
- Los botones de confirmación y cancelación deberán ser fáciles de identificar.
- Se deberá evitar el envío de solicitudes duplicadas mientras se procesa la reserva.
- Los mensajes de éxito o error deberán ser comprensibles para el usuario.
