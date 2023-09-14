Las variables en Rust son **inmutables** pordefecto, es decir que una vez se le de
un valor a la variable, el valor de la variableno cambiara,
para hacer que una variable sea mutable seagrega la palabra reservada **mut**

```Rust
let mut guess;
```
La funcion **String::new()** crea un nuevo objeto de tipo **String**,
el cual es un tipo de dato que es provisto por la biblioteca estandar de Rust,
y que es un tipo de dato que es crecido en memoria, es decir que puede almacenar
una cantidad de texto que no se conoce en tiempo de compilacion, sino en tiempo de ejecucion.

Los dos puntos **::** indican que **new()** es una funcion asociada al tipo de dato **String**, es decir que es una funcion estatica.

```Rust
let mut guess = String::new();
```

El metodo **read_line()** es un metodo de la biblioteca estandar de Rust, que es un metodo de entrada de texto, que permite al usuario ingresar texto en la consola, y que almacena el texto ingresado en la variable **guess**.

La referencia **&** indica que la variable **guess** es una referencia, y que es pasada como argumento a la funcion **read_line()**.
Una referencia es una forma de referirse a un valor sin tener que poseerlo, y que permite pasar valores a funciones sin tener que transferir la propiedad de los mismos.
Por ejemplo, si se pasa una variable a una funcion, la variable se transfiere a la funcion, y ya no se puede usar en el codigo que sigue a la llamada de la funcion, pero si se pasa una referencia a la funcion, la variable se puede seguir usando despues de la llamada a la funcion.

La referencia **&mut** indica que la variable **guess** es una referencia mutable, es decir que se puede modificar el valor de la variable a la que se hace referencia.
Por defecto las referencias son inmutables, por lo que se debe agregar la palabra reservada **mut** para que la referencia sea mutable.

```Rust
 io::stdin()
        .read_line(&mut guess)
```

El metodo **expect()** es un metodo del tipo de dato **Result**, que es un tipo de dato que es provisto por la biblioteca estandar de Rust, y que es un tipo de dato que representa un valor que puede ser de dos tipos, **Ok** o **Err**, y que es usado para manejar errores.
El metodo **expect()** es usado para manejar el error que puede ocurrir al leer una linea de texto, y que imprime el mensaje de error que se le pasa como argumento.

```Rust
.expect("Failed to read line");
```
```