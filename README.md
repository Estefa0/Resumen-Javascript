# Resumen-Javascript
En este archivo puedes encontrar un breve resumen de las funciones, variables que se utilizan en el lenguaje de JavaScript.


>### Variables y Operaciones

>###  ¿ Què es una variable y para què sirve? 
>Una variable es la representaciòn de un lugar que reservamos en memoria para guardar un valor. 
>El valor puede ser cualquier tipo de dato, inclusive objetos o funciones.

>###  ¿ Cuàl es la diferencia entre declarar e inicializar una variable?
>Una variable se declara para indicarle al programa a partir de un lugar empieza a existir, que nombre tendrá y que tipo de datos almacenará.
>La asignación de un valor inicial se llama inicalización. 
>
>//Declarar una variable
>`let nombre = 'Estefanía';`
>
>//Inicializar una variable 
>`nombre = 'Estefania';`

>###  ¿ Cuàl es la diferencia entre sumar nùmeros y concatenar strings?
>Sumar números es una operación matemática y concatenar es unir strings uno tras otro.
>
>Cuando yo sumo los números `1 + 3`, sin comillas `(“”)`. Js entiende que se tiene que sumar, ya que son números. El resultado seria `4`.
>
>cuando se  concatena `1 + “5”`, el resultado va a ser `“15”`, ya que el uno va a ser convertido como un `string`.
Yo le puedo especificar a js que el cinco sea un numero de la siguiente manera `Number(“5”)`, y de esto forma me podría aplicar la suma de manera correcta.

>###  ¿ Cuàl operador me permite sumar o concatenar?
>El operador `+` cuando se utiliza con strings y otros objetos, crea un solo string que contiene la concatenación de todos sus operandos.

>
>#Determina el nombre y tipo de dato para almacenar en variables la siguiente información:
>

`Nombre "string"`

`Apellido "string"`

`Nombre de usuario "string"`

`Edad "Number"`

`Correo electrònico "string"`

`Mayor de edad "Boolean"`

`Dinero ahorrado "Number"`

`Deudas "Number"`
>
>Código JavaScript con las variables anteriores 
>
`let name = 'Estefania';`

`let lastName = 'Zapata';`

`let user name = 'Ezapa';`

`let age= 25;`

`let mail = ezapa@gmail.com`

`let adult = true;`

`let savedMoney = 1500;`

`let debtMoney = 500000;`
>
>Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:
 >Nombre completo (nombre y apellido)
 
`lett name = 'Estefa';`

`let lastName = 'Zapata';`

`console.log ('Mi nombre completo es ${name} ${lastName}');`
>
>Dinero real (dinero ahorrado menos dudas)
>
`let savedMoney = 1000000;`

`let debtMoney = 500000;`

`let totalMoney = savedMoney - debtMoney;`

`console.log('el total de mi dinero actual es: $${totalMoney});`

>
>###  Funciones 
>

>###  ¿Qué es una función?
>Un conjunto de instrucciones que realiza una tarea o calcula un valor, pero para que un procedimiento califique como función, 
>debe tomar alguna entrada y devolver una salida donde hay alguna relación obvia entre la entrada y la salida.

>###  ¿Cuándo me sirve usar una función en mi código?
>Una función en javascript es similar a un procedimiento, un conjunto de instrucciones que realiza una tarea o calcula un valor,
> pero para que un procedimiento califique como función, debe tomar alguna entrada y devolver una salida donde no hay alguna relación obvia entre la entrada 
> y la salida.

>###  ¿Cuál es la diferencia entre parámetros y argumentos de una función?
>Los parámetros son los nombres que aparecen en la definición de una función, por su parte, los argumentos son los valores que le pasamos y que, por tanto, 
>recibe una función.

`function myFunction(parámetro1 + parámetro2)`

`{
 //... All my code here
 }`

`myFunction(argumento + argumento2);
//Al declarar las variables parámetro1 y parámetro2 estamos generando los argumentos de nuestra función.`

>
>Convierte el siguiente código en una función pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función?
>
>
`const name = "Estefania";`

`const lastname = "Zapata";`

