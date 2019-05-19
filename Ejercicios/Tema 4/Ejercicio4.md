# Ejercicio 4

## Enunciado

Buscar información sobre los métodos de balanceo que implementan los dispositivos recogidos en el ejercicio 4.2 (o el software que hemos propuesto para la práctica 3).

## Solución

### HaProxy

HAProxy es un software que nos permite balancear carga entre varios servidores. Se suele usar para balancear servicios web, pero puede balancear cualquier servicio que funcione bajo protocolo TCP. Es necesario entender que por debajo de HTTP está el protocolo TCP y a nivel de TCP se habla de puertos, que sirven para identiﬁcar servicios en una misma máquina. Por debajo de TCP está el protocolo IP y a nivel del protocolo IP se habla de números de IP, que sirven para diferenciar máquinas en Internet.

### nginx 

El balanceo de carga es una excelente manera de escalar su aplicación y aumentar su rendimiento y redundancia. Nginx, que es un popular software para servir servicio web, puede configurarse como un simple pero potente balanceador de carga para mejorar la disponibilidad y eficiencia de sus servidores. En una configuración de balanceo de carga, nginx actúa como un punto de entrada único para una aplicación web distribuida que funciona en varios servidores separados.