# Aprendiendo JavaScript

*Guía para aprender JavaScript para [Comunidad Platzi](https://platzi.com/clases)*

![logo](img/logo_aprendiendoJS.png)

Esta guía está diseñada para conocer el lenguaje JavaScript, uno de los
más importantes de nuestra época, ya que podemos emplearlo en navegadores
web, en servidores, en procesos, e incluso en microcontroladores y
drones.

Cualquier estudiante de [Platzi](https://platzi.com) puede colaborar
en esta guía, añadiendo su conocimiento y contribuyendo a la comunidad.

Siéntete libre de *forkear* este repositorio y enviar *pull-request* para que
podamos conseguir entre todos, ser la mayor comunidad referencia en español
sobre JavaScript

## Tabla de contenidos
1. [Definición de variables](#definicion-de-variables)
2. [Tipos de variables](#tipos-de-variables)

## Definición de variables
Las variables son usadas para almacenar temporalmente y acceder a datos
desde nuestros ficheros JavaScript. Las variables pueden almacenar cualquier
tipo de datos como números, *Strings* o datos más complejos como objetos.

Para definir una variable en JavaScript, usamos `var` y le damos un nombre,
por ejemplo:
```js
var miDato;
```

Podemos asignar un valor a la variable en la misma linea, por ejemplo, a
continuación asignamos el string "Hola Mundo" a la variable `miDato`:
```js
var miDato = "Hola Mundo";
```

También podemos hacerlo en dos líneas:
```js
var miDato;
miDato = "hola Mundo";
```

Después de declarar una variable, podemos usar su nombre para asignarle un
valor y acceder al mismo. Por ejemplo, el siguiente código almacena un string en
la variable `miDato` y después lo usa asignándoselo a una nueva variable `miNuevoDato`,
a la que añadimos más texto.
```js
var miDato = "Hola Mundo";
var miNuevoDato = miDato + " Ola k ase!";
```

Debemos dar nombres descriptivos a nuestras variables, de manera que más
adelante en nuestros desarrollos, sepamos que dato estamos almacenando de
manera más sencilla.

Una variable siempre ha de comenzar por una letra, `$` o `_` y no puede
contener espacios. Los nombres de variables son sensibles a mayúsculas, por
ejemplo no es lo mismo `miDato` que `MyDato`, son variables diferentes.

**[Volver arriba](#tabla-de-contenidos)**

## Tipos de variables
JavaScript usa distintos tipos de datos para manejar como se almacenan
a una variable. El tipo de variable determina que operaciones podemos
usar con ella, como bucles o ejecuciones. La siguiente lista describe los
tipos de variables que utilizaremos en nuestros desarrollos:

### String
Este tipo de variable almacena caracteres como palabras o *Strings*. El
dato es especificado con comillas simples o dobles. Ej:
```js
var miString = "Esto es un String";
var otroString = 'Esto es otro texto';
```

### Number
Este tipo de dato almacena un valor númerico. Los `Number` son usados
para contar, hacer cálculos y comparaciones. Estos son algunos ejemplos:
```js
var miEntero = 1;
var miDecimal = 1.33;
```

### Boolean
Este tipo de dato almacena un bit que indica `true` o `false`. Los booleanos
suelen ser usados para indicaciones de estados. Por ejemplo, asignas
`false` a una variable al inicio de un código y cuando finaliza, se le
asigna `true`. Los siguientes ejemplos definen variables como `true` y `false`
```js
var yes = true;
var no = false;
```

### Array
Un array es una serie de elementos separados, todos almacenados bajo un mismo
nombre de variable. Los elementos en el array pueden ser accedidos por un
índice (empezando en 0), usando `array[indice]`. El siguiente ejemplo
crea un array con 3 elementos y accede al primero de ellos, el cual tiene
índice 0:
```js
var arr = ["uno", "dos", "tres"];
var primero = arr[0] //"uno"
```

### Object
JavaScript tiene la habilidad de crear y usar objetos literales. Cuando
los usamos, podemos acceder a sus valores y funciones usando la sintaxis `objecto.propiedad`.
El siguiente ejemplo muestra como crear y acceder a propiedades en un objeto:
```js
var objeto = {
  "nombre": "John Freddy",
  "ocupacion": "CEO de Mejorando.la",
  "edad": "desconocida"
};
var nombre = objecto.nombre; //"John Freddy"
```

### Null
A veces no tenemos un valor que almacenar en una variable, bien porque no
ha sido creado o bien porque no lo vamos a utilizar. Para estas ocasiones
usamos el valor `null`. Usar `null` es mejor que usar `0` o un string vacío
`""`, porque así permitimos valores válidos para la variable. Usando `null`, no asignamos
ningún valor y podemos comprobar la variable dentro de nuestro código:
```js
var nuevaVariable = null;
```

>**Nota**

>JavaScript es un lenguaje sin tipado. No necesitamos especificar
en el código que tipo de dato es cada variable. El intérprete automáticamente
advierte el tipo de dato correcto para cada una.
Es más, puedes asignar a una variable de un tipo el valor de otro tipo de dato.
Por ejemplo, el siguiente código define una variable de tipo `String` y despues
le asigna un valor `Number` entero:
```js
var id = "testID";
id = 1;
```




**[Volver arriba](#tabla-de-contenidos)**

## Licencia
#### (The MIT License)

Copyright (c) 2014 Carlos Azaustre

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
