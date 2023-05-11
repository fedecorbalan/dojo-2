# dojo-2
Alumno: Federico Corbalán

Integrantes: Federico Corbalán, Ramon Bautista Escalante, Leandro Escobar Perez, Lucas Figueroa

La empresa  “UTN FRA Robotics” ganó la licitación de un proyecto, y deberá Implementar un sistema que permita al usuario saber a qué estación de subte está llegando, aparte  el sistema muestra las estaciones que faltan hasta llegar a destino, para ello debemos utilizar 4 LEDs y el display de 7 segmentos. Esta vez el buzzer deberá emitir un sonido diferente cada vez que se llegue a una estación.
El sistema deberá arrancar apagado, luego de presionar el botón empezará y hará lo pedido.

![image](https://github.com/fedecorbalan/dojo-2/assets/123754871/399d1e32-9b73-431f-a5db-2874c056b0cf)

y para su correcto funcionamiento, se programo con el siguiente codigo:

# Definiciones
Se definen los siguientes elementos que se van a utilizar junto con sus respectivos pines

![image](https://github.com/fedecorbalan/dojo-2/assets/123754871/66f601ad-94cb-4369-a4b8-f61553663652)
![image](https://github.com/fedecorbalan/dojo-2/assets/123754871/567bd053-0e68-4279-bb6d-d2cef0cc34c3)



# Funcion Principal

![image](https://github.com/fedecorbalan/dojo-2/assets/123754871/2c7e64b5-f85e-485b-97a2-620bf016fadc)

En el loop, se declara la variable pulsador que contiene la lectura del pin del mismo y si al presionarlo, devuelve 1023, se ejecutan las funciones EncenderEstacion a los cuales se les ingresa por parametro el led en donde se quiere ejecutar y el tiempo de delay que se busca.

# Buzzer
Se le ingresa por parametro el pin en donde se encuentra el buzzer y se utiliza la funcion tone, a la que se le ingresa, el pin, la frecuencia de sonido y el delay.

![image](https://github.com/fedecorbalan/dojo-2/assets/123754871/3cea508f-ebb7-443e-a1d8-08f9995ce210)

# Encender Estacion
A esta funcion se le ingresa por parametro el led que se quiere prender y el tiempo en el que tarde en prenderse y apagarse, y dentro de la funcion se hace un switch de los led y en base al led que se haya ingresado, este se va a prender y apagar en el tiempo pasado por parametro. Y ademas en el medio, se utiliza la funcion Encender Display, que imprime en el display de 7 segmentos un numero del 0 al 9

![image](https://github.com/fedecorbalan/dojo-2/assets/123754871/4fd29c55-cceb-418d-96b5-768d11cac7b5)

# Encender Display
Esta funcion muestra en el display de 7 segmentos, un numero ingresado por parametro del 0 al 9, se recorre con un switch.
![image](https://github.com/fedecorbalan/dojo-2/assets/123754871/b9a30d4b-6795-4aec-bcd5-10fe1042c047)

# Link al proyecto 

https://www.tinkercad.com/things/dZIaGhdQoVs
