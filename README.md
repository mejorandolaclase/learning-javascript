# Aprendiendo JavaScript

*Guía para aprender JavaScript para [Comunidad Mejorando.la](//cursos.mejorando.la)*

![logo](img/logo_aprendiendoJS.png)

Esta guía está diseñada para conocer el lenguaje JavaScript, uno de los
más importantes de nuestra época, ya que podemos emplearlo en navegadores
web, en servidores, en procesos, e incluso en microcontroladores y
drones.

Cualquier estudiante de [Mejorando.la](//mejorando.la) puede colaborar
en esta guía, añadiendo su conocimiento y contribuyendo a la comunidad.

Siéntete libre de *forkear* este repositorio y enviar *pull-request* para que
podamos conseguir entre todos, ser la mayor comunidad referencia en español
sobre JavaScript

## Tabla de contenidos
1. [Definición de variables](#definicion-de-variables)
2. [Tipos de variables](#tipos-de-variables)

## Definición de variables
Las variables son usadas para almacenar datos. Las variables pueden almacenar cualquier
tipo de datos como números, *Strings* (cadenas) o datos más complejos como objetos.

Para definir una variable en JavaScript, usamos la palabra reservada `var` y un nombre (identificador),
por ejemplo:
```js
var miVariable;
```

Los nombres (identificadores) pueden comenzar con los caracteres `$`, `_`; estar formadas por letras
y no pueden contener espacios. Los nombres de variables son sensibles a mayúsculas, por lo cual
`miDato` y `MyDato` son variables distintas.

```js
// Identificadores validos
var _miVariable;
var $miOtraVriable;
var mi1234Variable;

// Identificadores invalidos
var 123;
var mi dato;
var {}dato;
```

Podemos asignar un valor a la variable en la misma linea. Por ejemplo: a
continuación asignamos el string "Hola Mundo" a la variable `miDato`:
```js
var miDato = 'Hola Mundo';
```

También podemos declarar la variable en una linea y la asignación en otra.
```js
var miDato;
miDato = 'hola Mundo';
```

Después de declarar una variable, podemos asignarle un valor y después acceder al mismo.
Por ejemplo, el siguiente código almacena un *string* (cadena de caracteres) en la variable
`miDato` y después asignarle su valor a otra variable llamada `miNuevoDato`:
```js
var miDato = 'Hola Mundo';
var miNuevoDato = miDato + ' k ase!';
```

Debemos dar nombres (identificadores) descriptivos a nuestras variables, de manera que tengamos
una pista tanto del uso como del valor de dicha variable.

**[Volver arriba](#tabla-de-contenidos)**

## Tipos de variables
JavaScript usa distintos tipos de datos para manejar como se almacenan
a una variable. El tipo de variable determina que operaciones podemos
usar con ella, como bucles o ejecuciones. La siguiente lista describe los
tipos de variables que utilizaremos en nuestros desarrollos:

### String
Este tipo de variable almacena una cadena de caracteres o *Strings*. El
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
