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

SuperCollider output_1 -------- pe_in_l    IDJC 
              output_2 -------- pe_in_r
              
              
              IMAGEN 
  Ahora en IDJC...
            
Para configurar el idjc al servidor 
Vamos a la pestaña de Ver → Salida → Configuración 

Ahí le damos en Nuevo y empezamos a generar la configuración 



Continuara....

