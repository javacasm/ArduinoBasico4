# Minicurso Bitbloq

## Introducción a la programacion con bitbloq: 
[[vídeo]](http://youtu.be/3hqwEtsN-Wk) [[ejemplo Parpadeo]](./ejemplosBitbloq/parpadeo.xml)

Bitbloq es un entorno de programación visual por bloques que nos permite programar nuestra placa arduino o compatible de forma sencilla, evitando la complejidad de las sentencias C++

Además nos permite programar nuestro arduino sin instalar (practicamente) nada en nuestro ordenador


### Ver código C++ de un programa bitbloq:  
[[vídeo]](http://youtu.be/lqEB5Pv8JUs) 

Desde bitbloq siempre podemos ver el codigo Arduino generado. De momento no podemos modificar este código pero si copiarlo y llevarlo al IDE de arduino


### Transfiriendo el programa bitbloq a Arduino 
[[vídeo]](http://youtu.be/OZV2lG3xl18) 

Bitbloq nos permite programar nuestro arduino sin instalar (practicamente) nada en nuestro ordenador. Sólo tenemos que pulsar sobre el botón cargar lo que hace que se compile el código, se detecte la placa y se envíe el programa a naestro Arduino


Para aprender las funciones de pin en bitbloq  
[[vídeo]](http://youtu.be/zKs0-vwoxMM) 

Las funciones de pin son las distintas formas que tenemos de manejar los pines de arduino. Tenemos las mismas sentencias que en arduino (en el menú Funciones de Pin): DigitalWrite, AnalogWrite, DigitalRead y AnalogRead. También podemos usarlas si utilizamos un bloque ZUM o octopus correspondiente.

## Sentencias de control

### Bucle **for**
[[vídeo]](http://youtu.be/0Af8VdF6h24) [[ejemplo]](./ejemplosBitbloq/bucle_for.xml)

El bucle **for** permite repetir un conjunto de pasos un número de veces determinado. 
Necesitamos  declarar una variables que actuará como contador y definir el valor inicial que tendrá la variable y el final, realizándose tantos como pasos como valores enteros haya entre ambas.

### Bucle **while** 
[[vídeo]](http://youtu.be/894D9hV8paw) [[ejemplo]](./ejemplosBitbloq/bucle_while.xml)

Usaremos la sentencia de control **while** para los bucles donde el número de veces que se repite no está definido desde el principio

### Bloque **if** : sentencias condicionales
[[vídeo]](http://youtu.be/dXpDCOzsO2U) [[ejemplo]](./ejemplosBitbloq/condicional.xml)

Las sentencias condicionales permiten ejecutar un código y otro según se cumpla o no una determinada condición. Esta condición será una validación que definiremos con operandos.

Podemos hacer que en caso de que se cumpla se ejecute un código (es el bloque if) y en caso de que no se cumpla la condición se ejecute otro (bloque else)

### Sentencias condicionales complejas
[[vídeo]](http://youtu.be/en_Y-_wVyO0) [[ejemplo]](./ejemplosBitbloq/condiciones_if.xml)

La condición que determina si se ejecuta un bloque u otro o si salimos de un bloque while puede contener varias comprobaciones. 

Entre estas condiciones utilizaremos operadores lógicos que pueden ser AND o OR

* Estas condiciones se tendrán que cumplir todas en el caso del operador AND

* Con que se cumpla una de elllas se dará por válida toda la condición


## Envío de datos al PC: 
[[vídeo]](http://youtu.be/uAy_reYl8_Y) [[ejemplo]](./ejemplosBitbloq/Serial.xml) 

Podemos enviar contenidos entre nuestra placa y el PC usando las sentencias de comunicaciones. Usaremos print para enviar algo (puede ser el valor de una variable o un texto) al pc o println para enviar y pasar a la siguiente línea.


tag bitbloq, arduino, programación
