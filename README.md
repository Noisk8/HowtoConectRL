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

esto para que la señal que este saliendo desde nuestro soft en mi caso foxdot(supercollider) llegue al idjc

output_1 pe_in_l  
output_2 pe_in_r


Para configurar el idjc al servidor 

Vamos a la pestaña de Ver → Salida → Configuración 

Ahora nos paramos sobre 
![2](https://github.com/Noisk8/HowtoConectRL/blob/master/VER-SALIDA%20IDJC.png)


Ahí le damos en Nuevo y empezamos a generar la configuración, damos click en nuevo.

![3](https://github.com/Noisk8/HowtoConectRL/blob/master/NUEVO%20IDJC.png)

Rllenamos la configuración con la información que se ve en la imagen 

![4](https://github.com/Noisk8/HowtoConectRL/blob/master/SETINGS%20CONECT.png)
luego vamos a la pestaña de formato y configuramos el formato de salida de la transmisión

![5](https://github.com/Noisk8/HowtoConectRL/blob/master/FORMATO%20SALIDA%202.png)
Con el el boton de siguiente señalado en la imagen vamos setiando los items hasta que llegueos al final y todos queden con el boton verde.


![6](https://github.com/Noisk8/HowtoConectRL/blob/master/CONTROLES%201.png)

ahora activamos el canal y conectamos, como ves en la parte superior hay varios puntitos con un numero, eso son los canales, como estamos setiando el no 1  lo activamos y le clickeamos encima y ae pone la flecha 

![7](https://github.com/Noisk8/HowtoConectRL/blob/master/LISTERINE.png)

Ahora clikeamos en conectar  y  vemos que el botoncito verde de el canal uno se pone amarillo y luego en verde, eso significa que ya estas saliendo por RL  :)


