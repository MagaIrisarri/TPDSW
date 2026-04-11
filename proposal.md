# Propuesta TP DSW

## Grupo
### Integrantes
* 52218 - Irisarri, Magalí
* 49781 - Schultz, Valentino
* 49737 - Nagel, Mateo

### Repositorios
* [frontend app](http://hyperlinkToGihubOrGitlab)
* [backend app](http://hyperlinkToGihubOrGitlab)
*Nota*: si utiliza un monorepo indicar un solo link con fullstack app.

## Tema
### Descripción
*Para facilitar el uso de cocheras, se busca desarrollar un sistema de reservas físicas y/o virtuales en tiempo real, el cual se base en la disponibilidad de cada cochera adherida, tarifas competitivas y experiencia del usuario.

### Modelo
![imagen del modelo]()

*Nota*: incluir un link con la imagen de un modelo, puede ser modelo de dominio, diagrama de clases, DER. Si lo prefieren pueden utilizar diagramas con [Mermaid](https://mermaid.js.org) en lugar de imágenes.

## Alcance Funcional 

### Alcance Mínimo

*Nota*: el siguiente es un ejemplo para un grupo de 3 integrantes para un sistema de hotel. El 

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Cliente<br>2. CRUD Estacionamiento<br>3. CRUD Empleado<br>4. CRUD Precio|
|CRUD dependiente|1. CRUD Auto {depende de} CRUD cliente<br>2. CRUD Ubicacion_playa {depende de} CRUD Estacionamiento|
|Listado<br>+<br>detalle| 1. Listado de Estacionamiento filtrado por localidad, muestra direccion => detalla Ubicacion_playa<br> 2. Listado de reservas filtrado por fecha, muestra cod_reserva y monto => detalle cliente|
|CUU/Epic|1. Reservar un estacionamiento<br>2. Registrar facturacion de la estadia|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Cliente<br>2. CRUD Estacionamiento<br>3. CRUD Empliador<br>4. CRUD Precio<br>5. CRUD Auto<br>6. CRUD Ubicacion_playa<br>7. CRUD Reserva<br>7. CRUD Lugares|
|CUU/Epic|1. Reservar un estacionamiento<br>2. Registrar confirmacion de reserva<br>3. Registrar facturacion de la estadia<br>4.Registrar cliente|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Listado de vehículos filtrado por tipo muestra patente, marca, modelo y seguro => detalle cliente<br>2. Resumen mensual de Reserva filtrado por estado muestra codigo de reserva, tipo_reserva, fecha (desde y hasta) y monto neto|
|CUU/Epic|1. Cancelación de reserva|
|Otros|1. Envío de recordatorio de reserva por email|
