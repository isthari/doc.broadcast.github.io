---
title: "HQ Portable"
permalink: /es/hq-portable
excerpt: "HQ PortableI
modified: 2016-04-13T15:54:02-04:00
redirect_from:
  - /theme-setup/
---

{% include base_path %}
Esta sección describe la instalación y configuración de la imagen para la utilización del software en Raspberry PI con pantalla táctil de 3.5" o 7"

El primer paso es descargar la imagen del software en función de la pantalla seleccionada:
* Pantalla de 3.5" [Descarga](https://isthari-hq.s3.amazonaws.com/hq-portable-35-v3.1.2.img)
* Pantalla de 7" [Descarga](https://isthari-hq.s3.amazonaws.com/hq-portable-7-v3.1.2.img)

A continuación es necesario descarga e instalar el software para copiar la imagen a la tarjeta SD [Descargar Balena](https://www.balena.io/etcher/)

Una vez copiada la imagen en la tarjeta extraerla y volver a conectarla al PC. Buscar la unidad "boot" y localizar el archivo data.json

|![](file-browser.png)|
|:--:|
|*Archivo de login data.json*|

Abrirlo con el Notepad e indicar los siguientes campos:
* user: nombre del usuario HQ
* password: Clave del usuario HQ
* remotePassword: Clave para que soporte técnico pueda conectarse remotamente al equipo

|![](data-json.png)|
|:--:|
|*Configurar usuario y clave*|

A continuación insertar la tarjeta en la Raspberry, conectar el micro auricular USB, el cable de red e iniciarla

# Funcionamiento
Una vez iniciado el equipo se mostrará la siguiente pantalla mientras se conecta al servidor

|![Conectando pantalla 3.5"](conectando.png)|
|:--:|
|*Conectando al servidor, pantallas de 3.5" y 7"*|

En caso de no avanzar de esta pantalla puede ser:
* Debido a la falta de conectividad de red. Revisar la conexión del cable. En el conector RJ45 debe estar encendido fijo el Led Naranja y parpader el Led verde
* El usuario y contraseña configurados pueden no ser correctos

Una vez conectado al servidor, solicitará pulsar en la pantalla para iniciar la aplicación

|![](pulse-iniciar.png)|
|:--:|
|*Inicio pantallas de 3.5" o 7"*|

El usuario ya se encuentra conectado y esperando una llamada

|![](esperando.png)|
|:--:|
|*Esperando llamada, pantalla 3.5"*|

|![](esperando-7.png)|
|:--:|
|*Esperando llamada, pantalla 7"*|

Una vez que recibe una llamada el estado cambiará a "Conectado". 
Se indicará el nombre del usuario remoto "admin" en este ejemplo.
Y se podrán ver los vúmetros de Rx y Tx

|![](conectado.png)|
|:--:|
|*Conectada llamada, pantalla 3.5"*|

|![](conectado-7.png)|
|:--:|
|*Conectada llamada, pantalla 7"*|
