---
layout: post
title: "Hardware y Software"
subtitle: "Definiendo un poco de argot, para que no confunda"
date: 2022-07-28 18:45:00 +1000
categories:
  - esenciales
background: '/img/bg-default.jpg'
image: '/img/bg-default.jpg'
---
# Hardware y Software 
**Hardware** es una palabra que, traducida literalmente del inglés, significa “mercancía dura”. Visto así, sin contexto, no tiene mucho sentido, pero cuando pensamos en un ordenador, se refiere a todo aquello que se puede tocar y, por lo tanto, engloba a todos los componentes físicos: pantallas, teclados, ratones, discos internos y chips de distintos tipos. Son los componentes que podemos encontrar en una tienda especializada para montar un ordenador a medida, como memoria, microprocesador, tarjeta gráfica y placa base, y de los que seguramente ya habremos oído hablar. En otros artículos veremos qué hacen y cómo se conectan todos estos componentes, y algunos más.

Por su parte, **software** significa “mercancía blanda”. Sigue sin tener mucho sentido como traducción literal, pero en el contexto de un ordenador es fácil de asociar con todo aquello que se carga en memoria. Aunque normalmente su significado se simplifica para referirse sólamente a programas y otro tipo de código ejecutable, como librerías, es igualmente válido para referirse a los documentos y el contenido multimedia que se procesa con un ordenador.

Como las traducciones literales de *hardware* y *software* no tienen el más mínimo sentido en Español, mejor no lo voy a intentar y seguiré hablando de *hardware* y *software*.

# Requisitos de hardware
La relación entre *hardware* y *software* es bastante directa, y es que para que un software se pueda ejecutar, o procesar, en un ordenador, suelen existir requisitos de *hardware*. Una determinada cantidad de memoria, o un microprocesador o una tarjeta gráfica lo suficientemente potentes, o con una determinada serie de capacidades, son ejemplos frecuentes. Mientras que para editar documentos o realizar cálculos domésticos podemos suponer que cualquier configuración de *hardware* medianamente actual servirá, es fácil pensar que si, por ejemplo, vamos a procesar vídeo de muy alta calidad, necesitaremos *hardware* más rápido y con ciertas capacidades específicas. 

# El sistema operativo y los controladores de dispositivo
Por otra parte, el sistema operativo juega un papel fundamental para poner en contacto *software* y *hardware*. El sistema operativo es un conjunto de programas y otro *software* sin el cual un ordenador no se puede usar: si encendemos un ordenador sin sistema operativo recibiremos un error que dice, literalmente, que no se encuentra el sistema operativo. 

Lo que hace un sistema operativo es poner todas las capacidades del hardware a disposición de los programas que vamos a utilizar, de una forma fácil de usar y homogénea. Por decirlo así, la inmensa mayoría de los programas trabajan, en realidad, con el sistema operativo, y no con el *hardware* directamente.

Por ejemplo, cuando un procesador de textos, como Libreoffice Write o Microsoft Word, quieren guardar un documento en la carpeta “Documentos” de nuestro ordenador, lo hacen a través del sistema operativo de una forma sencilla, y sin entrar en detalles: *guarda estos datos, con este nombre, y en esta carpeta*. 

{% include image.html url="/img/posts/guardar-como.png" description="La ventana de “Guardar como…” de Libreoffice Writer, bajo Manjaro GNU/Linux" %}

De no ser por el sistema operativo, los distintos programas tendrían que saber qué tipo de almacenamiento hay conectado (disco duro, DVD grabable, unidades de memoria USB,…), cómo acceder a él, y tomar una extensa y compleja serie de decisiones acerca del espacio libre, dónde grabar el documento, qué pasa si el espacio libre no es contiguo,… si esto fuera así, programar aplicaciones sería difícil, tedioso y muchísimo más caro.

Gracias al sistema operativo, todas esas complejidades se ocultan de las aplicaciones finales y éstas pueden concentrarse en hacer lo que mejor saben: procesar textos, retocar fotos, o lo que sea.

En general, sin embargo, los sistemas operativos no son capaces de controlar cualquier componente de *hardware*, bajo cualquier circunstancia. En muchas ocasiones, los fabricantes tienen que suministrar pequeños paquetes de *software* que, a modo de extensión del sistema operativo, controlan los dispositivos que forman parte del ordenador o que se conectan a él. Estos paquetes se llaman controladores de dispositivo, símplemente controladores, o también módulos, dependiendo del sistema operativo. Muchas veces, el sistema operativo incorpora los controladores de los dispositivos más populares, pero en otras ocasiones deberemos instalarlos manualmente.

# El firmware: ni duro ni blando, sino firme
Hay una tercera categoría, llamada **firmware**, que se traduciría literalmente como “mercancía firme”… algo así como una cosa que no es blanda pero no llega a ser del todo dura. El *firmware* es código ejecutable que se graba de forma semipermanente (no se borra cuando apagamos el ordenador) en ciertos componentes de *hardware* para simplificar su uso. 

Por ejemplo, una cámara web tiene un cierto comportamiento automático: enfoque, temperatura de color, contraste,… y es capaz de ajustarse automáticamente sin necesidad de que ninguna aplicación ni sistema operativo estén constantemente controlándola. Si la cámara es lo suficientemente compleja y de cierta calidad, ese comportamiento estará programado en una memoria semipermanente y podrá actualizarse para corregir problemas o mejorar su función; en ese caso, este tipo de programas se engloban en lo que se conoce como *firmware*.

¿En qué se diferencia un controlador de un *firmware*? Veamos dos diferencias:

- Mientras que los controladores se instalan sobre el sistema operativo, el *firmware* se instala dentro del *hardware*; por ejemplo, en un chip de la placa de control de un disco duro, o dentro de una cámara web.
- Mientras que el sistema operativo percibe y utiliza los controladores como otro componente de *software* cualquiera, y los carga en la memoria del ordenador, el *firmware* forma parte interna del dispositivo a controlar y no se carga en la memoria del ordenador.

En este caso, el *firmware* es código que reside dentro de los dispositivos, y que hace tareas específicas de forma autónoma en lugar de ser el sistema operativo o sus controladores los encargados de hacerlo.