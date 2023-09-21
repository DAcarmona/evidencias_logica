<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


<!-- Su documentación aquí -->

# Operadores aritméticos
Los operadores aritméticos en Java se utilizan para realizar operaciones matemáticas básicas. Los operadores aritméticos incluyen:

# Suma (+): se utiliza para sumar dos valores.
`int a = 5;
int b = 10;
int c = a + b; // c es igual a 15`

# Resta (-): se utiliza para restar un valor de otro.
`int a = 10;
int b = 5;
int c = a - b; // c es igual a 5`

# Multiplicación (*): se utiliza para multiplicar dos valores.
`int a = 5;
int b = 10;
int c = a * b; // c es igual a 50`

# División (/): se utiliza para dividir un valor entre otro.
`int a = 10;
int b = 5;
int c = a / b; // c es igual a 2`

# Módulo (%): se utiliza para obtener el resto de una división entre dos valores.
`int a = 10;
int b = 3;
int c = a % b; // c es igual a 1`

# Ejemplos
```
public class OperadoresAritmeticos {

    public static void main(String[] args) {
        int x = 10;
        int y = 5;

        // Suma
        int resultadoSuma = x + y;
        System.out.println("El resultado de la suma es: " + resultadoSuma);

        // Resta
        int resultadoResta = x - y;
        System.out.println("El resultado de la resta es: " + resultadoResta);

        // Multiplicación
        int resultadoMultiplicacion = x * y;
        System.out.println("El resultado de la multiplicación es: " + resultadoMultiplicacion);

        // División
        int resultadoDivisionEntera = x / y;
        System.out.println("El resultado de la división entera es: " + resultadoDivisionEntera);

        double resultadoDivisionDecimal = (double) x / y;
        System.out.println("El resultado de la división decimal es: " + resultadoDivisionDecimal);

        // Módulo
        int resultadoModulo = x % y;
        System.out.println("El resultado del módulo es: " + resultadoModulo);

        // Incremento
        x++;
        System.out.println("El valor de x después del incremento es: " + x);

        // Decremento
        y--;
        System.out.println("El valor de y después del decremento es: " + y);
    }
}
```

# Operadores de Asignación
En Java, los operadores de asignación son símbolos que se utilizan para asignar valores a las variables. Además de la asignación básica (=), Java ofrece otros operadores de asignación que combinan la asignación con una operación matemática. Estos operadores de asignación son útiles para simplificar y acortar el código en situaciones donde se realiza una operación aritmética y luego se asigna el resultado a una variable.

A continuación se describen los operadores de asignación disponibles en Java:

# Operador de asignación básico (=)
Se utiliza para asignar un valor a una variable. Por ejemplo:

int x = 5;

# Operador de asignación compuesta de suma (+=)
Se utiliza para sumar un valor a una variable y luego asignar el resultado a la misma variable. Por ejemplo:

x += 3; es equivalente a x = x + 3;

# Operador de asignación compuesta de resta (-=)
Se utiliza para restar un valor de una variable y luego asignar el resultado a la misma variable. Por ejemplo:

x -= 2; es equivalente a x = x - 2;

# Operador de asignación compuesta de multiplicación (*=)
Se utiliza para multiplicar una variable por un valor y luego asignar el resultado a la misma variable. Por ejemplo:

x *= 4; es equivalente a x = x * 4;

# Operador de asignación compuesta de división (/=)
Se utiliza para dividir una variable por un valor y luego asignar el resultado a la misma variable. Por ejemplo:

x /= 2; es equivalente a x = x / 2;

# Operador de asignación compuesta de módulo (%=)
Se utiliza para calcular el módulo de una variable por un valor y luego asignar el resultado a la misma variable. Por ejemplo:

x %= 3; es equivalente a x = x % 3;

# Operador de asignación compuesta de desplazamiento a la izquierda (<<=)
Se utiliza para desplazar los bits de una variable a la izquierda por un número de posiciones y luego asignar el resultado a la misma variable. Por ejemplo:

x <<= 2; es equivalente a x = x << 2;

