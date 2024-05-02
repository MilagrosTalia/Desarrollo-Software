# Desarrollo-Software
Aplicación Web Full Stack 

Integrantes:
De Carlos, David - 51482
// Ferramondo, Pedro - 50385
// Ferraris, Manuel - 51937
// Talia, Milagros - 51406

Minuta de Relevamiento N° 1

Tema: Relevamiento inicial

Fecha: 05/04/2024

Participantes: Encargado de Peluquería (EP), Cliente (CLI), Peluquero (PE), Peluquero a domicilio (PD).

La empresa objeto de nuestro trabajo brinda servicio de peluquería y venta de productos capilares y cosméticos. Se desea construir un sistema para controlar: la gestión de turnos y venta de productos.

_Descripción del negocio. _

Cuando una persona o cliente (CLI) necesita obtener un turno para la peluquería ingresa a la página web, en caso de no estar registrado el sistema solicita los datos al cliente (DNI, nombre y apellido, mail, dirección y teléfono). Una vez que el cliente está logueado ingresa los datos del turno:

fecha-desde: Se ingresa día en el calendario proporcionado por el sistema.

fecha-hasta: Se ingresa día en el calendario proporcionado por el sistema.

tipo-turno: Admite dos tipos de modalidades (domicilio/sucursal), en caso de ser un corte a domicilio se le cobrará un 25% más.

En base a los datos ingresados el sistema verifica los horarios y días disponibles, el CLI lo reserva y el sistema actualiza el estado del turno reservado ( Los turnos se encuentran codificados poseen fecha, hora.). En caso de que el cliente decida modificar o cancelar el turno lo deberá hacer con 24 horas de anticipación.

RN1: En caso de que el cliente no asista al corte en sucursal, se le aplica una tarifa del 25% al próximo servicio que solicite el cliente.El EP actualiza estado de turno a “Ausente” y actualiza el estado de cobro a “Pendiente”.

RN2: En caso de que el cliente no asista al corte a domicilio, se le aplica una tarifa del 50% al próximo servicio que solicite el cliente. El PD actualiza el estado de turno a “Ausente” y actualiza el estado de cobro a “Pendiente”.

RN3:  Cada peluquero cuenta con un numero que lo identifica, además posee una descripción con el tipo de servicio al cual se dedica (domicilio - local).

Llegada la fecha del turno el CLI se presenta a la peluquería y es recibido por el EP. Una vez realizado el corte, el cliente le indica al EP el medio de pago, puede hacerlo en efectivo o por MercadoPago. Luego que el EP realiza el cobro, se actualiza el estado del cobro a “Abonado”.

El PE atiende al CLI el EP actualiza el estado del turno (Atendido) en el sistema.

RN4: Los estados de turno posibles son (Libre/reservado/Atendido/Ausente).

RN5: Los estados de cobro posibles son (Pendiente/Abonado).

En caso de que el tipo de turno sea a domicilio el PD a cargo de este turno se dirige hacia el domicilio asignado. Es recibido por el cliente, verifica el medio de pago seleccionado por este y cobra el importe. Luego de esto el PD realiza el servicio y actualiza el estado de turno y cobro.

El sistema que debemos desarrollar también cuenta con apartado de compras en la página web, donde se muestran los productos capilares y cosméticos disponibles en la peluquería. Un producto se identifica por un número único secuencial. Un producto puede tener una o más presentaciones. Los precios de los artículos dependen de la presentación del mismo.

El cliente selecciona los productos que desea, los agrega al carrito y selecciona el método de pago (MercadoPago), se deberá presentar al local para retirar el pedido. Cuando una persona o cliente (CLI) desea finalizar la compra, [en caso de no estar registrado el sistema solicita los datos al cliente (DNI, Nombre y apellido, mail, dirección y telefono)], el sistema verifica el cobro y descuenta el stock de los productos. El EP prepara el pedido para la posterior entrega del cliente.

Posibles extensiones: /*Asignar turno por peluquero. Asignar turnos por sucursales. Realizar seña de turno. Realizar compra sin estar logueado. */

Siguiente entrega: CRUD PE.
