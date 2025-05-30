instrucciones ejecutar el codigo

1)se extrae el archivo zip

2)instalar la aplicacion de godot engine 4.4.1

3)abrir godot engine

4)Darle importar archivo

5)seleccionar la carpeta del archivo extraido

6)alli abajo a la izquierda podras observar todos los elemntos incluidos los codigos los cuales terminan en gd
solo les daras doble click y podras observarlos

7)para ejecutar el juego puedes darle a la flecha en la esquina superior derecha

Funciones adicionales:

1.Graficos:

para que se implemento:

Se implementó para mejorar la experiencia visual del jugador, permitiendo que el entorno, los personajes y los elementos del juego sean representados de manera clara, atractiva y de una manera comprensible.

porque se considero necesario:

Se consideró necesario porque los gráficos son una parte fundamental en la interacción entre el jugador y el juego para darle una representacion a lo que sucede en el programa.

como se implemento:

Se implementó utilizando la herramienta de desarrollo Godot Engine, que ofrece un sistema visual intuitivo para añadir y organizar gráficos. Se usaron nodos como Sprite, buttons y CanvasLayer para incorporar imágenes, y fondos al juego.
y me guie usando la guia "Juego de Plataformas 2D/Godot Tutorial/Introduccion Godot/1-Capitulo/Programacion Videojuegos"
https://www.youtube.com/watch?v=F3T_ZhllzJs&list=PLNEAWvYbJJ9nNOpe6fun7m6L_M8xslYnT

y tambien la guia UI en Godot: crea tu INTERFAZ DE USUARIO sin morir en el intento 
https://www.youtube.com/watch?v=55U-hnUnFAY

2.animaciones:

para que se implemento:

Se implementó para dar vida a los elementos del juego y asemejarse al juego original
porque se considero necesario:
las animaciones ayudan a comunicar visualmente lo que está ocurriendo en el juego y ademas ppara asemejarse al juego original

como se implemento:

Se implementó utilizando el motor Godot Engine, específicamente con nodos como AnimationPlayer y elementos visuales como Sprite para controlar las animaciones. Por ejemplo, para la habilidad “Garra”, se utilizó un Sprite y un AnimationPlayer que reproduce una animación al activarse el botón correspondiente. Se mostraron efectos visuales como el sprite de garras, se reprodujo la animación con play(), y se usó await para esperar a que termine antes de continuar con el flujo del combate.
Además, se manejaron otras animaciones como el rayo, usando visibilidad y temporizadores (create_timer) para mostrar los efectos por un tiempo determinado.
para su implementacion me base en los videos de Tutorial AnimationPlayer en Godot Engine. (Parte 1) https://www.youtube.com/watch?v=pXK-CotnVIM

y para crear la animacion del rayo especificamente me base en la siguiente  publicacion de reddit https://www.reddit.com/r/godot/comments/15lzzgw/little_question_about_using_a_timer_in_an_await/
