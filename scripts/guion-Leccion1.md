## Guion Leccion 1: Introduccion al Desarrollo Web + Estructura HTML Basica

Hola y bienvenido. En esta leccion vas a aprender que es el desarrollo web, como funciona un sitio web y como escribir tu primera pagina en HTML. No necesitas instalar nada, solo abre tu navegador. Vamos.

---

### Que es un sitio web

Primero lo primero: que es exactamente un sitio web. Cuando abres una pagina como Wikipedia o YouTube en tu navegador, lo que estas viendo es el resultado de un archivo de texto especial que el navegador interpreta y muestra visualmente.

Piensalo asi: un sitio web es como una carta. La carta tiene contenido, palabras, imagenes, listas. Pero tambien tiene formato, el tipo de letra, los colores, el tamanio del texto. En el desarrollo web, el contenido lo maneja HTML y el formato lo maneja CSS.

En esta leccion nos enfocamos en HTML, que es la base de todo sitio web. Sin HTML no hay pagina web.

---

### Que es HTML

Ahora, que es HTML. HTML significa HyperText Markup Language. Lo que hace HTML es muy simple: le dice al navegador que es cada cosa en la pagina. Le dice: esto es un titulo, esto es un parrafo, esto es una imagen, esto es un enlace.

HTML no es un lenguaje de programacion como Java. Es un lenguaje de estructura, defines que hay en la pagina y donde va. Lo hace con etiquetas. Eso es lo que vamos a ver ahora.

---

### Abrir CodePen

Para escribir HTML no necesitas instalar nada. Vamos a usar CodePen, un editor online gratuito. Abre una nueva pestania y escribe: codepen.io/pen. Vas a ver tres columnas: HTML, CSS y JS. Hoy solo usamos la columna de HTML. En la parte de abajo veras el resultado en tiempo real cada vez que escribas algo.

---

### Estructura basica de HTML

Todo documento HTML tiene una estructura base que siempre es la misma. Escribe esto en la columna HTML de CodePen:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Mi primera página</title>
  </head>
  <body>
    <h1>¡Hola Mundo!</h1>
    <p>Esta es mi primera página web.</p>
  </body>
</html>
```

Mira el resultado abajo, ya aparece tu primera pagina web. Ahora te explico que significa cada parte:

- `<!DOCTYPE html>` le dice al navegador que este archivo es HTML moderno. Siempre va en la primera linea.
- `<html>` es la etiqueta raiz. Todo el contenido de la pagina va dentro de ella.
- `<head>` es la cabeza del documento. Aqui va informacion sobre la pagina que el usuario no ve directamente, como el titulo.
- `<title>` define el texto que aparece en la pestania del navegador.
- `<body>` es el cuerpo. Todo lo que va aqui si aparece en la pagina visible.
- `<h1>` es un encabezado de nivel 1, el titulo principal de la pagina.
- `<p>` es un parrafo de texto.

---

### Etiquetas, elementos y atributos

Ahora entendamos bien como funciona una etiqueta HTML. Una etiqueta tiene tres partes:

- Etiqueta de apertura: `<p>`
- Contenido: el texto que va adentro
- Etiqueta de cierre: `</p>`

Juntas forman un elemento HTML: `<p>Este es un parrafo.</p>`

La etiqueta de cierre lleva una barra `/` antes del nombre. Algunos elementos tambien tienen atributos, informacion extra que va dentro de la etiqueta de apertura:

```html
<body>
  <h1>Mi página</h1>
  <p>Bienvenido a mi primera página web.</p>

  <!-- Enlace con atributo href -->
  <a href="https://www.google.com">Ir a Google</a>

  <!-- Imagen con atributos src y alt -->
  <img src="https://via.placeholder.com/200" alt="Una imagen de ejemplo">

</body>
```

El atributo `href` le dice al navegador a donde ir cuando el usuario haga clic. El atributo `src` es la direccion de la imagen. El atributo `alt` es un texto alternativo que aparece si la imagen no carga. La etiqueta `<img>` no tiene etiqueta de cierre porque es una etiqueta vacia. Las lineas que empiezan con `<!--` y terminan con `-->` son comentarios, el navegador las ignora.

---

### Practica - Tu turno

Ahora es tu turno. En CodePen, escribe una pagina sencilla con esta informacion:

- Un `<h1>` con tu nombre
- Un `<p>` que diga algo sobre ti
- Un enlace a tu red social favorita

Ejemplo:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Mi perfil</title>
  </head>
  <body>

    <h1>Ana García</h1>

    <p>Hola, soy Ana. Me encanta la música y el diseño web.</p>

    <a href="https://www.instagram.com">Sígueme en Instagram</a>

  </body>
</html>
```

Pausa el video aqui, hazlo en CodePen y regresa cuando termines.

---

### Errores comunes

Antes de terminar te muestro los errores mas frecuentes:

**Error 1 - Olvidar cerrar la etiqueta:**

```html
<!-- Error: falta el cierre -->
<p>Este parrafo no tiene cierre

<!-- Correcto -->
<p>Este parrafo si tiene cierre.</p>
```

**Error 2 - Cerrar en el orden incorrecto:**

```html
<!-- Error: orden incorrecto -->
<h1><p>Texto</h1></p>

<!-- Correcto: el ultimo en abrir es el primero en cerrar -->
<h1>Titulo</h1>
<p>Parrafo</p>
```

**Error 3 - Olvidar las comillas en los atributos:**

```html
<!-- Error: sin comillas -->
<a href=https://google.com>Google</a>

<!-- Correcto: con comillas dobles -->
<a href="https://google.com">Google</a>
```

Si algo no aparece como esperas en CodePen, revisa estas tres cosas: cerraste todas las etiquetas, el orden es correcto, y los atributos tienen comillas.

---

### Resumen y cierre

Llegaste al final de la Leccion 1. Aprendiste:

- Un sitio web tiene contenido en HTML y estilo en CSS.
- HTML usa etiquetas para definir que es cada elemento.
- La estructura base siempre incluye `<!DOCTYPE html>`, `<html>`, `<head>` y `<body>`.
- Los atributos dan informacion extra a las etiquetas.
- Toda etiqueta se cierra, excepto las vacias como `<img>`.

En la proxima leccion veremos mas elementos HTML: encabezados, listas, imagenes y enlaces en detalle. El enlace a CodePen con el codigo de hoy esta en la descripcion. Nos vemos en la Leccion 2.
