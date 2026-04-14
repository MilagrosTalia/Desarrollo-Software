# Propuesta TP DSW

## Grupo
### Integrantes
* 51406 - Talia, Milagros Soledad
* 51120 - Etchecopar , Olivia

### Repositorio

https://github.com/MilagrosTalia/Desarrollo-Software

## Tema
### Descripción
Trabajaremos con el complejo 'La Tomasa', ofrece 7 cabañas con distintas capacidades. Los clientes pueden reservar una cabaña abonando una seña y opcionalmente contratar servicios adicionales como desayuno o servicio de mucama
(los precios se pueden actulizar).Nuestro objetivo es gestionar la reserva desde su creación hasta el pago final, descontando la seña abonada y sumando los servicios contratados. El sistema debe controlar que no se superpongan reservas para
una misma cabaña en las mismas fechas...

### Modelo
<img width="845" height="516" alt="image" src="https://github.com/user-attachments/assets/b5cc035e-83d1-420d-b3b8-224f80d22d55" />

## Alcance Funcional 

### Alcance Mínimo

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Cabañas<br>2. CRUD Servicio<br>
|CRUD dependiente|1. CRUD Precio Servicios {depende de} CRUD Servicios <br>
|Listado<br>+<br>detalle| 1. Listado de reservas filtrado por rango de fecha, muestra la cabaña, fecha inicio y fin estadía, estado y nombre del cliente. 
|CUU/Epic|1. Reservar una cabaña

Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Clientes <br>2. CRUD Estado Reserva<br>3. CRUD Pagos <br>
|CUU/Epic|1. Realizar facturación de estadía y servicios|


### Alcance Adicional Voluntario - PENDIENTE

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.
