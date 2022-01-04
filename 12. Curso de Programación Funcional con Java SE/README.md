## ¿Qué es una función en Java?


    En la programación funcional una función es un tipo de dato que opera sobre un dato X y genera un dato Y.

    Una función es una serie de pasos parametrizados. Las funciones pueden generar o no un resultado.

    Las funciones se definen, almacenan o declaran bajo demanda como cualquier otro tipo de dato.

    Pueden definirse funciones con respecto a otras funciones
    esPar(x) = !esNon(x).

    Pueden definirse funciones con respecto a sí mismas (Recursividad).

    Pueden existir funciones que toman a otras funciones como parámetros:
    f(x, g(x)) = x2 * (gx)

## Funciones como ciudadanos de primera clase



    Tradicionalmente en Java y cualquier otro lenguaje de programación que no es naturalmente funcional, las funciones son métodos, meros procedimientos que se utilizan para reciclar cálculos u operaciones.

    Cuándo se hace referencia a funciones como ciudadanos de primera clase se hace alusión a las funciones como elementos primordiales del lenguaje. En Java los ciudadanos de primera clase han sido siempre los objetos.

    Cuándo el profesor hace referencia a funciones como ciudadanos de primera clase se refiere claramente a la capacidad que confiere Java 8 en adelante para tratar las funciones como Tipos de datos, que pueden declararse, recibirse cómo parámetros o enviarse (retornarse) cómo resultados.

## Funciones puras


    Función pura: determinista (resultado predecible). Fácil de probar. Su resultado será siempre el mismo al recibir siempre los mismos parámetros. No dependen del contexto, siempre generará el mismo resultado y no generará efectos secundarios, es decir no afectará datos de entrada ni otros datos relativos a otros flujos de datos. No dependen del estado del sistema.

    Función impura: no determinista. Dependen del estado del sistema. Dependen de su contexto. Pueden generar efectos secundarios, es decir, pueden afectar a otros flujos de datos o verse afectadas por otros flujos de datos subyacentes. No son predecibles.

    Una función pura puede invocar a una función pura, pero no a una impura. Si una función pura invoca a una impura se transformará entonces en una función impura ya que la naturaleza de la impura hará impredecible el resultado de la función pura, ya sea por resultado o por los efectos secundarios y contexto que impliquen la función pura.

## Entendiendo los efectos secundarios
Un efecto secundario es todo cambio observable desde fuera del sistema es un efecto secundario. Los efectos secundarios son inevitables (porque terminan siendo necesarios), algunos ejemplos son:


    CRUD sobre archivos
    CRUD sobre una base de datos
    Enviar/Recibir una llamada de red
    Alterar un objeto/variable usada por otras funciones.

Sin embargo, se deben reducir los efectos secundarios, porque ayuda a tener una mejor estructura del código (favoreciendo la generación de funciones puras, la modularidad y la testeabilidad).

## Funciones de orden mayor
funcion de orden mayor toma una funcion como otro parametro o retorna una funcion

## Funciones lambda

Función = Tiene un nombre.
Lambda = Función que no tiene un nombre.

Por qué usar lambdas?
Es un comportamiento único.
Es una regla que solo se requiere en un lugar.
Es una función muy simple (1 línea).

* https://platzi.com/blog/feature-lambda/

