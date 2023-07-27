<style>
    #Color{
        color: blue;
    }
</style>

<h1 id="Color">Etiquetas de texto</h1>
A continuacion se presentarán las etiquetas de texto mas comunes en el lenguaje HTML.
<br><br>

## < p ></ p >
Funcionan simplemente para colocar texto.

Da un salto de linea al terminar el texto
```html
<p>
    Texto
</p>
```
<br>

## < b ></ b >
Funciona para poner un texto en negritas
```html
<b>Negrita</b>
```
<br>

## < strong ></ strong >
Igual las pone en negritas pero toma como un significado mas importante en el texto.
```html
<strong>Negrita</strong>
```
<br>

## < i ></ i >
Pone en cursivas el texto.
```html
<i>Cursiva</i>
```
<br>

## < em ></ em >
De igual manera pone en cursiva pero tiene importancia semántica.
```html
<em>Cursiva</em>
```
<br>

## < blockquote ></ blockquote >
Se utiliza para citar un bloque de texto.


```html
<blockquote>Este es un bloque de texto citado, es solo como un ejemplo de como se veria.</blockquote>
```
*Esto es un texto de ejemplo:*
>Este es un bloque de texto citado, es solo como un ejemplo de como se veria.

<br>

## < hr />
Es una etiqueta de apertura y sirve para hacer una linea horizontal en la pagina. 
```html
<hr/>
<hr/>
<hr/>
```
*Ejemplo de como se ve:*

---
---
---
<br>

## < br />
Simplemente da un salto de linea al texto que se esta escribiendo.
```html
<p>Este es un texto<br/>con un salto de línea.</p>
```
*Ejemplo de como se ve:*
<p>Este es un texto<br/>con un salto de línea.</p>
<br>

## < h# >< /h# >
Sirven para colocar diferentes tamaños de títulos. Solo hay seis y el primero es el tamaño mas grande.
```html
<h1>Título principal</h1>
<h2>Título secundario</h2>
<h3>Título terciario</h3>
<h4>Título cuarto</h4>
<h5>Título quinto</h5>
<h6>Titulo sexto</h6>
```
<br>

*Ejemplo de como se ve:*

<br>
<h1>Título principal</h1>
<h2>Título secundario</h2>
<h3>Título terciario</h3>
<h4>Título cuarto</h4>
<h5>Título quinto</h5>
<h6>Titulo sexto</h6>

<br>

## < abbr title=”” >  </ abbr >
Sirve para abreviar.

Con title dentro de la etiqueta, cuando el usuario pase el mause aparecera completa la definicion.
```html
<p>La <abbr title="Organización de las Naciones Unidas">ONU</abbr> es una organización internacional.</p>
```
*Ejemplo de como se ve:*
<p>La <abbr title="Organización de las Naciones Unidas">ONU</abbr> es una organización internacional.</p>

<br>

## < cite ></ cite >
Se utiliza para indicar que el texto está citando una obra o una referencia. Se suele usar para títulos de libros, películas, artículos, etc.
```html
<p>Según el libro <cite>"El gran Gatsby"</cite> de F. Scott Fitzgerald, "El pasado puede perseguirnos".</p>

<!-- Otra opcion -->

<p>Fuente: <cite title="https://es.wikipedia.org/wiki/Vinton_Cerf">Wikipedia</cite> </p>
```

*Ejemplo de como se ve:*

<p>Según el libro <cite>"El gran Gatsby"</cite> de F. Scott Fitzgerald, "El pasado puede perseguirnos".</p>
<!-- Otra opcion -->
<p>Fuente: <cite title="https://es.wikipedia.org/wiki/Vinton_Cerf">Wikipedia</cite> </p>

<br>

## < u ></ u >
Sirve para subrayar un texto simple
```html
<u>Texto subrayado</u>
```
*Ejemplo de como se ve:*

<u>Texto subrayado</u>

<br>

## < ins ></ ins >
Sirve para un subrayado, como insertar.
```html
<ins>Texto subrayado</ins>
```
*Ejemplo de como se ve:*

<ins>Texto subrayado</ins>

<br>

## < del ></ del >
Tacha el parrafo, eliminar.

Hace referencia a que fue eliminado el texto del documento y por lo tanto ya no es valido.
```html
<del>Texto subrayado</del>
```
*Ejemplo de como se ve:*

<del>Texto eliminado</del>

<br>

## < s ></ s >
Sirve para tachar el texto e indica que po alguna razon esta pero ya no deberia
```html
<p><s>Texto obsoleto</s></p>
```
*Ejemplo de como se ve:*

<p><s>Texto obsoleto</s></p>

<br>

## < code ></ code >
Esta etiqueta se utiliza para resaltar fragmentos de código o elementos de programación dentro de un documento.
```html
<p>Para imprimir un mensaje en JavaScript, usa el siguiente código: <code>console.log("Hola, mundo!");</code></p>
```
*Ejemplo de como se ve:*

<p>Para imprimir un mensaje en JavaScript, usa el siguiente código: <code>console.log("Hola, mundo!");</code></p>

<br>

## < pre ></ pre >
Esta etiqueta se utiliza para representar texto preformateado, lo que significa que el texto se muestra exactamente como se escribe en el código fuente
```html
<pre>
function calcularSuma(a, b) {
    return a + b;
}
</pre>
```
*Ejemplo de como se ve:*

<pre>
function calcularSuma(a, b) {
    return a + b;
}
</pre>

<br>

## < q ></ q >
Pone entre comillas el texto. se utiliza para indicar una cita corta en línea dentro del texto.
```html
<p>El autor dijo: <q>La vida es lo que sucede mientras estás ocupado haciendo otros planes</q>.</p>
```
*Ejemplo de como se ve:*

<p>El autor dijo: <q>La vida es lo que sucede mientras estás ocupado haciendo otros planes</q>.</p>

<br>

## < small ></ small >
Sirve para hacer mas chico un texto
```html
<small>El autor dijo: <q>La vida es lo que sucede mientras estás ocupado haciendo otros planes</q>.</small>
```
*Ejemplo de como se ve:*

El autor dijo: <small><q>La vida es lo que sucede mientras estás ocupado haciendo otros planes</q>.</small>

<br>

## < mark ></ mark >
Funciona para remarcar un texto.
```html
El autor dijo: <mark>La vida es lo que sucede mientras estás ocupado haciendo otros planes</mark>.
```
*Ejemplo de como se ve:*

El autor dijo: <mark>La vida es lo que sucede mientras estás ocupado haciendo otros planes</mark>.

<br>

## < sub ></ sub >
Sirve para colocar como un subindice, es decir, mas abajo del texto.
```html
H<sub>2</sub>O
```
*Ejemplo de como se ve:*

H<sub>2</sub>O

<br>

## < sup ></ sup >
Sirve para colocar lo de adentro un poco mas arriba del texto
```html
Esto es un <sup>párrafo</sup>
```
*Ejemplo de como se ve:*

Esto es un <sup>párrafo</sup>

<br># Cursos