`const completeName = name + lastname;`

`const nickname = "ezapa";`

`console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + ezapa + ".");`

>
>Se cambia el código de la funcion y queda de la siguiente manera:
>
>
`const name = "Estefania";`

`const lastname = "Zapata";`

`const completeName = name + lastname;`

`const nickname = "ezapa";`

`console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");`

`//My solution
function presentation(name, lastName, nickName){`

 `return console.log(Mi nombre completo es ${name} ${lastName}, pero prefiero que me digas ${nickName});
}
presentation("Estefania", "Zapata", "ezapa");`

>
>###  Condicionales 
>

>### ¿Qué es un condicional?
> Nos  permite introducir una situación que debe ser verdadero para que una acción suceda. Luego de esto escribiremos la acción a ejecutar 


>### ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?
>Esta el `if`: Este es el mas comun, ya que solo le decimos que ejecute una parte del código si sucede una acción.
>
>En adición a este, esta el `if else`, que puede ejecutar mas de una condición encadenada.
>
>También tenemos al `switch`: Este es parecido al `if else` pero es mas fácil de leer, sobre todo cuando hay condicionales encadenadas.

>### ¿Puedo combinar funciones y condicionales?
>Definitivamente, dentro de una función puede a ver condicionales y dentro de condicionales puede haber funciones.
>
>// Condiciones dentro de funciones
>
`function myFunction(parameterOne, parameterTwo)`

`{
  if(parameterOne > parameterTwo){
   @code
  }else{
    @code
  }
}`

>// Funciones dentro de condicionales

`if(variableOne < variableTwo){`

  `my-functionOne();`
  
`}else{`

  `my-functionTwo();
}`

>Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).
>
`const tipoDeSuscripcion = "basic";`
`switch (tipoDeSuscripcion) {`
   `case "Free":`
   
  `console.log("Solo puedes tomar los cursos gratis");`
       `break;
   case "Basic":`
   
     `console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
      break;`
   `case "Expert":`
      ` console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
       break;`
  ` case "Free":`
       `console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");`
     `  break;
}`
>RESPUESTA
>
`if(tipoDeSuscripcion === "Free"){`

  `console.log("Solo puedes tomar los cursos gratis");`
  
`} else if(tipoDeSuscripcion === "Basic"){`

  `console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");`
  
`} else if(tipoDeSuscripcion === "Expert"){`

  `console.log("Puedes tomar casi todos los cursos de Platzi durante un año");`
  
`} else{`

  `console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
}`

>### Listas
>### ¿Qué es un array?
>Es una lista, en ella se pueden guardar números, strings, objetos e incluso hasta otras listas.

>### ¿Qué es un objeto?
>Es un tipo de dato en JavaScript en donde podemos declarar varios títulos y sus respectivos valores. Incluso hasta pueden ser considerados listas.

>### ¿Cuándo es mejor usar objetos o arrays?
>Depende de la situación. Ya que un array se usa cuando solo quieres tener una lista de productos, por ejemplo. 
>Pero un objeto se usa cuando quieres saber el producto mas otros datos en relacion al producto. 
>En lo particular, una buena practica es usar un array de objetos.

>### ¿Puedo mezclar arrays con objetos o incluso objetos con arrays?
> En los objetos no puede haber arrays, pero si puede haber arrays donde dentro haya objetos.
> 
>### Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.

`var myArray = [10, 9, 8, 7, 6, 5, 4, 3, 2, 1]`

`function firstElement(ofThisArray){`

  `console.log(ofThisArray[0]);
}`

`firstElement(myArray);`

>### Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).

`var myArray = [10, 9, 8, 7, 6, 5, 4, 3, 2, 1]`

`function allElements(ofThisArray){`

  `ofThisArray.forEach(item => {`
    `console.log(item)
  })
}`

`allElements(myArray)`

>### Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).

`var myObject = {product: "Buzz Lightyear", price: 43, category: "toys"}`

`function allElements(ofThisObject){`

  `let objectValues = Object.values(myObject)`
  
  `objectValues.forEach(item => {`
    `console.log(item)`
  `})`
`}`

`allElements(myObject);`
