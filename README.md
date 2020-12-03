### Universidad de Costa Rica
#### IE0405 - Modelos Probabilísticos de Señales y Sistemas
---

# `L5` - *Cadenas de Markov*
### Jeffry Luque Aguero 
### B33893
### Grupo_: 02

En el laboratorio 5 se modificó el código dado, con tal de que se cumliera la asignación, es decir que el servidor no esté vacío (sin atender solicitudes) más del 10% del tiempo. Se debe hallar  el parámetro $\nu$ para satisfacer este requisito y modificar el código para medir la variable de interés en una simulación.

Se parte de la ecuación dada en el L5.ipynb, adecuandolo a nuestra situación, que sería con los siguientes datos:


> P como el umbral de personas en el sistema, y p-1 las personas en fila. En nuestro desarrollo tomaremos P = 1

En el documento L5.ipynb, sección de solución, vimos que nuestro v debe ser mayor o igual a 2.10.

> Para nuestro ejemplo y solución tomaremos el valor de v = 2.15.

Se realizan los siguientes cambios en el código: 
#### Parámetro de servicio (servicios/segundos)
>nu = 2.15/60

Además se realizó un cambio importante en el código, ya que debemos velar que el 90% del tiempo haya una solicitud
>fraccion = frecuencia / len(t)
if fraccion >= 0.9:  # El resultado debe ser mayor al 90%
---

Por ultimo en la sección de solución, en el resultado del código se detallan los datos obtenidos, teniendo coherencia con lo esperado:

>
Tiempo con más de -1 solicitudes en fila:
	 91.24%
	 Sí cumple con la especificación.
Simulación es equivalente a 8.28 horas.

Concluyendo con la asignación planteada
