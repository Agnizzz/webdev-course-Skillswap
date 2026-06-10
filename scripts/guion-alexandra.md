# Estilos en CSS

¡Hola! En la lección anterior aprendimos cómo agregarle contenido a nuestra primera página web. Por ahora, nuestra página sigue viéndose bastante simple, así que en la lección de hoy aprenderemos cómo cambiar el color, el tipo de fuente, el grosor y hasta el tamaño de las letras de nuestro texto.

Para ello, tenemos que dirigirnos a la hoja de estilos en CodePen. Para acceder a ella, debemos hacer clic en el ícono del archivo en el menú izquierdo de nuestra pantalla. Allí aparecerán tres archivos diferentes:

- `index.html` (donde está toda la estructura actual de nuestra página).
- `script.js`
- `style.css` (nuestra hoja de estilos).

Vamos a darle clic a `style.css` y aparecerá una nueva hoja. Existen tres formas diferentes de agregar estilo a un elemento:

---

## 1. Estilos por Etiquetas

Comenzaremos con el más simple. Por ejemplo, si queremos que los títulos de los capítulos tengan un tipo de letra diferente al resto del texto, regresamos al `index.html` y veremos que a los capítulos les hemos puesto la etiqueta `<h2>`.

Para hacer referencia en nuestra hoja de estilos, utilizamos esa misma etiqueta: escribimos el nombre `h2` y abrimos llaves `{}`. Adentro indicamos la propiedad que queremos cambiar. En este caso, el tipo de letra con la propiedad `font-family`:

```css
h2 {
    font-family: Calibri;
}
```

Aplicar estilos usando etiquetas es bastante cómodo si quieres que el mismo estilo se aplique a todos los elementos de ese tipo.

---

## 2. Estilos por Clases (Class)

Ahora, si quisiéramos que **solo** el título del Capítulo 3 fuera de color morado, podemos utilizar clases.

Vamos al `index.html` y, en la etiqueta de ese título, dejamos un espacio y escribimos `class="nombre-de-la-clase"`. Por ejemplo: `titulo-llamativo`.

> ⚠️ **Nota importante:** El nombre de la clase no debe tener espacios porque si no se rompe; lo ideal es usar minúsculas y separar las palabras con un guion.

Luego, regresamos a la hoja de estilos y para llamar a una clase usamos un **punto (`.`)** seguido de su nombre:

```css
.titulo-llamativo {
    color: purple;
}
```

Lo bueno de las clases es que **pueden reutilizarse** cuantas veces quieras. Si vas al Capítulo 1 y le agregas la misma clase `class="titulo-llamativo"`, automáticamente adoptará el color morado.

> **Nota:** También podemos usar clases para aplicar otros estilos, como crear una clase `.negrita` que use la propiedad `font-weight: bold;` para resaltar párrafos.

---

## 3. Estilos por Identificadores (ID)

Si queremos que el encabezado principal (`<h1>`) que dice *"Mi primera página web"* tenga un estilo único, utilizamos un ID. En el HTML le asignamos, por ejemplo, `id="titulo"`.

En la hoja de estilos, los IDs se llaman utilizando un **hashtag o número (`#`)**:

```css
#titulo {
    font-size: 60px;
    color: red;
}
```

---

# 👑 La Jerarquía en CSS (Especificidad)

¿Qué pasa si le aplicamos las tres formas (etiqueta, clase e ID) a un mismo elemento? Si a nuestro título principal le asignamos la etiqueta `h1` (color verde), la clase `.titulo-llamativo` (color morado) y el ID `#titulo` (color rojo), el navegador elegirá un ganador basado en una clara jerarquía de prioridades:

1. 🥇 **ID:** Tiene la máxima prioridad. El título se verá rojo.
2. 🥈 **Clase:** Si quitamos el ID, el elemento adoptará el estilo de la clase (morado).
3. 🥉 **Etiqueta:** Si también quitamos la clase, al final adoptará el estilo de la etiqueta base (verde).

---

¡Eso sería todo por la lección de hoy! En la siguiente clase aprenderemos más cosas interesantes para agregarle más estilos a nuestra página web y que se vea muchísimo más llamativa.