# Operador de asignación compuesta de desplazamiento a la derecha (>>=)
Se utiliza para desplazar los bits de una variable a la derecha por un número de posiciones y luego asignar el resultado a la misma variable. Por ejemplo:

x >>= 1; es equivalente a x = x >> 1;

# Operador de asignación compuesta de desplazamiento a la derecha sin signo (>>>=)
Se utiliza para desplazar los bits de una variable a la derecha sin signo por un número de posiciones y luego asignar el resultado a la misma variable. Por ejemplo:

x >>>= 3; es equivalente a x = x >>> 3;

Es importante recordar que los operadores de asignación compuesta realizan la operación indicada y luego asignan el resultado a la misma variable. Por lo tanto, la variable se modifica en el lugar en el que se encuentra sin necesidad de declarar una nueva variable.

# Ejemplos
```
public class OperadoresAsignacion {

    public static void main(String[] args) {
        int a = 10;
        int b = 5;

        // Operador de asignación simple
        int c = a + b;
        System.out.println("c = " + c);

        // Operadores de asignación compuestos
        a += b; // equivalente a a = a + b;
        System.out.println("a = " + a);

        b -= 3; // equivalente a b = b - 3;
        System.out.println("b = " + b);

        c *= 2; // equivalente a c = c * 2;
        System.out.println("c = " + c);

        double d = 6.0;
        d /= 2; // equivalente a d = d / 2;
        System.out.println("d = " + d);

        int e = 7;
        e %= 3; // equivalente a e = e % 3;
        System.out.println("e = " + e);

        // Operador de concatenación de cadenas
        String s1 = "Hola";
        String s2 = "Mundo";
        String s3 = s1 + " " + s2;
        System.out.println(s3); // Hola Mundo

        // Operador de asignación ternario
        int edad = 18;
        String mensaje = (edad >= 18) ? "Eres mayor de edad" : "Eres menor de edad";
        System.out.println(mensaje);
    }
}
```
# Operadores de comparación
En Java, los operadores de comparación se utilizan para comparar dos valores y evaluar si una determinada condición es verdadera o falsa. A continuación, se muestran los operadores de comparación más comunes en Java, junto con sus nombres y descripciones:

# Operador de igualdad (==)
Nombre: Igual a Descripción: Comprueba si dos valores son iguales.

int a = 5;
int b = 7;
boolean resultado = (a == b); // false

# Operador de desigualdad (!=)
Nombre: No igual a Descripción: Comprueba si dos valores son diferentes.

int a = 5;
int b = 7;
boolean resultado = (a != b); // true

# Operador mayor que (>)
Nombre: Mayor que Descripción: Comprueba si el valor de la izquierda es mayor que el valor de la derecha.

int a = 5;
int b = 7;
boolean resultado = (a > b); // false

# Operador menor que (<)
Nombre: Menor que Descripción: Comprueba si el valor de la izquierda es menor que el valor de la derecha.

int a = 5;
int b = 7;
boolean resultado = (a < b); // true

# Operador mayor o igual que (>=)
Nombre: Mayor o igual que Descripción: Comprueba si el valor de la izquierda es mayor o igual que el valor de la derecha.

int a = 5;
int b = 7;
boolean resultado = (a >= b); // false

# Operador menor o igual que (<=)
Nombre: Menor o igual que Descripción: Comprueba si el valor de la izquierda es menor o igual que el valor de la derecha.

int a = 5;
int b = 7;
boolean resultado = (a <= b); // true

# Ejemplos
```
public class OperadoresComparación {

    public static void main(String[] args) {        
        int x = 5;
        int y = 10;
        boolean esIgual = (x == y); // Devuelve false, porque x no es igual a y.
        boolean esDiferente = (x != y); // Devuelve true, porque x es diferente a y.
        boolean esMenor = (x < y); // Devuelve true, porque x es menor que y.
        boolean esMayor = (x > y); // Devuelve false, porque x no es mayor que y.
        boolean esMenorIgual = (x <= y); // Devuelve true, porque x es menor o igual que y.
        boolean esMayorIgual = (x >= y); // Devuelve false, porque x no es mayor o igual que y.
    }
}
```

