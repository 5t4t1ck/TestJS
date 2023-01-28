
Variables y operaciones
1. Responde las siguientes preguntas:

    ¿Qué es una variable y para qué sirve?
    ¿Cuál es la diferencia entre declarar e inicializar una variable?
    ¿Cuál es la diferencia entre sumar números y concatenar strings?
    ¿Cuál operador me permite sumar o concatenar?

2. Determina el nombre y tipo de dato para almacenar en variables la siguiente información:

    Nombre
    Apellido
    Nombre de usuario de Abacom
    Edad
    Correo electrónico
    Mayor de edad
    Dinero ahorrado
    Deudas

3. Traduce a código JavaScript las variables del ejemplo anterior.
4. Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:

    Nombre completo (nombre y apellido)
    Dinero real (dinero ahorrado menos deudas)

Funciones
1. Responde las siguientes preguntas:

    ¿Qué es una función?
    ¿Cuándo me sirve usar una función en mi código?
    ¿Cuál es la diferencia entre parámetros y argumentos de una función?

2. Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:

const name = "Juan David";
const lastname = "Castro Gallego";
const completeName = name + lastname;
const nickname = "juandc";

console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");

Condicionales
1. Responde las siguientes preguntas:

    ¿Qué es un condicional?
    ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?
    ¿Puedo combinar funciones y condicionales?

2. Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:

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

3. Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).
Ciclos
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
