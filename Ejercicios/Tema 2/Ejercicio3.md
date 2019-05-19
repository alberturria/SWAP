# Ejercicio 3

## Enunciado

¿Cómo analizar el nivel de carga de cada uno de los subsistemas en el servidor? Buscar herramientas y aprender a usarlas.

## Solución

### PM2

Pm2 es una librería de NodeJS que nos permite monitorizar nuestra aplicación.
Además, al trabajar con clústeres, permite a nuestra aplicación ser fácilmente escalable.

### forever

forever es una librería para NodeJS que nos permite lanzar nuestra aplicación durante un tiempo indefinido.
Es de gran utilidad a la hora de realizar despliegues, por ejemplo, en máquinas virtuales de Azure.

### PyClustering

PyClustering es una librería de Python que nos permite trabajar con clústeres. Aunque no podamos aumentar directamente el número de clúster de la aplicación lanzada, sí podríamos hacer un pequeño programa que se encargase de lanzar nuestra aplicación, e ir ofreciéndole un número mayor de clústeres conforme sea necesario.