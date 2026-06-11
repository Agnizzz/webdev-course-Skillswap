# Guion: Lección 9 - Armamos tu perfil web (David Komatsu)

**[0:00 - 0:50] Introducción:** "¡Hola! Bienvenidos al módulo final del curso. Mis compañeros ya te enseñaron HTML, listas, imágenes, links, CSS y cómo darle estilo a todo. Hoy vamos a tomar exactamente esa página que veníamos construyendo y la vamos a convertir en algo real: **tu perfil web personal**. Y al final te cuento los errores más típicos para que no te frustres cuando te pasen."

**[0:50 - 2:00] El punto de partida:** *(Muestras la página como quedó en el módulo 4)* "Esta es la página que dejó Victor en el módulo anterior. Ya tiene títulos con colores, párrafos con bordes, imágenes centradas. Funciona, pero parece un documento. Un perfil necesita identidad: una foto tuya, tu nombre grande, tus redes. Eso es lo que vamos a agregar — sin borrar nada de lo que ya hicieron mis compañeros."

**[2:00 - 3:30] La tarjeta de perfil (HTML):** "Lo primero: arriba de todo, antes del título, agregamos un `div` con `id='tarjeta-perfil'`. ¿Por qué un div? Porque es una caja que agrupa cosas — adentro le metemos tres elementos: la foto con `<img>`, el nombre con el `<h1>` que ya existía, y un párrafo nuevo con la clase `subtitulo`. El div nos permite darle estilo a todo el bloque junto."

**[3:30 - 5:00] La tarjeta de perfil (CSS):** "Ahora el estilo. Al `#tarjeta-perfil` le ponemos fondo morado — seguimos la identidad del proyecto — `text-align: center` que aprendimos en el módulo 4, padding y `border-radius` para las esquinas suaves. Y aquí viene el truco estrella: a la foto le ponemos `border-radius: 50%`. Eso convierte cualquier imagen cuadrada en un **círculo perfecto**. Es la misma propiedad de los bordes redondeados, solo que llevada al máximo."

**[5:00 - 6:00] Sobrescribiendo estilos:** "Ojo con algo importante. Nuestro `h1` tenía color rojo por el `#titulo`, pero dentro de la tarjeta morada el rojo no se lee bien. Entonces escribimos `#tarjeta-perfil h1 { color: white; }`. Esto se llama **selector descendiente**: solo afecta a los h1 que están DENTRO de la tarjeta. Así no rompemos nada del código anterior — solo lo ajustamos donde lo necesitamos."

**[6:00 - 7:30] Redes y pie de página:** "Agregamos el Capítulo IV: Mis redes. Son tres etiquetas `<a>` normales, como las del módulo 2, pero con la clase `boton-red`. En el CSS les ponemos fondo morado, texto blanco, padding y `text-decoration: none` para quitar el subrayado clásico de los links. Resultado: links que parecen botones. Y cerramos con un pie de página simple. Fíjate que al subtítulo y al pie les pongo `background: none` y `border: none` — porque la regla general de `p` les estaba poniendo borde morado a todos, y aquí no lo queremos."

**[7:30 - 8:00] Resultado:** *(Refrescas el navegador)* "Y mira eso. Foto circular, nombre destacado, secciones ordenadas, botones de redes. La misma página de mis compañeros, ahora convertida en un perfil de verdad. Ahora sí: los errores."

# Guion: Lección 10 - Cosas a evitar (David Komatsu)

**[8:00 - 8:50] Error 1 — El CSS no carga:** "Abres tu página y todo se ve blanco, sin estilos. El 90% de las veces es el `<link>`: revisa que el `href` apunte bien al archivo. Si tu archivo se llama `style.css`, el href tiene que decir exactamente eso. Mayúsculas y minúsculas importan: `Style.css` no es lo mismo que `style.css`."

**[8:50 - 9:40] Error 2 — La imagen rota:** "El cuadrito con la X en lugar de tu foto. Casi siempre es la ruta del `src`. Si la imagen está en internet, copia la URL completa. Si está en tu carpeta, escribe solo el nombre: `src='mifoto.jpg'`. Un espacio de más, una letra cambiada, y no carga."

**[9:40 - 10:30] Error 3 — El selector no coincide:** "Escribiste `.boton-red` en el CSS pero en el HTML pusiste `class='Boton-Red'`. Para el navegador son cosas completamente distintas y el estilo nunca llega. Regla de oro: todo en minúsculas, con guiones, y exactamente igual en ambos archivos."

**[10:30 - 11:10] Error 4 — Etiqueta sin cerrar:** "Olvidaste un `</div>` y de repente media página quedó morada porque todo cayó dentro de la tarjeta. VS Code te avisa: si los colores del código se ven raros o la indentación se rompe, busca la etiqueta que quedó abierta."

**[11:10 - 11:40] Error 5 — Reglas que se pisan:** "¿Por qué mi h1 sigue rojo si le puse blanco? Porque en CSS gana el selector más específico: un `id` le gana a una clase, y una clase le gana a una etiqueta. Si un estilo 'no funciona', probablemente otra regla más específica lo está ganando. Aprende a leer tu CSS de arriba a abajo preguntándote: ¿quién gana aquí?"

**[11:40 - 12:00] Cierre:** "Y con eso cerramos el curso. Cinco módulos, una página real construida entre todos, y ahora tu propio perfil web. El siguiente paso natural es JavaScript, para darle vida e interacción. ¡Gracias por llegar hasta el final, y nos vemos en la web!"