# Operadores lógicos
Los operadores lógicos en Java permiten realizar operaciones booleanas entre dos o más expresiones. Estos operadores son muy útiles en la toma de decisiones y en la evaluación de condiciones en una variedad de situaciones. Los tres operadores lógicos en Java son AND (&&), OR (||) y NOT (!).

Aquí te explico cómo funcionan estos operadores:

# AND (&&)
Este operador retorna true si ambas expresiones a su izquierda y derecha son verdaderas. Si al menos una de las expresiones es falsa, retorna false. Por ejemplo:

boolean a = true;
boolean b = false;
boolean resultado = a && b; // false

# OR (||)
Este operador retorna true si al menos una de las expresiones a su izquierda o derecha es verdadera. Si ambas expresiones son falsas, retorna false. Por ejemplo:

boolean a = true;
boolean b = false;
boolean resultado = a || b; // true

# NOT (!)
Este operador invierte el valor booleano de la expresión a su derecha. Si la expresión es verdadera, retorna false, y si es falsa, retorna true. Por ejemplo:

boolean a = true;
boolean resultado = !a; // false

Además, también es posible combinar estos operadores para formar expresiones booleanas más complejas, utilizando paréntesis para establecer el orden de evaluación. Por ejemplo:

boolean a = true;
boolean b = false;
boolean c = true;
boolean resultado = (a || b) && !c; // false

En este ejemplo, primero se evalúa la expresión (a || b), que retorna true. Luego, se aplica el operador NOT a la variable c, que es verdadera, resultando en false. Finalmente, se aplica el operador AND a los resultados anteriores, lo que resulta en false.

# Ejemplos
```
public class OperadoresLogicos {
    public static void main(String[] args) {
        int edad = 25;
        boolean esEstudiante = true;
        boolean esDiaLaboral = false;
        boolean esVacaciones = true;

        boolean resultado1 = (edad > 18) && esEstudiante;
        boolean resultado2 = esDiaLaboral || esVacaciones;
        boolean resultado3 = !esDiaLaboral;

        System.out.println("El resultado 1 es: " + resultado1);
        System.out.println("El resultado 2 es: " + resultado2);
        System.out.println("El resultado 3 es: " + resultado3);
    }
}
```
# Actividad 3: Ejercicios de operaciones básicas en Java.
1. Suma y multiplicación: Escribe un programa que solicite al usuario dos números enteros y luego imprima la suma y multiplicación de esos números.

2. Resta y división: Escribe un programa que tome dos números enteros ingresados por el usuario y calcule la resta y división de esos números.

3. Operaciones combinadas: Escribe un programa que solicite al usuario tres números enteros y realice las siguientes operaciones: suma de los tres números, multiplicación del primer número por el segundo y división del resultado entre el tercer número.

4. Operaciones con decimales: Escribe un programa que solicite al usuario dos números decimales y realice las siguientes operaciones: suma, resta, multiplicación y división.

5. Incremento y decremento: Escribe un programa que declare una variable entera y la inicialice con un valor. Luego, incrementa su valor en 1 y muestra el resultado. Después, decrementa su valor en 1 y muestra el resultado nuevamente.

6. Operador de asignación compuesta: Escribe un programa que declare una variable entera y la inicialice con un valor. Utiliza el operador de asignación compuesta para sumar 5 a la variable y luego mostrar su valor.

7. Operadores lógicos: Escribe un programa que tome dos valores booleanos ingresados por el usuario y muestre el resultado de las operaciones lógicas AND, OR y NOT entre esos valores.

8. Operador ternario: Escribe un programa que tome un número entero ingresado por el usuario y utilice el operador ternario para determinar si el número es positivo o negativo. Luego, muestra el resultado en la salida.

