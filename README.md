# flow4
Este repositorio contiene el flow 4 del curso de NodeRed, visto en en los contenidos de Internet de las cosas de Codigo IoT en edu.codigoiot.com
## Introducción 

Este flow consiste en un tablero que presente la información de temperatura y humedad locales. Este flow recibe la información por MQTT con un broker local.

## Material Necesario

Para realizar el flow 1 sera necesario lo siguiente:

- [Ubuntu20.04 ](https://releases.ubuntu.com/20.04/)
- [NodeJS](https://nodejs.org/es/)
- [NPM](https://www.npmjs.com/)
- [NodeRed](https://nodered.org/docs/getting-started/local)

## Material de Referencia

A continuación podras puedes encontrar los enlaces a cursos de la plataforma de edu.codigoiot.com con ellos podras realizar las configuraciones necesarias

- [Instalación de Virutal Box y Ubuntu 20.04](https://edu.codigoiot.com/course/view.php?id=812)
- [Instalación de NodeRed](https://edu.codigoiot.com/enrol/index.php?id=817)
- [Introducción a NodeRed](https://edu.codigoiot.com/enrol/index.php?id=278)

## Instrucciones

### Requisitos previos
Para que el flow-4 funcione de manera adecuada se debe cumplir con los siguientes requisitos:

1.- Instalación de NodeJS: Se recomienda tener instalado NodeJS en alguna versión LTS. Para la creación de este Flow se usó la versión 16.17.0LTS. Esta instalación debe incluir las Build-Tools para hacer uso de NPM

2.- Instalación de NodeRed: La instalación se realiza por NPM. Al momento de la creación de este documento se usó la versión 3.0.2
3.- Instalar los nodos node-red-dashboard. Para ello, dirigete a la opcion "Manage Palet" de NodeRed y en la pestaña Install busca node-red-dashboard. Finalmente haz clic en instalar.

4.- Instalación de Broker local Mosquitto MQTT.

### Instrucciones de preparación del entorno
Para ejecutar este flujo, es necesario lo siguiente:

1.-Arrancar NodeRed (usando el comando "node-red" en nuestra terminal)
2.-Importar el flujo desde el repositorio
3.-Hacer clic en el boton Deploy


### Instrucciones de operacion
- Para poder visualizar el resultado de este flujo, sólo necesitas abrir la pestaña Debug.
- Enviar por MQTT un mensaje que contenga un JSON con las variables ID, temp y hum-

### Notas

- Este Flow se suscribe al tema codigoIoT/Mor/mqtt/flow4
- El mensaje mqtt usado para probar este flow es mosquitto_pub -h localhost -t codigoIoT/Mor/mqtt/flow4 -m '{"ID":"Frida","temp":18,"hum":78}'
- Para que la gráfica historica muestre información, deben enviarse al menos 2 puntos

### Resultados 
En la siguiente imagen se puede ver los nodos
![](https://github.com/Fridaa-Andrade/flow4/blob/main/flow4-nodos.jpeg)

En la siguiente imagen se puede ver el tablero
![](https://github.com/Fridaa-Andrade/flow4/blob/main/Flow4-tablero.jpeg)
## Evidencias

## Créditos
