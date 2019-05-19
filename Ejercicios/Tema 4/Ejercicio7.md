# Ejercicio 7

## Enunciado

Buscar información sobre métodos y herramientas para implementar GSLB.

## Solución

Hoy en día, la alta disponibilidad de los servicios de TI es una necesidad y esa es la razón por la que las empresas y organizaciones desarrollan sistemas informáticos distribuidos en todo el mundo y hospedan servicios en más de un Centro de Datos, ya que ofrece los siguientes beneficios:
- Tolerancia a fallos: cuando el servicio alojado en el centro de datos falla, el servicio continúa en cualquiera de los otros sitios disponibles.
- Recuperación automática del centro de datos: cuando un centro de datos falla, el servicio se redirige automáticamente a cualquier otro centro de datos disponible.
- Balanceo de carga: el tráfico podría optimizarse distribuyendo la carga entre todos los sitios disponibles, mejorando la latencia y agilizando la entrega del servicio.
- Latencia mejorada: el tráfico de la aplicación cliente es directamente con el servidor real, sin necesidad de pasar todos los datos de la aplicación a través del equilibrador de carga.

Las herramientas que podemos utilizar son los propios servidores web, si tienen opción de balanceo de carga, por ello GSBL podría ser implementado por el propio nginx o haproxy.

