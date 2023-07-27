<script>
  var details = document.querySelectorAll('details');
  details.forEach(function(detail) {
    detail.addEventListener('click', function() {
      details.forEach(function(otherDetail) {
        if (otherDetail !== detail) {
          otherDetail.removeAttribute('open');
        }
      });
    });
  });
</script>
<style>
    h1{
        color: blue;
    }
</style>

# Titulo Principal
Esto es un documento de Markdown
alt 96 para poner comillas inversas `

Los titulos se escriben con los # desde poner 1 hasta 6.
## Titulo Secundario
El texto que sea
* Lista1
* Lista2
<details>
<summary>Concepto 1</summary>

Definición del concepto 1.
</details>

<details>
<summary>Concepto 2</summary>

Definición del concepto 2.
</details>

<details>
<summary>Concepto 3</summary>

Definición del concepto 3.
</details>

Las **negritas** las *cursivas*


# Código

```html
<!DOCTYPE html>
<html lang="en">
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
    <h1 >Aprendiendo estilos CSS</h1>
    <h2>Aprendiendo estilos CSS</h2>
    <h2>Aprendiendo estilos CSS</h2>
    <h2 id="ultimo">Aprendiendo estilos CSS</h2>
    <h2 class="brown">Aprendiendo estilos CSS</h2>
    <h2 class="brown">Aprendiendo estilos CSS</h2>
    <h2 id="ultimo">Aprendiendo estilos CSS</h2>
    <h2>Aprendiendo estilos CSS</h2>

</body>
</html>
```
