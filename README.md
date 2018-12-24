# HowtoConectRL
Guía basica para conectarse al  server de RadioLibre por medio de IDJC(Internet Dee Jay Console). 

La idea de este documento es dar una ruta para transmitir audio por radiolibre.co

Lo primero es instalar los requerimientos de software.

Requerimientos 

Jack / Qjackctl / IDJC

Jack es un controlador de audio para linux

Qjackctl es una interfaz grafica para el server de Jack 

Internet Dee Jay Console es un software para el control de sonido tipo DJ en linux 

Los comandos para instalar las dependencias necesarias 

sudo apt-get install jackd 

sudo apt-get install idjc 

sudo apt-get install qjackctl 


Lo primero que debemos hacer para iniciar este bproceso es activar el servidor de jack, en este caso por medio de la interfaz grafica Qjackctl, ejecutamos qjackctl en terminal y luego prersionamos el boton iniciar, así activas el servidor de jack (debes de revisar cual es tu tarjeta  de salida en la ventana de configuración por lo general es la defaulut).

después de tener el server de jack activo  corres tu software.

Luego de esto abrimos el Internet DJ Console.

Puedes ejecutar en terminal idjc o buscarlo en la seccion de multimedia de ti menu

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


