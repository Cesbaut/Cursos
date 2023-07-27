# INTRODUCCION CSS
Como introducción se estudiará como introducir estilos a un html, ademas de indentificadores y clases.
#### ¿Qué es CSS?
En español significa Hojas de Estilo en Cascada, este permite introducir diferentes estilos como colores, fondos, formas etc. a tu pagina web.

## METODOS PARA COLOCAR ESTILOS CSS EN HTML
Existen tres metodos.
* Colocar el estilo dentro de la etiqueta.
* Como estilos dentro de la etiqueta head.
* En una Hoja de CSS (mas eficiente).
### Dentro de la etiqueta en HTML
Si quiero cambiar, por ejemplo, el color de una etiqueta, como atributo pondremos style="" y dentro de las comillas los estilos a colocar.

```html
<h1 style="color:blue;">
    Aprendiendo estilos CSS
</h1>
```

### Con a etiqueta < style ></ style >
Se coloca la etiqueta dentro de head, con todos los atributos que desees.
```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CODING CSS</title>
    <style>
        h1{
            color: blue;
        }
        h2{
            color: greenyellow;
        }
        #ultimo{
            color: red;
        }
        .brown{
            color: brown;
        }
    </style> 
</head>
<body>
    <h1 style="color:blue;">Aprendiendo estilos CSS</h1>
    <h2>Aprendiendo estilos CSS</h2>
    <h2>Aprendiendo estilos CSS</h2>
    <h2 id="ultimo">Aprendiendo estilos CSS</h2>
    <h2 class="brown">Aprendiendo estilos CSS</h2>
    <h2 class="brown">Aprendiendo estilos CSS</h2>
    <h2 id="ultimo">Aprendiendo estilos CSS</h2>
    <h2>Aprendiendo estilos CSS</h2>
</body>
```

### Una hoja CSS :)
Este es el mejor metodo ya que lo podemos utilizar no solo para una hoja de html sino para mas.

Dentro del head le damos el enlace
```html
    <link rel="stylesheet" href="NombreArchivo.css">
```
 
Esto lo enlaza con nuestra pagina, en donde pondremos los estilos.
```css
h1{
    color: rebeccapurple;
}
h2{
    color: greenyellow;
}
#ultimo{
    color: red;
}
.brown{
    color: brown;
}
```
## METODOS PARA APLICAR ESTILOS A ETIQUETAS
Tenemos tres principales metodos.
* Etiqueta General.
* ID.
* Clase.
## Aplicar a una etiqueta general
Ponemos el nomnbre de la etiqueta HTML y abajo con estilo, esto se aplicara para todos los de la misma etiqueta.
```css
h1{
    color: blue;
}
h2{
    color: greenyellow;
}
```
## ID
Aplicamos un identificador a la etiqueta en el html que quedramos editar, importante mencionar que los cambios se haran solamente a este id.

Usamos **id=" "**
```html
<h2 id="ultimo">Aprendiendo estilos CSS</h2>
```

Y en los estilos de la hoja css pondemos un **#** con el nombre del id.
```css
#ultimo{
    color: red;
}
```
## Clase
Las clases pueden aplicar estilos a diferentes etiquetas.

Usamos **class=" "**
```html
<h2 class="brown">Aprendiendo estilos CSS</h2>
<h2 class="brown">Aprendiendo estilos CSS</h2>
```
En CSS los identificaremos con un punto **.** seguido del nombre de la clase.
```css
.brown{
    color: brown;
}
```

## COLORES
Existen tres diferentes formas de poner colores en paginas web.
* Nombre
* Hexadecimal
* RGB
* RGBa
* HSL
* HSLa
Aqui algunos ejemplos en CSS:
```css
.name{
    background-color: lightgreen;
}
.hex{
    background-color: #00FF6C;
}
.rgb{
    background-color: rgb(219, 53, 53);
}
.rgba{
    background-color: rgba(219, 53, 53, 0.3);
}
.hsl{
    background-color: hsl(130, 94%, 51%);
}
.hsla{
    background-color:  hsla(16,100%,50%,0.8);
}
```
Pagina que te da mas informacion:
https://htmlcolorcodes.com/
