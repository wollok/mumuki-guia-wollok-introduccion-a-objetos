El motivo por el cual Caperucita sabe responder a algunos mensajes y otros no, es porque cuando definimos el objeto que la representa, indicamos qué y cómo responder.

Un objeto se define con un nombre y una serie de porciones de codigo que se denominan metodos, que indican qué mensajes puede responder y describen la manera en que lo hacen.

Por ejemplo, para que Caperucita pueda responder a las preguntas anteriores, tiene que estar definido lo siguiente:

```scala
object caperucita {

  method vasACasaDeTuAbuelita() {
    return true
  }
  
  method cuantoPesas() {
    return 80 
  }
  
  method comoEstas() {
    return "Contenta de venir a una clase en la facultad"
  }
  
  method deQueColorEsLoQueLlevasEnLaCanasta() {
    return "rojo" 
  }
  
}
```

Como podemos ver, en primer lugar esta definido el objeto caperucita y luego cada uno de los metodos para responder a las preguntas que le hicimos.

Tomemos nota de los elementos sintacticos que utilizamos:
* la palabra object delante del nombre del objeto
* {} para encerrar lo que estamos definiendo de ese objeto, en este ejmplo, todo.
* la palabra method delante del nombre de cada metodo del objeto.
* () al final del nombre, tal cual como lo usamos al enviar el mensaje
* nuevamente {} para encerrar todo lo que abarca cada metodo.
* la palabra return para indicar cual es la respuesta que se debe retornar en cada caso
* Como detalle, a las cadenas de caracteres las encerramos entre "", los valores de verdad sin nada y los numeros tal cual son.
 
___

Si quisieramos que funcione el mensaje que anteriormente daba error, podriamos definir un nuevos metodo al objeto caperucita. Seria posible y sencillo, pero pensandolo mejor no tiene mucho sentido que sea Caperucita quien responda, sino otro personaje...  

Definir un objeto para representar al espejo magico, que sepa decir quien es la mas bella del reino y nos responda que es la reina malvada

