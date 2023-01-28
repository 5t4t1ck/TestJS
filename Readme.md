
# Variables y operaciones

## Responde las siguientes preguntas:

1. ¿Qué es una variable y para qué sirve?

* Espacio en memoria que podemos guardar información, depende del tipo y estructura de datos que soporte el lenguaje de programación donde se esté utilizando.

2. ¿Cuál es la diferencia entre declarar e inicializar una variable?

* Declarar es crear una variable e inizializar es asignarle un valor.
    
3. ¿Cuál es la diferencia entre sumar números y concatenar strings?

* Incrementar el valor de las variables y concatenar es unir cadenas de caracteres.

4. ¿Cuál operador me permite sumar o concatenar?

* El operador que nos permite sumar o concatenar es "+". Este operador nos permite sumar números cuando lo usamos con números. Pero cuando los strings, lo que hace es unir (concatenar) ambos strings.

2. Determina el nombre y tipo de dato para almacenar en variables la siguiente información:

* Nombre: string
* Apellido: string
* Nombre de usuario de Abacom: string (@statick_ds)
* Edad: number
* Correo electrónico string (dsaavedra88@gmail.com)
* Mayor de edad: boolean
* Dinero ahorrado: number
* Deudas: number

3. Traduce a código JavaScript las variables del ejemplo anterior.

````
let nombre = "Milton";
let apellido = "Labanda";
let username = "mlabanda";
let edad = 35;
let email = "dsaavedra88@gmail.com";
let esMayorDeEdad = true;
let dineroAhorrado = 1000;
let deudas = 200;
````

4. Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:

Nombre completo (nombre y apellido)
Dinero real (dinero ahorrado menos deudas)

````
let nombreCompleto = nombre + " " + apellido;
let saldoIgual = dineroAhorrado - deudas;
````

# Funciones.

## Responde las siguientes preguntas:

1. ¿Qué es una función?

* Las funciones nos permiten encapsular (guardar) bloques de código para ser reutilizaods y ejecutados en el futuro.

2. ¿Cuándo me sirve usar una función en mi código?

* Nos sirve cuando tenemos variables o bloques de código muy parecidos (con camb ios que podrían ser parámetros y argumentos) que podemos encapsular para reutilziar más de una vez en el futuro.

3. ¿Cuál es la diferencia entre parámetros y argumentos de una función?

* Las funciones reciben parámetros cuando las creamos. Y les enviamos argumentos cuando las ejecutamos.

2. Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:

````
const name = "Diego";
const lastname = "Saavedra";
const completename = name + lastname;
const nick = "statick";

console.log("Mi nombre es " + completename + ", pero prefiero que me digas " + nick + ".");
````
````
function nombreCompleto(name, lastName) {
    return name + " " + lastName;
}

function saludo(name, lastname, username) {
    const completeName = nombreCompleto(name, lastname);
    console.log("Mi nombre es " + completeName +", pero prefiero que me digas " + username + "·");
}

saludo(name, lastname, nick);

````
# Condicionales
## Responde las siguientes preguntas:

1. ¿Qué es un condicional?

* Son la forma en que ejecutamos un bloque de código u otro dependiendo de alguna condición o validación.

2. ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?

* If (else y else if): El condicional if (con else y elseif) nos permite hacer validaciones completamente distintas (si asi lo deseamos) en cada validación o condiconal.
* Switch: La sentencia switch en todos los cases se comparan con la misma variable o condición que definimos en el switch.

3. ¿Puedo combinar funciones y condicionales?

* Sí, las funciones pueden encapsular cualquier bloque de código, incluyendo los condicionales.

4. Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:
````
const tipoDeSuscripcion = "Basic";

switch (tipoDeSuscripcion) {
   case "Free":
       console.log("Solo puedes tomar los cursos gratis");
       break;
   case "Basic":
       console.log("Puedes tomar casi todos los cursos de Abacom durante un mes");
       break;
   case "Expert":
       console.log("Puedes tomar casi todos los cursos de Abacom durante un año");
       break;
   case "ExpertPlus":
       console.log("Tú y alguien más pueden tomar TODOS los cursos de Abacom durante un año");
       break;
}
````

````
if (tipoDeSuscripcion == "Free") {
    console.log("Solo puedes tomar los cursos gratis");
} else if (tipoDeSuscripcion == "Basic") {
    console.log("Puedes tomar casi todos los cursos de Abacom durante un mes");
} else if (tipoDeSuscripcion == "Expert") {
    console.log("Puedes tomar casi todos los cursos de Abacom durante un año");
} else if (tipoDeSuscripcion == "ExpertPlus") {
    console.log("Tú y alguien más pueden tomar TODOS los cursos de Abacom durante un año");
} else {
    console.log("No existe ese tipo de suscripción");
}

````

3. Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).
Ciclos.


````
if (tipoDeSuscripcion == "Free") {
    console.log("Solo puedes tomar los cursos gratis");
    }
if (tipoDeSuscripcion == "Basic"){
    console.log("Puedes tomar casi todos los cursos de Abacom durante un mes");
}
if (tipoDeSuscripcion == "Basic") {
    console.log("Puedes tomar casi todos los cursos de Abacom durante un mes");
} 
if (tipoDeSuscripcion == "Expert") {
    console.log("Puedes tomar casi todos los cursos de Abacom durante un año");
} 
if (tipoDeSuscripcion == "ExpertPlus") {
    console.log("Tú y alguien más pueden tomar TODOS los cursos de Abacom durante un año");
} 
if !(tipoDeSuscripcion == "Free") || !(tipoDeSuscripcion == "Basic") || !(tipoDeSuscripcion == "Expert") || (tipoDeSuscripcion == "ExpertPlus") {
    console.log("No existe ese tipo de suscripción");
}

````


1. Responde las siguientes preguntas

    ¿Qué es un ciclo?
    ¿Qué tipos de ciclos existen en JavaScript?
    ¿Qué es un ciclo infinito y por qué es un problema?
    ¿Puedo mezclar ciclos y condicionales?

2. Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:

for (let i = 0; i < 5; i++) {
    console.log("El valor de i es: " + i);
}

for (let i = 10; i >= 2; i--) {
    console.log("El valor de i es: " + i);
}

3. Escribe un código en JavaScript que le pregunte a los usuarios cuánto es 2 + 2. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.

    💡 Pista: puedes usar la función prompt de JavaScript.

Listas
1. Responde las siguientes preguntas:

    ¿Qué es un array?
    ¿Qué es un objeto?
    ¿Cuándo es mejor usar objetos o arrays?
    ¿Puedo mezclar arrays con objetos o incluso objetos con arrays?

2. Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.
3. Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).
4. Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).
