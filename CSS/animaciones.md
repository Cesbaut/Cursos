# Animaciones CSS
```css
.box{
    /* border: 1px solid;
    position: absolute;
    top: 16px;
    left: 20px;
    width: 300px;
    height: 300px; forma en html */
    /* animation-name: CamColor;
    animation-duration: 2000ms;
    animation-delay: 0;
    animation-iteration-count: 1;
    animation-direction: normal;
    animation-timing-function: cubic-bezier(0.175, 0.885, 0.32, 1.275);
    animation-fill-mode: forwards; */
    animation: CamColor 2000ms cubic-bezier(0.175, 0.885, 0.32, 1.275) 0s infinite normal forwards, otraAnim 2000ms none 0s infinite;
}

@keyframes CamColor{
    0%{
        background-color: rgb(255, 0, 0);
    }
    50%{
        background-color: aqua;
    }
    100%{
        background-color: rgb(83, 9, 255);
    }
}
@keyframes otraAnim {
    0%{border-radius: 0%;}
    50%{border-radius: 25%;}
    100%{border-radius: 50%;}
}
```
Las animaciones en CSS son una forma poderosa de agregar movimiento y dinamismo a los elementos de una página web. Con ellas, puedes crear efectos visuales atractivos y mejorar la experiencia del usuario. Las animaciones en CSS se basan en la modificación gradual de las propiedades de estilo de un elemento a lo largo del tiempo.
## Propiedades
### @keyframes
```css
@keyframes nombreDeLaAnimacion {
  0% {
    /* Estilos iniciales */
  }
  50% {
    /* Estilos a la mitad de la animación */
  }
  100% {
    /* Estilos finales */
  }
}
```
### animation-name
Es una propiedad que define el nombre de la animación que se utilizará. Debes usar el nombre que hayas definido en @keyframes.
```css
.elemento {
  animation-name: nombreDeLaAnimacion;
}
```
### animation-duration
Establece la duración de la animación en segundos o milisegundos.
```css
.elemento {
  animation-duration: 2s; /* 2 segundos */
}
```
### animation-delay
Especifica el tiempo de espera antes de que comience la animación. 
```CSS
.elemento {
  animation-delay: 1s; /* 1 segundo */
}
```
### animation-iteration-count
Define cuántas veces se repetirá la animación. Puede ser un número específico o "infinite" para que la animación se repita indefinidamente.
```css
.elemento {
  animation-iteration-count: 3; /* Se repetirá 3 veces */
}
```
### animation-direction
Indica si la animación se ejecutará en sentido normal ("normal"), al revés ("reverse"), alternando entre ambos ("alternate"), o alternando yendo hacia atrás ("alternate-reverse").
```css
.elemento {
  animation-direction: alternate;
}
```
### animation-timing-function
Define cómo los valores intermedios de la animación se calculan a lo largo del tiempo. Puede ser lineal, ease, ease-in, ease-out, ease-in-out, entre otros.
```CSS
.elemento {
  animation-timing-function: ease-in-out;
}
```
### animation-fill-mode
Esta propiedad determina cómo se aplican los estilos del primer y último fotograma de una animación antes y después de que se ejecute. Los mas comunes son none(no aplicara estilos), forwards(mantendra los estilos del ultimo fotograma de la animacion), backwards(el elemento tomara los estilos del primer fotograma antes de que la animacion comienze a ejecutarse) y both(mezcla los dos anteriores).
```css
.elemento {
  animation-fill-mode: forwards;
}
```
## animation:
La propiedad animation en CSS es una forma abreviada de establecer múltiples propiedades de animación en un solo lugar. En lugar de declarar cada propiedad de animación por separado (como animation-name, animation-duration, etc.), puedes usar la propiedad animation para combinarlas todas en una sola línea.
```css
.elemento{
    animation: name duration timing-function delay iteration-count direction fill-mode;
}
```

