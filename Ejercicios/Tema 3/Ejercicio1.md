# Ejercicio 1

## Enunciado

Buscar con qué órdenes de terminal o herramientas podemos configurar bajo Windows y bajo Linux el enrutamiento del tráfico de un servidor para pasar el tráfico desde una subred a otra.

## Solución

### Linux

En Linux podremos dirigir el tráfico de nuestro servidor con el comando `route`, y podremos añadir rutas con `add` o eliminarlas con `del`. 

Además podemos restringir el tráfico con `ufw`, o con `iptables`.

### Windows

En Windows podemos hacer uso del monitor de recursos de red que viene por defecto. Si no queremos este, siempre podremos instalar software de terceros como 'LiveTcpUdpWatch'.