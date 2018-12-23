# HowtoConectRL
Guía basica para conectarse al  server de RadioLibre


La idea de este documento es dar una  ruta de como transmitir audio por radiolibre.co

Lo primero es instalar los requerimientos.

Requerimientos 

Jack / Qjackctl / IDJC

sudo apt-get install idjc

sudo apt-get install idjc 

sudo apt-get install qjackctl 

sudo apt-get install jackd 

Lo primero es activar el servidor  de jack por medio de la interfaz grafica Qjackctl,  prersionando el boton iniciar activas el servidor de jack.

En este paso activas tu software en mi caso Supercollider y FoxDot 

Luego de esto abrimos el Internet DJ Console 

Teniendo IDJC abierto vamos a la interfaz de Qjack y abrimos la pestaña de conexiones, allí observamos que en la parte de IN y OUT 
esta super collider e IDJC ahì a forma de patch conectamos el OUT de Supercollider con el IN de Idjc.


![1](https://github.com/Noisk8/HowtoConectRL/blob/master/SCIDE%20CONECTADO%20CON%20IDJC.png)

las conexiones en jack ....

output_1 pe_in_l  
output_2 pe_in_r


Para configurar el idjc al servidor 

Vamos a la pestaña de Ver → Salida → Configuración 

Ahora nos paramos sobre 
![2](https://github.com/Noisk8/HowtoConectRL/blob/master/VER-SALIDA%20IDJC.png)


Ahí le damos en Nuevo y empezamos a generar la configuración, damos click en nuevo.

![3](https://github.com/Noisk8/HowtoConectRL/blob/master/NUEVO%20IDJC.png)

Rllenamos la configuración con la información que se ve en la imagen 

![]()
luego vamos a la pestaña de formato y configuramos el formato de salida de la transmisión

![]()

ahora activamos el canal y conectamos 

![]()

![]()


