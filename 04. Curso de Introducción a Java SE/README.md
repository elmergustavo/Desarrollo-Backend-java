## Tags Java Docs

![](https://static.platzi.com/media/user_upload/Screen%20Shot%202019-07-08%20at%204.29.49%20PM-fbd23e6a-b892-4d33-8ef4-4669d81b63dc.jpg)

## Bucle do While

Los bucles (ciclos) nos ayudan a ejecutar una parte de nuestro código una cantidad de veces hasta que se cumpla alguna condición y podamos continuar con la ejecución de nuestro código.

Existen diferentes bucles. Por ejemplo, el bucle do while:

do {
  // instrucciones
} while (condición);

Los ciclos evaluarán si la condición se cumple y cuando deje de hacerlo no ejecutarán más el código del ciclo. Las instrucciones son las encargadas de que esta condición cambie de verdadero a falso. De otra forma, si las instrucciones nunca cambian la condición, el ciclo no se detendrá nunca, lo que conocemos como un ciclo infinito.

La clase Scanner le permite a los usuarios contestar algunas preguntas para que nuestro programa actúe de una forma u otra. Para usarla solo debemos importar la clase Scanner de las APIs de desarrollo de Java:

import java.util.Scanner;

int response = 0;

Scanner sc = new Scanner(System.in);
response = Integer.valueOf(sc.nextLine());

## Operador Ternario y Bucle While

Vamos a crear el algoritmo con la lógica necesaria para encender una lampara, emitir un mensaje y detener las luces en algún momento.

El Bucle While nos ayuda a ejecutar una parte del código mientras una condición se cumpla. Recuerda tener mucho cuidado y asegurarte de que la condición del ciclo while cambie en algún momento, de otra forma, el ciclo no se detendrá nunca y sobrecargarás tu programa:

while (isTurnOnLight) {
  printSOS();
}

Los operadores ternarios son otra forma de evaluar condiciones, así como los condicionales IF y ELSE`:

// Operador Ternario:
isTurnOnLight = (isTurnOnLight) ? false : true;

// IF y ELSE:
if (isTurnOnLight) {
  isTurnOnLight = false;
} else {
  isTurnOnLight = true;  
}

## Bucle For
El Ciclo For también nos ayuda a ejecutar una parte de nuestro código las veces que sean necesarias para que se cumpla una condición. De hecho, el ciclo FOR nos da muchas ayudas para lograr este resultado de la forma más fácil posible:

// Estructura:
for (inicialización; condición; incremento o decremento;) {
  // Instrucciones
}

// En este ejemplo el mensaje de printSOS se
// ejecutará 10 veces:
for (int i = 1; i <= 10; i++) {
  printSOS();
}

![](https://static.platzi.com/media/user_upload/for-6916fd8b-c33f-4022-a9c0-4f9e5e7281fb.jpg)

## Break, Continue y Return

Antes de pasar a uno de nuestros temas más importantes del curso es importante que sepas todas las opciones que tienes para detener ciclos y así seguir controlando el flujo de tus programas.
Break

En Java esta sentencia la verás en dos situaciones especificamente:

   1. En un Switch: en esta situación break hace que el flujo del switch no continúe ejecutándose a la siguiente comparación, esto con el objetivo de que solo se cumpla una sola condición:

```java
switch (colorModeSelected){
	case "Light":
                System.out.println("Seleccionaste Light Mode");
                break;
        case "Night": //Ambar
                System.out.println("Seleccionaste Night Mode");
                break;
        case "Blue Dark":
                System.out.println("Seleccionaste Blue Dark Mode");
                break;
}
```
  2. Para salir de un bucle: Como acabamos de ver un break es capaz de detener el flujo en el código, en este caso detendremos el ciclo como tal terminándolo y haciendo que saltemos a la siguiente instrucción después del ciclo.
 
 ## Continue

Continue en cierto modo también nos va a servir para detener un ciclo pero en lugar de terminarlo como en el caso de break, este volverá directo a la condición.

## Return

Aunque en algunos lenguajes esta sentencia sirve como un tipo goto, dónde se rompe el flujo del programa la mejor forma de usarlo en Java es en Funciones, cuando lo usamos aquí siempre viene acompañado de un valor, el cuál indica el dato que se estará devolviendo en la función.

## Arrays
Los arreglos o arrays son objetos en los que podemos guardar más de una variable, una lista de elementos. Los arrays son de una sola dimensión, pero si guardamos arrays dentro de otros arrays podemos obtener arrays multidimensionales.

Los arrays se definen en código de las siguientes maneras:

```java
// 1. Definir el nombre de la variable y el tipo de datos
//  que va a contener, cualquiera de las siguientes dos
// opciones es válida:
TipoDato[] nombreVariable;
TipoDato nombreVariable[];

// 2. Definir el tamaño del array, la cantidad de elementos
// que podemos guardar en el array:
TipoDato[] nombreVariable = new TipoDato[capacidad];

// Array de dos dimensiones:
TipoDato[][] cities = new String[númeroFilas][númeroColumnas];
```

Ya que los arrays pueden guardar multiples elementos, la convención es escribir los nombres de las variables en plural.

