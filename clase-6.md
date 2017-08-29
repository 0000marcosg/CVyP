# Funciones

Las funciones nos permite separar el codigo en partes, volviendolo modular y reusable sin tener que repetirlo. Vuelve nuestro codigo mas facil de leer y ajustar.

Todo el tiempo estamos haciendo uso de funciones, por ejemplo cada vez que llamamos la funcion line\(\), rect\(\), ellipse\(\)  estamos haciendo uso de una fraccion de codigo escrita por los desarrolladores de Processing. Sin embargo, la creacion de funciones de usuario requiere varias elementos a tener en cuenta.

Los puntos importantes sobre porque deberiamos escribir nuestras propias funciones:

* Modularidad - Las funciones parten un codigo largo en varias partes peque;as, haciendolo mas entendible y manejable. Por ejemplo, una vez que desarrollamos la manera de dibujar cierto elemento, podemos redibujarlo todas las veces que queramos sin preocuparnos de sus caracteristicas.

* Reusabilidad - Las funciones nos permiten reusar una parte del codigo sin tener que escribirlo de nuevo, podemos llamarlo cuantas veces sea necesario.

### Definicion de una Funcion.

Una definicion de funcion consta de tres partes:

* Return Type
* Nombre de la funcion
* Argumentos

Y su sintaxis es la siguiente:

```Processing
returnType NombreFuncion(argumentos){

//Codigo a ejecutar

}
```



