---
layout: post
title: "La mínima expresión de un ordenador"
subtitle: "Los ordenadores no son tan complicados, en realidad"
date: 2021-09-09 10:45:13 +1000
categories:
  - esenciales
background: '/img/bg-default.jpg'
image: '/img/bg-default.jpg'
---
En realidad, un ordenador es una máquina de procesar de información. Sólo es capaz de hacer, muy bien y muy rápido, lo siguiente:

1. Se introducen unos **datos de entrada**,
2. el ordenador lleva a cabo uno o varios **procesos** sobre los datos de entrada,
3. y entrega unos **datos de salida** con el resultado del proceso.

Esta lista de pasos suele representarse de la siguiente forma:

{% include image.html url="/img/posts/ordenadores-proceso.png" description="Procesando información" style="width: 60%" %}

A simple vista, puedes pensar que estoy *sobresimplificando* esa máquina que tienes delante. Que eso se parece más a lo que puede hacer una calculadora de lo más rudimentaria, que acepta dos *operandos* (los datos de entrada), una *operación* (el proceso) para devolver un *resultado* (los datos de salida). Sin embargo, es lo único que hace cualquier ordenador, por avanzado que sea y por muy sofisticada que sea la forma que tienen de representar los resultados con ventanas, vídeos, animaciones, sonidos y texto con formato.

Cuando enciendes un ordenador, éste se quedará esperando a que le indiques qué quieres hacer. Normalmente, y a no ser que solamente quieras ver la hora en el reloj del sistema, deberás abrir una **aplicación**. *Aplicaciones*, o más generalmente, *programas*, es la forma que grupos de procesos toman ante nosotros en la práctica, como veremos a continuación.

{% include image.html url="/img/posts/windows-10.png" description="El escritorio de Windows 10" %}

Los datos de entrada para ese proceso consisten en la aplicación que quieres abrir, el proceso consiste en cargarla en memoria y ejecutarla, y los datos de salida suelen ser una pista de que se ha ejecutado o se está ejecutando. En su forma más sofisticada, eso consiste en mostrar una ventana gráfica completa, con menús, botones y toda una serie de controles y gráficos. Pero, en esencia, lo que ha ocurrido es lo que hemos explicado arriba: introducir unos datos de entrada, procesarlos, y producir unos datos de salida.

Si la aplicación que has abierto es un procesador de textos, como [Microsoft Word](https://es.wikipedia.org/wiki/Microsoft_Word), [LibreOffice Writer](https://es.libreoffice.org/descubre/writer/) o [Apple Pages](https://www.apple.com/es/pages/), éste va a quedarse esperando, de nuevo, por datos de entrada. En este caso, esos datos son texto, los procesos van a ser la serie de operaciones de formato y maquetación que queramos aplicar, y los datos de salida consistirán en el documento que vemos tomar forma ante nosotros. 

{% include image.html url="/img/posts/word.png" description="Un procesador de textos (Microsoft Word)" %}

Con una hoja de cálculo, o con cualquier otra aplicación de productividad ofimática, la mecánica es la misma.

Para terminar con los ejemplos veamos uno mucho más complejo por la variedad de datos de salida que produce, y la forma que toman: un videojuego sencillo. En este tipo de programas, los datos de entrada, los procesos y los datos de salida serán mucho más numerosos y diversos, en forma de gráficos, sonido, acciones sobre controladores de videojuegos (🎮) y un largo etcétera.

“[Pac-Man](https://es.wikipedia.org/wiki/Pac-Man)” o, como se llamó en España, come-cocos, tiene como protagonista [a una pelota amarilla que debe comerse todos los objetos de un laberinto](https://en.wikipedia.org/wiki/File:Pac-man.png), evitando a cuatro fantasmas. Si el protagonista se come un elemento especial, que por aquel entonces llamábamos “vitamina”, las tornas se giran durante unos segundos y podremos “comernos” a los fantasmas, que ahora escapan, para enviarlos a una cárcel temporal. 

Los datos de entrada vienen dados por: 

1. Tu uso del control, que mueve al protagonista en una dirección
2. La posición relativa del protagonista con respecto a las paredes del laberinto, a los elementos que quedan disponibles en el laberinto, y a los fantasmas
3. El último elemento que el protagonista ha comido, cuyo tipo puede afectar al comportamiento de los fantasmas.
4. Cuántos elementos quedan en el laberinto

El funcionamiento del videojuego consta de **muchos procesos, cada uno con sus datos de salida** en forma de consecuencias en el propio videojuego, y acción, en forma de gráficos en movimiento: 

- si el protagonista intenta moverse:
  - hacia una pared inmediatamente contigua, no se podrá mover, 
  - contra un fantasma inmediatamente contiguo: 
    - hemos perdido una vida, 
    - pero si eso ocurre durante los efectos de la “vitamina”, quien pierde es el fantasma; 
  - contra un elemento “comestible”, acumula puntos; 
    - si el elemento es una vitamina, los fantasmas escaparán, 
    - si choca es el último elemento que quedaba por comer, hemos ganado el nivel.
- si no choca con nada, o sólo choca con un elemento comestible, entonces el comecocos se moverá en la dirección especificada por el jugador.
- durante estos procesos, además, todos los fantasmas se mueven aleatoriamente por el laberinto.

En esencia, los ordenadores son procesadores de información que gozan de toda una serie de posibilidades que los hacen versátiles para múltiples tareas. A diferencia de sistemas más especializados como la calculadora del ejemplo, los ordenadores tienen un **propósito general**, de tal forma que son capaces de realizar muchos procesos, muy rápido, a menudo varios a la vez, mostrando resultados de diferentes formas. 

Un concepto tan sencillo como el esquema de proceso en tres pasos introducido al principio de este artículo es la base para entender, prácticamente, todo lo que ocurre en un ordenador. A lo largo de la vida de este blog llegaremos a ver y usar esa secuencia lógica de operaciones en muchas ocasiones, como puede ser programar o automatizar tareas.