# Actividad
1.
```
import java.util.Scanner;

public class SumaMultiplicacion {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Ingrese el primer número entero: ");
        int numero1 = scanner.nextInt();

        System.out.print("Ingrese el segundo número entero: ");
        int numero2 = scanner.nextInt();

        int suma = numero1 + numero2;
        int multiplicacion = numero1 * numero2;

        System.out.println("La suma de los números es: " + suma);
        System.out.println("La multiplicación de los números es: " + multiplicacion);

        scanner.close();
    }
}
```
2.
```
import java.util.Scanner;

public class RestaDivision {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Ingrese el primer número entero: ");
        int numero1 = scanner.nextInt();

        System.out.print("Ingrese el segundo número entero: ");
        int numero2 = scanner.nextInt();

        int resta = numero1 - numero2;
        double division = (double) numero1 / numero2; // Usamos double para obtener decimales inexactos

        System.out.println("La resta de los números es: " + resta);
        System.out.println("La división de los números es: " + division);

        scanner.close();
    }
}
```
3.
```
import java.util.Scanner;

public class OperacionesCombinadas {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Ingrese el primer número entero: ");
        int numero1 = scanner.nextInt();

        System.out.print("Ingrese el segundo número entero: ");
        int numero2 = scanner.nextInt();

        System.out.print("Ingrese el tercer número entero: ");
        int numero3 = scanner.nextInt();

        int suma = numero1 + numero2 + numero3;
        int multiplicacion = numero1 * numero2;
        double division = (double) multiplicacion / numero3;

        System.out.println("La suma de los tres números es: " + suma);
        System.out.println("La multiplicación del primer número por el segundo es: " + multiplicacion);
        System.out.println("La división del resultado entre el tercer número es: " + division);

        scanner.close();
    }
}
```
4.
```
import java.util.Scanner;

public class OperacionesDecimales {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Ingrese el primer número decimal: ");
        double numero1 = scanner.nextDouble();

        System.out.print("Ingrese el segundo número decimal: ");
        double numero2 = scanner.nextDouble();

        double suma = numero1 + numero2;
        double resta = numero1 - numero2;
        double multiplicacion = numero1 * numero2;
        double division = numero1 / numero2;

        System.out.println("La suma de los números es: " + suma);
        System.out.println("La resta de los números es: " + resta);
        System.out.println("La multiplicación de los números es: " + multiplicacion);
        System.out.println("La división de los números es: " + division);

        scanner.close();
    }
}
```
5.
```
public class IncrementoDecremento {
    public static void main(String[] args) {
        int numero = 4; // Inicializamos la variable con un valor

        System.out.println("Valor inicial: " + numero);

        numero++; // Incremento en 1
        System.out.println("Después del incremento: " + numero);

        numero--; // Decremento en 1
        System.out.println("Después del decremento: " + numero);
    }
}
```
6.
```
public class AsignacionCompuesta {
    public static void main(String[] args) {
        int numero = 10; // Inicializamos la variable con un valor

        System.out.println("Valor inicial: " + numero);

        numero += 5; // Sumamos 5 usando el operador de asignación compuesta
        System.out.println("Valor después de sumar 5: " + numero);
    }
}
```
7.
```
import java.util.Scanner;

public class OperadoresLogicos {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Ingrese el primer valor booleano (true/false): ");
        boolean valor1 = scanner.nextBoolean();

        System.out.print("Ingrese el segundo valor booleano (true/false): ");
        boolean valor2 = scanner.nextBoolean();

        // Operación lógica AND
        boolean resultadoAnd = valor1 && valor2;
        System.out.println("Resultado de la operación AND: " + resultadoAnd);

        // Operación lógica OR
        boolean resultadoOr = valor1 || valor2;
        System.out.println("Resultado de la operación OR: " + resultadoOr);

        // Operación lógica NOT para el primer valor
        boolean resultadoNotValor1 = !valor1;
        System.out.println("Resultado de la operación NOT para el primer valor: " + resultadoNotValor1);

        // Operación lógica NOT para el segundo valor
        boolean resultadoNotValor2 = !valor2;
        System.out.println("Resultado de la operación NOT para el segundo valor: " + resultadoNotValor2);

        scanner.close();
    }
}
```
8.
```
import java.util.Scanner;

public class OperadorTernario {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Ingrese un número entero: ");
        int numero = scanner.nextInt();

        String resultado = (numero >= 0) ? "positivo" : "negativo";

        System.out.println("El número es " + resultado);

        scanner.close();
    }
}

```








