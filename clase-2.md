# ¿Porque aprender a programar, a crear nuestro propio software?

* Las herramientas que encontramos en el mercado, puede que esten limitadas.
* Para poder desarrollar nuestras ideas sin limitaciones, necesitamos crear herramientas que se ajusten exactamente a nuestras necesidades.

### Elementos y practicas a tener en cuenta en la programacion:

> * La computadora no tiene intuicion.
>
> * Necesitamos una sintaxis correcta.
>
> * Pseudo-Codigo.
>
> * Proceso de "Desarrollo en aumento".

# Computacion Grafica, Pixeles y Coordenadas

El pixel, la unidad grafica minima dentro de una imagen debe ser colocado en su posicion a traves de coordenadas. Este sistema de coordenadas tiene similitudes y diferencias con el de Ejes Cartesianos que estamos mas habituados a ver.

![](http://4.bp.blogspot.com/-I3Cv5MXxni4/UEPdwzQPFPI/AAAAAAAAAAw/_OD6DbV-yWo/s1600/SISTEMA+DE+COORDENADAS+LINEAS+Y+RECTANGULARES+1.png)

En el sistema de Ejes Cartesianos tenemos una representacion grafica compuesta por dos ejes, uno horizontal llamado eje "x" y uno vertical llamado eje "y". La interseccion de los mismos es lo que conocemos como punto de origen y sus coordenadas son x = 0 e y = 0. En este caso el origen es el punto `D(0,0)`.

```
A(-5, 3)
B(6, 5)
C(4.5, -3.5)
```

Por otro lado, el sistema de coordenadas en processing \(y en general otros softwares de produccion de imagenes\) se maneja de manera diferente.

![](http://www.mywonderland.es/curso_js/images/processing/ejes.png)

La diferencia radica en que no existen pixeles negativos en pantalla, por lo cual el punto de origen, es decir donde se cruza el eje x y el eje y, se encuentra en la esquina superior izquierda de la ventana. Los valores de x aumentan a medida que nos movemos a la derecha y los valores de y aumentan a medidad que nos desplazamos hacia abajo.

# Puntos y Lineas

El elemento grafico mas simple que podemos dibujar con pixeles \(dejando afuera el punto\) es la lina, un segmento de recta que marca la distancia mas corta entre un punto A y un punto B.

El pseudo-codigo para indicar como dibujar una linea, definiendo la posicion del punto `A(30, 100) y punto B(60, 80)`:

```
Dibujar linea desde (30, 100) a (60, 80).
```

Sin embargo, cuando traducimos nuestro pseudo-codigo a la sintaxis correcta en processing el resultado es:

```
line(30, 100, 60, 80);
```

```
line(Ax, Ay, Bx, By);
```

`line` es el nombre de la funcion y los elementos dentro de los parentesis son conocidos como `argumentos`, los cuales son valores numericos separados entre si por comas.

Podemos pensar en la funcion como un comando y en los argumentos como los parametros en los que ese comando se va a ejecutar.

