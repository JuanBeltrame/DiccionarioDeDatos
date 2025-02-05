# Diccionario de Datos - Ex.6 - Practica

#### <mark style="color:orange;">Ejercicio 6 - Exercise 6</mark>

***

Spanish:

Cuando un socio de un Videoclub desea alquilar películas, indica al sistema el no de socio, o si no lo recuerda indicará su nombre, DNI y el nombre de las películas, que por norma establecida en la organización no podrán ser más de tres.

English:

When a member of a Video Club wants to rent movies, they provide the system with their membership number. If they cannot remember it, they will instead provide their name, ID number (DNI), and the titles of the movies, which, according to the organization’s policy, may not exceed three.

***

<mark style="color:green;">**Solution:**</mark>&#x20;

e: Alquiler = \[ nroSocio | (nombre\[e] + tipoDocumento(d) + nroDocumento) ] + 1{nombrePelicula}3 \
tipoDocumento(d) = char(3); \[DNI | DU | PAS | LE | LC]\
nombre(e) = nombre + (segundoNombre) + apellido

***

Tipo de Evento: Evento Externo\
\


