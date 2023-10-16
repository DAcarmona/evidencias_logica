<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 11 


<!-- Su documentación aquí -->
# Actividad: Ejercicios de Lógica de Programación
1. Basándose en el algoritmo 1 de la sesión 11, aplicar la siguiente variante: Dado un conjunto de números enteros, se debe determinar si existe algún número que aparezca más de una vez. Si es así, se deben imprimir todos los números que aparezcan más de una vez.

2. Desarrollar un algoritmo que realice la conversión de binario a decimal.

# Ejercicio # 1

```
import java.util.ArrayList;

public class Ejercicio1 {

    public static void main(String[] args) {
        int[] numeros = {1, 2, 3, 4, 5, 2,3,4,7,8,7,9,10,4,5,10};
        
        ArrayList<Integer> numerosRepetidos = new ArrayList<>();

        for (int i = 0; i < numeros.length; i++) {
            for (int j = i + 1; j < numeros.length; j++) {
                if (numeros[i] == numeros[j] && !numerosRepetidos.contains(numeros[i])) {
                   add(numeros[i]);
                }
            }
        }

       
        if (!numerosRepetidos.isEmpty()) {
            System.out.println("Números repetidos: " + numerosRepetidos);
        } else {
           
         System.out.println("No hay ningún número repetido");
        }
    }
}

```

# Ejercicio # 2

```
public class Ejercicio1 {

    public static void main(String[] args) {
        
        String numeroBinario = "111"; 

        int numeroDecimal = 0;

        for (int i = numeroBinario.length() - 1; i >= 0; i--) {
            if (numeroBinario.charAt(i) == '1') {
                int potencia = numeroBinario.length() - 1 - i;
                numeroDecimal += Math.pow(2, potencia);
            }
        }

        System.out.println("El número decimal es: " + numeroDecimal);
    }
}


```





