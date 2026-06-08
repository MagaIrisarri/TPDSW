

# Propuesta TP DSW Estacionamiento COM 301 

## Grupo
### Integrantes
* 52218 - Irisarri, Magalí
* 49781 - Schultz, Valentino
* 49737 - Nagel, Mateo
* 53485 - Lopez, Ariana

### Repositorios
* [frontend app](http://hyperlinkToGihubOrGitlab)
* [backend app](https://github.com/MagaIrisarri/Backend)


## Tema
### Descripción
Para facilitar el uso de cocheras, se busca desarrollar un sistema de reservas físicas y/o virtuales en tiempo real, el cual se base en la disponibilidad de cada cochera adherida, tarifas competitivas y experiencia del usuario.

### Modelo 
Imagen del Modelo de Dominio

<img width="760" height="1110" alt="TP-MD drawio" src="https://github.com/user-attachments/assets/3c4a0da5-300e-471f-8d88-c0f971891a65" />

Imagen del Diagrama Entidad Relacion

<img width="1013" height="952" alt="TP-DER drawio" src="https://github.com/user-attachments/assets/64423e12-e9b5-4217-b01e-d43fbf29f12e" />


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
|CRUD |1. CRUD Usuario<br>2. CRUD Estacionamiento<br>3. CRUD Servicio<br>4. CRUD TipoVehículo<br>5. CRUD Vehículo<br>6. CRUD Ubicacion_playa<br>7. CRUD TurnoEmpleado<br>8. CRUD PrecioVehículoHora<br>9. CRUD PrecioServicio|
|CUU/Epic|1. Reservar un estacionamiento<br>2. Registrar confirmacion de reserva<br>3. Realizar facturacion de la estadia<br>4.Registrar uso de un servicio|


### Alcance Adicional Voluntario


|Req|Detalle|
|:-|:-|
|Listados |1. Listado de vehículos filtrado por tipo muestra patente, marca, modelo y seguro => detalle cliente<br>2. Resumen mensual de Reserva filtrado por estado muestra codigo de reserva, tipo_reserva, fecha (desde y hasta) y monto neto|
|CUU/Epic|1. Cancelación de reserva|
|Otros|1. Envío de recordatorio de reserva por email|
