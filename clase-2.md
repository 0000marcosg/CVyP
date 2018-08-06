# ¿Porque aprender a programar, a crear nuestro propio software?

* Las herramientas que encontramos en el mercado, puede que estén limitadas.
* Para poder desarrollar nuestras ideas sin limitaciones, necesitamos crear herramientas que se ajusten exactamente a nuestras necesidades.

### Elementos y practicas a tener en cuenta en la programación:

> * La computadora no tiene intuición.
>
> * Necesitamos una sintaxis correcta.
>
> * Pseudo-Código.
>
> * Proceso de "Desarrollo en aumento".

# Computación Gráfica, Pixeles y Coordenadas

El pixel, la unidad gráfica mínima dentro de una imagen debe ser colocado en su posición a través de coordenadas. Este sistema de coordenadas tiene similitudes y diferencias con el de Ejes Cartesianos que estamos mas habituados a ver.

![](http://4.bp.blogspot.com/-I3Cv5MXxni4/UEPdwzQPFPI/AAAAAAAAAAw/_OD6DbV-yWo/s1600/SISTEMA+DE+COORDENADAS+LINEAS+Y+RECTANGULARES+1.png)

En el sistema de Ejes Cartesianos tenemos una representación gráfica compuesta por dos ejes, uno horizontal llamado eje "x" y uno vertical llamado eje "y". La intersección de los mismos es lo que conocemos como punto de origen y sus coordenadas son x = 0 e y = 0. En este caso el origen es el punto `D(0,0)`.

```
A(-5, 3)
B(6, 5)
C(4.5, -3.5)
```

Por otro lado, el sistema de coordenadas en processing \(y en general otros softwares de producción de imágenes\) se maneja de manera diferente.

![](http://www.mywonderland.es/curso_js/images/processing/ejes.png)

La diferencia radica en que no existen pixeles negativos en pantalla, por lo cual el punto de origen, es decir donde se cruza el eje x y el eje y, se encuentra en la esquina superior izquierda de la ventana. Los valores de x aumentan a medida que nos movemos a la derecha y los valores de y aumentan a medida que nos desplazamos hacia abajo.

# Puntos y Lineas

El elemento gráfico mas simple que podemos dibujar con pixeles \(dejando afuera el punto\) es la linea, un segmento de recta que marca la distancia mas corta entre un punto A y un punto B.

El pseudo-código para indicar como dibujar una linea, definiendo la posición del punto `A(30, 100) y punto B(110, 120)`:

```
Dibujar linea desde (30, 100) a (110, 120).
```

Sin embargo, cuando traducimos nuestro pseudo-codigo a la sintaxis correcta en processing el resultado es:

```Processing
line(30, 100, 110, 120);
```

```
line(Ax, Ay, Bx, By);
```

`line` es el nombre de la función y los elementos dentro de los paréntesis son conocidos como `argumentos`, los cuales son valores numéricos separados entre si por comas.

Podemos pensar en la función como un comando y en los argumentos como los parámetros en los que ese comando se va a ejecutar.

`Ax - Posision x del punto A`

`Ay - Posision y del punto A`

`Bx - Posision x del punto B`

`By - Posision y del punto B`

Sin embargo, para que el sistema de coordenadas en processing funcione como queremos, debemos establecer el tamaño de la ventana.

Por defecto, Processing usa un tamaño de 100 pixeles por 100 pixeles. En este caso podemos usar una ventana de 200 por 200 para poder visualizar correctamente la linea.

```
size(200, 200);
line(30, 100, 110, 120);
```

### Resultado:

![](/assets/import.png)

> ### Ejercicio:
>
> En papel cuadriculado dibujar o diseñar una composición utilizando solo formas primitivas, estas son: rectángulos, elipses, lineas, puntos y triángulos.
>
> En una segunda hoja, escribir el pseudo-código para esa composición, tratando de descubrir los parámetros para todas las formas primitivas.



