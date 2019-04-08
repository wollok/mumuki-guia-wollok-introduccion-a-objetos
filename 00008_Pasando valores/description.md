Complementando lo anterior, algo que a veces estamos tentados de hacer es pretender modificar directamente desde afuera los atributos de un objeto, sin enviar mensajes.

Por ejemplo, si queremos modificar la edad de la abuela para que valga 100, no podemos hacer esto:

* `ム abuela edad = 100`
* `ム abuela.edad = 100`
* `ム abuela.edad() = 100`

La solución, nuevamente es enviarle un mensaje. 
Si el sentido del mensaje fuera cumplir años :birthday:, y lo que buscamos es que la edad de la abuela pase a ser 100 a partir de saber que tiene 99, podríamos definirlo así:

``` wolok
object abuela {
  var edad = 99
  method cumplirAnios(){
    edad = edad + 1
  }
}
```

Cuando le enviamos el mensaje `cumplirAnios()`, la edad de la abuela queda modificada, tiene un año más.

Pero pensemos... ¿cómo hacemos para que la edad de la abuela quede en el valor en que nosotros querramos, sin importar su valor previo, y que lo podamos modificar cuantas veces como se nos de la gana?

La clave es poder pasar valores adicionales cuando enviamos un mensaje, es lo que se llama **parámetros**.

* `ム abuela.edad(100)`
* `ム abuela.edad(15)`

Y para que esto funcione, el método tiene que estar definido con una variable para hacer referencia al parámetro que recibe.

> A ver si lo podés hacer solo

> Definí el método `edad(nuevaEdad)` que asigne el valor que se _pasa como parámetro_ en el atributo `edad`.




