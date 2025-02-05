---
description: Agencia de Publicidad
cover: >-
  https://images.unsplash.com/photo-1631270315847-f418bde47ca6?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw5fHxBZHZlcnRpc2luZ3xlbnwwfHx8fDE3Mzg3ODI1NTd8MA&ixlib=rb-4.0.3&q=85
coverY: -120
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Diccionario de Datos - Ex.10 - Practica

#### <mark style="color:orange;">Ejercicio 10 - Exercise 10</mark>

Spanish:

En una agencia de publicidad, los datos de la orden de publicidad son los siguientes: nro orden, fecha orden, código vendedor, código de medio, tipo de medio, código de cliente o nombre del comprador, texto que publica y según el tipo de medio:

* Para diarios o revistas: nro de página, tamaño, tarifa unitaria, una o varias fechas en las cuales desea publicar. Se supone que para una misma fecha se publica solamente en una página.
* Para televisión o radio: duración, programa o programas que desea, fecha o fechas que desea, horario u horarios en cada programa y tarifa del segundo correspondiente al horario del programa.



English:\
In an advertising agency, the data for a publicity order includes the following: order number, order date, salesperson code, media code, media type, client code or buyer’s name, text to be published, and depending on the media type:

* For newspapers or magazines: page number, size, unit rate, and one or multiple dates for publication. It is assumed that for the same date, the ad will only appear on one page.
* For television or radio: duration, program(s) requested, date(s) requested, time slot(s) within each program, and the per-second rate corresponding to the program’s time slot.

***

<mark style="color:green;">**Solution:**</mark>&#x20;

**Diccionario de Datos:**&#x20;

s: ordenPublicidad = nroOrden + fechaOrden + codigoVendedor + codigoMedio + tipoMedio(d) + \[ codigoCliente | nombreComprador ] + textoPublicacion + \[diarioRevista(e) | televisionRadio (e)\
\
diarioRevista(e) =  nroPagina  + tamaño + tarifaUnitaria + 1{fechasPublicacion}n\
televisionRadio(e) = duracion + \[ programa | programas ] + \[ fecha | fechas ] + \[ horario | horarios ] + tarifa

**Tipo de Evento:** &#x20;
