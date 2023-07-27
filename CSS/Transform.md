# Transform
El tema de "transform" en CSS es una poderosa propiedad que permite modificar la posición, tamaño y rotación de elementos HTML de una manera eficiente y sin afectar al flujo normal del documento. Esta propiedad es especialmente útil para realizar transformaciones visuales en elementos, como rotaciones, escalados, sesgados y translaciones.
```css
.elemento {
  transform: función(transformación);
}
```
# 2D

## translate()
La función translate() mueve un elemento en el plano 2D según las coordenadas especificadas en los ejes X e Y. Puedes utilizar valores en píxeles (px), porcentajes (%) o unidades de vista (vw y vh) para definir la distancia del desplazamiento.
```css
.box:hover{
    transform: translate(100px, 200px);
    transform: translate(200px);
    transform: translateY(200px);
}
```
## rotate()
La función rotate() rota un elemento en torno a un punto de referencia (normalmente el centro del elemento) en el sentido de las agujas del reloj. El ángulo de rotación se especifica en grados (deg). Un valor positivo produce una rotación en sentido horario, y un valor negativo produce una rotación en sentido antihorario.
```css
.elemento {
  transform: rotate(45deg);
}
```
## scale()
Con la función scale(), puedes aumentar o disminuir el tamaño de un elemento en el plano 2D. Puedes especificar valores para escalar tanto en el eje X como en el Y. Un valor de 1 mantiene el tamaño original, mientras que valores mayores que 1 aumentan el tamaño y valores entre 0 y 1 lo reducen.
```css
.elemento {
    transform: scale(2);
    transform: scalex(2);
    transform: scaley(2); 
    transform: scale(2,2);
    transform: scale(0.5,0.5);
}
```
## skew()
La función skew() permite inclinar o sesgar un elemento. Puedes especificar ángulos de inclinación en grados (deg) para los ejes X e Y. Un valor positivo producirá una inclinación hacia la derecha, mientras que un valor negativo la inclinará hacia la izquierda.
```css
.elemento {
    transform: skew(20deg, -10deg);
    transform: skew(45deg);
    transform: skew(-45deg);
}
```
## matrix()
La función matrix() se utiliza para aplicar transformaciones de escala, sesgado, rotación y translación en una sola línea de código. 
```css
elemento {
  transform: matrix(a, b, c, d, e, f);
}
```

Cada parámetro de la función matrix() representa un valor numérico que define cómo se llevará a cabo la transformación. Estos valores son los siguientes:

* a y d: Controlan la escala en los ejes X e Y, respectivamente. Si ambos valores son iguales a 1, el elemento no experimenta escala en ese eje. Valores mayores que 1 aumentan la escala, mientras que valores entre 0 y 1 reducen la escala.

* b y c: Representan el sesgado (skew) en los ejes X e Y, respectivamente. Estos valores determinan la inclinación o deformación del elemento. Si ambos valores son 0, no hay sesgado. Valores positivos generan un sesgado hacia la derecha, y valores negativos hacia la izquierda.

* e y f: Controlan la translación (desplazamiento) en los ejes X e Y, respectivamente. Estos valores desplazan el elemento a lo largo de esos ejes. Si ambos valores son 0, el elemento permanece en su posición original.
```css
.elemento{
    /* matrix(scaleX(),skewY(),skewX(),scaleY(),translateX(), translateY() */
    transform: matrix(2,.45,.45,2,200,20); 
}
```

## transform-origin
 Permite definir el punto de referencia alrededor del cual se aplican las transformaciones. Por defecto, el punto de referencia es el centro del elemento. Puedes cambiar este punto utilizando valores como top, left, right, bottom, center, coordenadas (x e y), porcentajes, entre otros.
 ```CSS
 .elemento {
  transform-origin: top left;
}
```
# 3D
Las transformaciones en 3D (rotateX(), rotateY() y rotateZ()) son funciones de transformación específicas que se utilizan para aplicar rotaciones alrededor de los ejes X, Y y Z, respectivamente. 
## rotateX()
Esta función permite rotar un elemento alrededor del eje X en el espacio 3D. Un valor positivo de ángulo (deg) realizará una rotación en sentido antihorario, mientras que un valor negativo realizará una rotación en sentido horario.
```css
.elemento {
  transform: rotateX(180deg); /* Realiza una rotación de 180 grados alrededor del eje X */
}
```
## rotateY()
Con esta función, puedes rotar un elemento alrededor del eje Y en el espacio 3D. Un valor positivo de ángulo (deg) hará una rotación en sentido antihorario, y un valor negativo hará una rotación en sentido horario.
```css
.elemento {
  transform: rotateY(180deg); /* Realiza una rotación de 180 grados alrededor del eje Y */
}
```
## rotateZ()
La función rotateZ() te permite rotar un elemento alrededor del eje Z en el espacio 3D. Al igual que con las otras funciones, un valor positivo de ángulo (deg) realizará una rotación en sentido antihorario, mientras que un valor negativo realizará una rotación en sentido horario.
```css
.elemento {
  transform: rotateZ(180deg); /* Realiza una rotación de 180 grados alrededor del eje Z */
}
```

## Relación entre perspective y rotateY()
La propiedad perspective tiene un efecto importante cuando se utiliza junto con la función rotateY(). Al establecer una perspectiva en un contenedor (elemento padre), se crea un punto de fuga en el que los elementos hijos con transformaciones 3D se ven afectados por la perspectiva y parecen moverse en el espacio tridimensional en relación con la ubicación del observador.

Al aplicar una rotación rotateY() a un elemento hijo dentro del contenedor con perspectiva, el elemento parece girar sobre su eje Y, como si estuviera volteándose de un lado a otro, y esta rotación se verá afectada por la perspectiva definida en el contenedor padre.
```css
.contenedor {
  perspective: 1000px; /* Perspectiva con una distancia de 1000 píxeles */
}

.elemento {
  transform: rotateY(180deg); /* Realiza una rotación de 180 grados alrededor del eje Y */
}
```