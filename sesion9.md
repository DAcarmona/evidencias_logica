<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 9 


<!-- Su documentación aquí -->

## Actividad: Prueba y ejecución de ejercicios de lógica de programación.
Prueba y ejecución de ejercicios de lógica de programación para mejorar las habilidades de resolución de problemas y pensamiento crítico.

```
import java.util.Arrays;

public class Mediana {

    public static void main(String[] args) {
        // Definimos el conjunto de números
        int[] numeros = {2, 3, 4, 7, 8};

        // Ordenamos el conjunto de números
        Arrays.sort(numeros);

        // Calculamos la mediana
        int mediana;
        if (numeros.length % 2 == 0) {
            // Si la cantidad de elementos es par, la mediana es el promedio de los dos elementos centrales
            int indice1 = numeros.length / 2 - 1;
            int indice2 = numeros.length / 2;
            mediana = (numeros[indice1] + numeros[indice2]) / 2;
        } else {
            // Si la cantidad de elementos es impar, la mediana es el elemento central
            int indice = numeros.length / 2;
            mediana = numeros[indice];
        }

        // Imprimimos la mediana
        System.out.println("La mediana es: " + mediana);
    }
}
```



