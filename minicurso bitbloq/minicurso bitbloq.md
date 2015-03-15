# Minicurso Bitbloq

Bitbloq es un entorno de programación visual que nos permite crear programas para Arduino y placas compatibles y transferir los mismos a las placas de una forma sencilla. 

Podemos acceder directamente desde su web  http://bitbloq.bq.com/
(En los vídeo se usa la versión beta http://beta-bitbloq.bq.com/, que en breve será la versión estable, ya que mejora mucho la gestión de las conexiones con las placas)

Como verás cuando entres a su página, funciona con Chrome en todos los sistemas operativos, y el se encarga de avisarte si necesitas drivers o cambiar algo en tu sistema

A lo largo de estos vídeos veremos algunas de sus características más importantes. Puedes encontrar más tutoriales en la página [oficial de bitbloq](http://diwo.bq.com/tag/bitbloq/)



## Introducción a la programacion con bitbloq: 
[[vídeo]](http://youtu.be/3hqwEtsN-Wk) [[ejemplo Parpadeo]](./ejemplosBitbloq/parpadeo.xml)

![parpadeo](./ejemplosBitbloq/Parpadeo.png)

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

![bucle for](./ejemplosBitbloq/Bucle_for.png)

El bucle **for** permite repetir un conjunto de pasos un número de veces determinado. 
Necesitamos  declarar una variables que actuará como contador y definir el valor inicial que tendrá la variable y el final, realizándose tantos como pasos como valores enteros haya entre ambas.

### Bucle **while** 
[[vídeo]](http://youtu.be/894D9hV8paw) [[ejemplo]](./ejemplosBitbloq/bucle_while.xml)

![bucle while](./ejemplosBitbloq/Bucle_while.png)

Usaremos la sentencia de control **while** para los bucles donde el número de veces que se repite no está definido desde el principio

### Bloque **if** : sentencias condicionales
[[vídeo]](http://youtu.be/dXpDCOzsO2U) [[ejemplo]](./ejemplosBitbloq/condicional.xml)

![condicional](./ejemplosBitbloq/condicional.png)

Las sentencias condicionales permiten ejecutar un código y otro según se cumpla o no una determinada condición. Esta condición será una validación que definiremos con operandos.

Podemos hacer que en caso de que se cumpla se ejecute un código (es el bloque if) y en caso de que no se cumpla la condición se ejecute otro (bloque else)

### Condicionales complejas
[[vídeo]](http://youtu.be/en_Y-_wVyO0) [[ejemplo]](./ejemplosBitbloq/condiciones_if.xml)

![Condiciones_lógicas](./ejemplosBitbloq/Condiciones_lógicas.png)

La condición que determina si se ejecuta un bloque u otro o si salimos de un bloque while puede contener varias comprobaciones. 

Entre estas condiciones utilizaremos operadores lógicos que pueden ser AND o OR

* Estas condiciones se tendrán que cumplir todas en el caso del operador AND

* Con que se cumpla una de elllas se dará por válida toda la condición


## Envío de datos al PC: 
[[vídeo]](http://youtu.be/uAy_reYl8_Y) [[ejemplo]](./ejemplosBitbloq/Serial.xml) 

![serial](./ejemplosBitbloq/Datos_al_pc.png)

Podemos enviar contenidos entre nuestra placa y el PC usando las sentencias de comunicaciones. Usaremos print para enviar algo (puede ser el valor de una variable o un texto) al pc o println para enviar y pasar a la siguiente línea.

## Variables locales vs Variables globales
[vídeo](http://youtu.be/D82lXUWH1Jg) [ejemplo](./ejemplosBitbloq/variables_locals_globales.xml)

![ejemplo](./ejemplosBitbloq/variables_locals_globales.png)

Podemos definir variables locales o globales. Una variable global estará definida y por tanto mantendrá su valor en todo el programa, mientras que una variable local solo se definirá donde se haya declarado.

Las variables globales mantienen su valor entre las distintas iteraciones que se realizan del programa.

## Ejemplo de bucle sin sentencias de control

![ejemplo](.ejemplosBitbloq/Bitbloq_bucle_globales.png)  [[ejemplo]](.ejemplosBitbloq/bucle_con_variable_global.xml)

Podemos usar la forma cíclica en la que se ejecutan los programas en Arduino para hacer un bucle sin más estructuras de control que una simple variable global

### Sonido

En bitbloq existen 2 formas de generar sonidos

* Reproducir notas musicales: podemos escoger la nota que vamos a reproducir y su duración

* Seleccionar la frecuencia exacta que queremos reproducir y su duración

![imagen](./ejemplosBitbloq/sonido.png) [[ejemplo]](./ejemplosBitbloq/sonido.xml)

## Librerías

En el caso de Bitbloq, ahora mismo no se pueden usar librerías, de forma manual.

### Servo

![imagen](./ejemplosBitbloq/Servo.png) [[ejemplo]](./ejemplosBitbloq/Servo.xml)

Para usar la librería Servo con bitbloq podemos usar los bloques Servo. Existen 2 tipos de servos: los de rotación continua y los normales.


