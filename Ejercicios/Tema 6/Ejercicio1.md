# Ejercicio 1

## Enunciado

Aplicar con iptables una política de denegar todo el tráfico en una de las máquinas de prácticas. 
Comprobar el funcionamiento.
Aplicar con iptables una política de permitir todo el tráfico en una de las máquinas de prácticas.
Comprobar el funcionamiento.

## Solución

### Denegar todo el tráfico

```
iptables -P INPUT DROP
iptables -P OUTPUT DROP
iptables -P FORWARD DROP

```

Una de las consecuencias de aplicar estas reglas, es el no poder establecer conexión por ssh.

### Aceptar todo el tráfico

```
iptables -P INPUT -j ACCEPT

```

El resultado de esta sentencia es que nuestra máquina se encuentra totalmente expuesta a cualquier intento de conexión.
