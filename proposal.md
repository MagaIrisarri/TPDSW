<img width="801" height="1011" alt="DER Estacionamiento drawio" src="https://github.com/user-attachments/assets/d4d67209-29b7-4e43-96c8-fbce15d84451" />
# Propuesta TP DSW Estacionamiento COM 301 

## Grupo
### Integrantes
* 52218 - Irisarri, Magalí
* 49781 - Schultz, Valentino
* 49737 - Nagel, Mateo
* 53485 - Lopez, Ariana

### Repositorios
* [frontend app](http://hyperlinkToGihubOrGitlab)
* [backend app](http://hyperlinkToGihubOrGitlab)


## Tema
### Descripción
Para facilitar el uso de cocheras, se busca desarrollar un sistema de reservas físicas y/o virtuales en tiempo real, el cual se base en la disponibilidad de cada cochera adherida, tarifas competitivas y experiencia del usuario.

### Modelo 
Imagen del Modelo de Dominio

<img width="777" height="1111" alt="TP-Página-1 (2)" src="https://github.com/user-attachments/assets/ebe3a67e-749a-4611-996b-91b13ac2ff00" />
Imagen del Diagrama Entidad Relacion

<img width="801" height="1011" alt="DER Estacionamiento drawio" src="https://github.com/user-attachments/assets/2fe869a7-23a2-4773-af8a-57691f007dcc" />

Link Modelos: https://app.diagrams.net/#G1kRBE9HilBemvbzsCnU2Gn20DMTaYp1sV#%7B%22pageId%22%3A%22nEvc5FtAkqEsQDL0Pzc8%22%7D
## Alcance Funcional 

### Alcance Mínimo


Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Usuario<br>2. CRUD Estacionamiento<br>3. CRUD Servicio<br>4. CRUD TipoVehículo|
|CRUD dependiente|1. CRUD Vehículo {depende de} CRUD TipoVehículo<br>2. CRUD Ubicacion_playa {depende de} CRUD Estacionamiento|
|Listado<br>+<br>detalle| 1. Listado de Estacionamiento filtrado por localidad, muestra direccion => detalla Ubicacion_playa<br> 2. Listado de reservas filtrado por fecha, muestra cod_reserva y monto => detalle cliente|
|CUU/Epic|1. Reservar un estacionamiento<br>2. Registrar facturacion de la estadia|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Usuario<br>2. CRUD Estacionamiento<br>3. CRUD Servicio<br>4. CRUD TipoVehículo<br>5. CRUD Vehículo<br>6. CRUD Ubicacion_playa<br>7. CRUD TurnoEmpleado<br>8. CRUD Factura<br>9. CRUD PrecioVehículoHora<br>10. CRUD PrecioServicio|
|CUU/Epic|1. Reservar un estacionamiento<br>2. Registrar confirmacion de reserva<br>3. Realizar facturacion de la estadia<br>4.Registrar uso de un servicio|


### Alcance Adicional Voluntario


|Req|Detalle|
|:-|:-|
|Listados |1. Listado de vehículos filtrado por tipo muestra patente, marca, modelo y seguro => detalle cliente<br>2. Resumen mensual de Reserva filtrado por estado muestra codigo de reserva, tipo_reserva, fecha (desde y hasta) y monto neto|
|CUU/Epic|1. Cancelación de reserva|
|Otros|1. Envío de recordatorio de reserva por email|
