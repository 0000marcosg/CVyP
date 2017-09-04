# Array

Pensemos en una variable como un elemento capaz de seguir los cambios de informacion dentro de un espacio en la memoria del programa en un periodo de tiempo. Un array es exactamente lo mismo, la diferencia es que en lugar de seguir una pieza particular de informacion un array se encarga de seguir a un conjunto de piezas.

![](/assets/array.png)

Debemos pensar en el array como una lista de variables. Por lo tanto, como lista es importante para dos cosas: en primer lugar sigue los cambios de cada uno de los elementos almacenados en ella, y numero dos, la lista mantiene el orden de los elementos que la componen.

En una array, cada elemento posee un unico valor de indice, designado por un numero entero que marca su posicion en la lista \(elemento \#1, elemento \#2, elemento \#3, etc.\) . En todos los casos, el nombre del array refiere a la lista completa, y para acceder a un elemento en particular lo hacemos a traves de su numero de indice.

La manera en la que este indice se organiza, como se ve en la imagen de mas abajo es el siguiente: Si tenemos un array de 10 elementos o posiciones, el primero de ellos va a ser nombrado con el indice 0 y el ultimo con el indice 9. Podria llamarnos la atencion el hecho de que el primer elemento sea nombrado con el indice 0, pero refiere a que existe cero distancia entre el comienzo del array y el primer elemento.

### ![](/assets/array2.png)

### Declaracion de un array

Si tomamos como referencia que para crear una variable debiamos indicar un tipo de dato \(int, float, bool, etc.\) debemos saber que no existe diferencia con el respecto a las arrays. Sin embargo, la sintaxis es diferente.

Creamos un array colocanto un par de parentesis rectos \( \[ \] \) luego del tipo de dato y el nombre del array.

Por ejemplo, un array de numero enteros seria definida de la siguiente manera:

```
int [] arrayDeEnteros;
```

Al igual que una variable, el nombre es totalmente trivial y puede ser cualquier cosa que queramos.

Una cosa a tener en cuenta con las arrays es que su tamaño no puede cambiar. Una vez que la declaremos con 10 posiciones, no puede pasar a tener 11 lugares en un determinado momento \(esto es en el caso de processing, en otros lenguajes existen las arrays dinamicas\).

