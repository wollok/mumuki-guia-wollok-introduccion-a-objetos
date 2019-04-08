Bien!

Efectivamente, ahora vemos que el lobo está en la casa de la abuela, lo que confirma que había realizado correctamente lo que le pedimos con el mensaje andaALaCasaDeLaAbuela(). Algo hizo el lobo en reacción a dicho mensaje, que provocó que una misma pregunta respondiera cosas diferentes antes y despues de haberlo enviado. De alguna manera, se las ingenio para recordar su ubicacion en cada momento y permitir que vaya cambiando.

Vamos a ampliar lo que veníamos diciendo de los mensajes:
- Como ya habiamos visto, si el mensaje es una pregunta, nos responde.
- Lo que agregamos ahora, es que si el mensaje es una indicacion, hace lo que le decimos y no nos responde nada. Decimos que es un mensaje con "efecto".

Para que todo esto sea posible, el objeto que representa al lobo puede estar definido de esta manera

```scala
object lobo {
   var ubicacion = "bosque"
   
   method dondeEstas() {
      return ubicacion
   }
   
   method andaALaCasaDeLaAbuela() {
      ubicacion = "casa de la abuela"
   }
  }
```

Para recordar en todo momento el lugar donde esta, el lobo tiene una variable denominada ubicacion. Su valor inicial es el bosque, pero en el metodo andaALaCasaDeLaAbuela su valor se modifica. 
Como el metodo dondeEstas en vez de un valor puntual devuelve la variable ubicacion, lo que obtenemos como respuesta es el valor referenciado en esa variable en el momento en que le preguntemos.

Las variables son identificadores que en un momento hacen referencia a un valor y en otro momento pueden hacer referencia a otro.
La manera en que una variabla cambia su valor es mediante una asignación.

Tomemos nota de la sintaxis:
- con var declaramos una variable
- el = indica una asignación; a su izquierda va la variable y a su derecha lo que queremos asignar en ella.
- al declarar una variable le podemos asignar un valor inicial
- para indicar que el método no retorna nada no hacemos nada especial, simplemente no aparece el return.

___

Volvamos a definir un objeto que represente al espejo mágico, que al igual que el ejercicio anterior nos diga que la mas bella del reino es la reina malvada, pero luego que le indicamos que blancanieves crecio nos responda que la mas bella del reino es precisamente blancanieves.



  
  