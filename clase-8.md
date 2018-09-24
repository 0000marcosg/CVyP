### Imagenes Externas - Clases

Para trabajar con imagenes externas en Processing, debemos comprender primero un concepto que aparece en los lenguajes de programacion de tipo OOP (Object Oriented Programming) como es el caso de Processing.

Cuando hablamos de programacion orientada a objetos nos estamos refiriendo a un tipo de programacion en la cual se estructuran tipos de datos complejos (dejando afuera a los datos primitivos como int, float o char), este tipo de datos son conocidos como Clase.

Una clase, en programacion, corresponde a un tipo de dato definido por el usuario y corresponde a un conjunto de campos y metodos.

Si pensamos en las variables como un elemento capaz de cambiar de valor durante su ejecucion y cuyo valor podemos reutilizar en cualqiuer momento y pensamos en las funciones como una abstraccion de codigo que permite modular un programa, podemos definir a la Clase como la suma de estos dos elementos.

Podemos hacer una analogia entre las clases en programacion y las clases que componen a los elementos de nuestro mundo fisico:

![](/assets/17import.png)

Por ejemplo, la clase Manzana contiene dos campos, o variables, una para su color y otra para su peso, y por otra parte posee tres metodos o funciones que definen su manera de manifestarse.

Sus campos o propiedades en relacion con sus metodos o funciones son las que definen el comportamiento del objeto manzana en su universo.

Debemos pensar en la Clase como la definicion de un Objeto. Un objeto existe cuando sus campos o propiedades son completados y sus funciones ejecutadas.
La clase PImage

La clase PImage es una clase definida por Processing que nos permite cargar y modificar imagenes.

```
// Declaramos la clase PImage;
PImage img;

void setup() {
    size(320,240);

    //Creamos una nueva instancia de la clase PImage, es decir, crear un objeto con las caracteristicas
    img = loadImage( " mysummervacation.jpg " );
}

void draw() {

    background(0);

    //La funcion image() muestra una instancia de PImage en la ventana de Processing.
    image(img,0,0);
}
```

    Ejercicio:
    Crear una composicion que utilice mas de una imagen y elementos de dibujo vistos hasta ahora.
