# Guion - Módulo 4: Ajustando los detalles

¡Hola a todos! ¿Cómo están? En el video anterior ya vieron cómo cambiar los colores de las letras y las fuentes. Ahora vamos a llevar esto al siguiente nivel. 

A veces nuestra página se ve un poco desordenada con todo tirado hacia la izquierda. Hoy vamos a aprender a centrar las cosas, a pintar el fondo de la página y a ponerle bordes a nuestros elementos. 

Abran el enlace que les dejamos en la descripción. Van a ver una pequeña tarjeta de presentación en blanco y negro.

Primero, vamos a pintar el fondo de tooooda la pantalla. Para eso, usamos el selector `body`, que representa todo el cuerpo de nuestra página web. En la cajita de CSS escribimos `body`, abrimos llaves `{}` y adentro ponemos `background-color: lightgray;`. 

¡Pum! Ahora el fondo es de un color gris claro.

Pero nuestra tarjeta de presentación se pierde un poco, ¿no? Vamos a arreglar al contenedor que tiene nuestro texto, que es esa etiqueta `div` que ven en el HTML. 

Escriban `div`, abran llaves `{}` y vamos a ponerle fondo blanco con `background-color: white;`. 

Mucho mejor. Ahora, para que no se vea todo pegado a la izquierda, vamos a centrar el texto. Dentro de las mismas llaves del `div`, agreguen esta instrucción: `text-align: center;`. Esta es súper útil y la van a usar un montón.

Por último, vamos a encerrar nuestra tarjeta en un cuadrado para que resalte. Escriban `border: 3px solid black;`. Esto le dice al navegador: "Pon un borde de 3 píxeles de grosor, que sea una línea sólida y de color negro". 

¡Y listo! Ya tienen una tarjeta centrada y con estilo. Prueben cambiando los colores o el grosor del borde y diviértanse un rato. ¡Nos vemos en la siguiente lección para el proyecto final!
