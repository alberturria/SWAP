# Ejercicio 1

## Enunciado

Calcular la disponibilidad del sistema si tenemos dos réplicas de cada elemento (en total 3 elementos en cada subsistema).

### Con 1 elemento cada subsistema 

Web -> 85%
Application -> 90%
Database -> 99.9%
DNS -> 98%
Firewall -> 85%
Switch -> 99%
Data Center -> 99.99%
ISP -> 95%


### Con 2 elementos cada subsistema 

Web -> 97.75%
Application -> 99%
Database -> 99.9999%
DNS -> 99.96%
Firewall -> 97.75%
Switch -> 99.99%
Data Center -> 99.99%
ISP -> 99.75%

## Solución

Web -> 0.9775 + (1-0.9775)*0.85 = 99.6625%
Application -> 0.99 + (1-0.99)*0.90 = 99.9%
Database -> 0.999999 + (1-0.999999)*0.999 = 99.9999%
DNS -> 0.9996 + (1-0.9996)*0.999 = 99.6392%
Firewall -> 0.9775 + (1-0.9775)*0.85 = 99.6625%
Switch -> 0.9999 + (1-0.9999)*0.99 = 99.9999%
Data Center -> 0.9999 + (1-0.9999)*0.9999 = 99.999999%
ISP -> 0.9975 + (1-0.9975)*0.95 = 99.9875%

Disponibilidad total = 0.996625 * 0.999 * 0.999999 * 0.996392 * 0.996625 * 0.999999 * 0.99999999 * 0.999875 = 0.98856