# Ejercicio 3

## Enunciado

Implementar un pequeño servicio web en los servidores finales que devuelva el % CPU y % RAM que en un instante tiene en uso dicho servidor.
Lo debe devolver como una cadena de texto plano que representa ambos porcentajes, p.ej: “CPU 45% RAM 76%”

## Solución

Esta es la salida que nos ofrece el script.

![Funcionamiento de script](./assets/scriptsh.png)

El contenido del script es el siguiente: 
```
#!/bin/sh
free -m | awk 'NR==2{printf "Memory Usage: %s/%sMB (%.2f%%)\n", $3,$2,$3*100/$2 }'
df -h | awk '$NF=="/"{printf "Disk Usage: %d/%dGB (%s)\n", $3,$2,$5}'
top -bn1 | grep load | awk '{printf "CPU Load: %.2f\n", $(NF-2)}'
```