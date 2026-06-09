# Guión – Lección 4: Estilos Simples con CSS
**Duración estimada:** ~12 minutos  
**Tema:** Colores de fondo, centrar contenido y bordes

---

¡Hola a todos! ¿Cómo están? En el video anterior ya aprendieron a agregar párrafos,
listas, imágenes y enlaces a una página web. ¡Quedó genial!

Pero... seamos honestos. La página se ve un poco aburrida, ¿no? Solo texto negro
sobre fondo blanco. Hoy vamos a arreglar eso con CSS.

Abran el enlace que les dejamos en la descripción. Van a ver la misma página que
dejaron sus compañeros en la lección anterior, lista para darle estilo.

---

**¿Qué es CSS?**

CSS significa *Cascading Style Sheets*. No hay que memorizar eso. Lo importante es
saber para qué sirve: si HTML es el esqueleto de la página, CSS es la ropa que le
pones. Con CSS decides los colores, el tamaño de las letras, los bordes, dónde va
cada cosa... todo lo visual.

Y lo mejor: en CodePen ya está todo conectado. Solo escribimos en el panel de CSS
y los cambios aparecen al instante.

---

**Color de fondo**

Empecemos por algo divertido. Vamos a cambiar el color de fondo de toda la página.
En el panel de CSS escribimos:

```css
body {
  background-color: #f0f4ff;
}
```

El `body` representa toda la página. `background-color` es la propiedad, y ese código
con el numeral `#f0f4ff` es una forma de escribir colores que se llama código
hexadecimal. No se preocupen por memorizarlo — pueden buscar "color picker" en
Google, eligen el color que quieran y les da el código listo para copiar.

También pueden escribir colores directamente en inglés: `red`, `blue`, `purple`,
`lightblue`... pruébenlo.

---

**Centrar texto**

Ahora vamos a centrar el título principal. Súper fácil:

```css
h1 {
  text-align: center;
}
```

`text-align` puede ser `center`, `left` o `right`. Simple, ¿no? ¡Ya quedó centrado!

---

**Bordes y color de fondo en párrafos**

Vamos a hacer algo más interesante. Le vamos a poner un borde y un fondo blanco
a los párrafos para que resalten:

```css
p {
  background-color: white;
  border: 2px solid purple;
  border-radius: 6px;
  padding: 10px;
}
```

Vamos parte por parte:
- `background-color: white` — fondo blanco para el párrafo
- `border: 2px solid purple` — borde de 2 píxeles, línea sólida, color morado
- `border-radius: 6px` — esquinas redondeadas, le da un look más moderno
- `padding: 10px` — espacio entre el texto y el borde, para que no quede apretado

¡Miren qué diferente se ve!

---

**Estilos para imágenes**

Ahora algo importante: ¿cómo centramos una imagen? Porque `text-align: center`
solo funciona con texto. Para imágenes hay que hacer esto:

```css
img {
  display: block;
  margin: 0 auto;
  width: 300px;
  border: 3px solid purple;
  border-radius: 8px;
  margin-bottom: 15px;
}
```

La combinación de `display: block` y `margin: 0 auto` es la forma clásica de centrar
una imagen. Lo que hace `margin: 0 auto` es repartir el espacio sobrante igual a los
dos lados, lo que la centra automáticamente.

Además le pusimos un borde morado y esquinas redondeadas — ¿recuerdan que
Alexandra dijo que el morado es su color favorito? ¡Aprovechamos eso!

Y `width: 300px` le fija un tamaño razonable, porque como vieron en la lección
anterior, sin eso las imágenes salen enormes.

---

**Cierre**

¡Y listo! Con unas pocas líneas de CSS la página cambió completamente. Pusimos
color de fondo, centramos el título, le dimos estilo a los párrafos y a las imágenes.

En la siguiente lección vamos a juntar todo lo que aprendieron — HTML y CSS —
para construir una página de perfil completa desde cero.

Su tarea: en el CodePen del enlace de la descripción, cambien los colores por sus
favoritos y prueben diferentes valores de `border-radius`. Pongan `50px` y vean
qué pasa con las imágenes. ¡Diviértanse! Nos vemos en la siguiente lección.

---

*Notas de producción:*
- *Herramienta en pantalla: CodePen (sin registro requerido)*
- *Link del starter: completar con URL del CodePen al subir*
- *Sin branding ni referencias a autores en pantalla*
