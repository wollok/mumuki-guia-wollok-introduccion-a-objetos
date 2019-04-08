abuela.edad

No funciona, porque a falta de parentesis no se lo interpreta como un mensaje.

abuela.edad()

Tampoco funciona, porque no está definido el método edad()

Esto nos lleva a ver que las variables no se pueden acceder desde afuera del objeto, decimos que son "privadas". 
Si queremos preguntarle a la abuela cuantos años tiene, sí o sí tenemos que definir un método para ello. 
Vamos a denominar "encapsulamiento" a esta característica de un objeto de ser el único que puede manipular sus propias variables. En otras palabras, retomando la nocion de entender a los objetos como sujetos, podemos decir que cada objeto mantiene oculta su intimidad y los demas objetos lo respetan.

De todas maneras, no seria difícil hacer el método que nos permitan preguntarle la edad a la abuela.

Podríamos denominarlo como quisiéramos, cuantosAñosTenes(), decimeTuEdad(), tiempoTranscurridoDesdeElNacimiento(), pero para simplificar sin perder expresividad y también por convención vamos a llamarlo directamente edad()

¿Lo hacemos?


