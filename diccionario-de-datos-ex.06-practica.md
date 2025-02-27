---
description: Socio Videoclub
cover: >-
  https://images.unsplash.com/photo-1711912517564-2aa33854e4d4?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw3fHxCbG9ja2J1c3RlcnxlbnwwfHx8fDE3Mzg3Nzc0ODl8MA&ixlib=rb-4.0.3&q=85
coverY: 0
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

# Diccionario de Datos - Ex.6 - Practica

#### <mark style="color:orange;">Ejercicio 6 - Exercise 6</mark>

Spanish:

Cuando un socio de un Videoclub desea alquilar películas, indica al sistema el no de socio, o si no lo recuerda indicará su nombre, DNI y el nombre de las películas, que por norma establecida en la organización no podrán ser más de tres.

English:

When a member of a Video Club wants to rent movies, they provide the system with their membership number. If they cannot remember it, they will instead provide their name, ID number (DNI), and the titles of the movies, which, according to the organization’s policy, may not exceed three.

***

<mark style="color:green;">**Solution:**</mark>&#x20;

**Diccionario de Datos:**&#x20;

e: alquiler = \[ nroSocio | (nombre\[e] + tipoDocumento(d) + nroDocumento) ] + 1{nombrePelicula}3 \
tipoDocumento(d) = char(3); \[DNI | DU | PAS | LE | LC]\
nombre(e) = nombre + (segundoNombre) + apellido

**Tipo de Evento:** Evento Externo\


