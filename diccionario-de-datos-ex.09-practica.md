---
description: Resumen de Gastos
cover: >-
  https://images.unsplash.com/photo-1649209979970-f01d950cc5ed?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw2fHxpbnZvaWNlfGVufDB8fHx8MTczODc3OTc1Nnww&ixlib=rb-4.0.3&q=85
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

# Diccionario de Datos - Ex.9 - Practica

#### <mark style="color:orange;">Ejercicio 9 - Exercise 9</mark>

Spanish:

El sistema deberá generar el último día hábil de cada mes un resumen de los gastos ocurridos durante el mes, clasificado por tipo de gasto (existen 3 tipos: comerciales, administrativos y de producción), y dentro de éstos, totalizar los gastos por quincena, importe mensual por tipo e importe total mensual de los gastos.\


English:\
The system must generate, on the last business day of each month, a summary of the expenses incurred during the month, classified by expense type (there are 3 types: commercial, administrative, and production). Within these categories, it must total the expenses by fortnight (two-week period), provide the monthly amount per type, and calculate the total monthly amount of expenses.

***

<mark style="color:green;">**Solution:**</mark>&#x20;

**Diccionario de Datos:** \
s: resumenGastos = fechaInforme +  1{tipoDeGasto(d)}3\
\
tipoDeGasto(d) = \[ comercial(e) | {administrativo(e) | produccion(e) ] \
\
comercial(e) = 1{gastoQuincena}2 + gastoMensual \
administrativo(e) = 1{gastoQuincena}2 + gastoMensual \
produccion(e) = 1{gastoQuincena}2 + gastoMensual \
&#x20;

**Tipo de Evento:** Evento Temporal.
