<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 7 


<!-- Su documentación aquí -->
# Actividad: Ejecicios Array - ArrayList
## 1. En parejas, probar, analizar y explicar el funcionamiento de los siguientes ejemplos de Array y ArrayList.
### Ejemplo Array

``` import java.util.Arrays;

public class EjercicioArray {

    public static void main(String[] args) {
        // Crear un array de números enteros
        int[] numeros = {5, 2, 10, 7, 1};

        // Imprimir el array original
        System.out.println("Array original: " + Arrays.toString(numeros));

        // Calcular la suma de los elementos del array
        int suma = 0;
        for (int i = 0; i < numeros.length; i++) {
            suma += numeros[i];
        }
        System.out.println("La suma de los elementos es: " + suma);

        // Encontrar el número más grande en el array
        int maximo = numeros[0];
        for (int i = 1; i < numeros.length; i++) {
            if (numeros[i] > maximo) {
                maximo = numeros[i];
            }
        }
        System.out.println("El número más grande es: " + maximo);

        // Ordenar el array en orden ascendente
        Arrays.sort(numeros);
        System.out.println("Array ordenado: " + Arrays.toString(numeros));
    }
}
```

### Ejemplo Array list

```import java.util.ArrayList; 
import java.util.Scanner;

public class AppNotas {

  public static void main(String[] args) {

    ArrayList<String> notas = new ArrayList<>();
    
    Scanner scan = new Scanner(System.in);

    while(true) {

      System.out.println("1. Agregar nota");  
      System.out.println("2. Mostrar notas");
      System.out.println("3. Salir");

      int opcion = scan.nextInt();

      if (opcion == 1) {
        agregarNota(notas, scan);  
      } else if (opcion == 2) {
        mostrarNotas(notas);
      } else {
        break;
      }

    }

  }
```

  ```public static void agregarNota(ArrayList<String> notas, Scanner scan) {
    
    System.out.println("Ingrese el titulo de la nota:");
    String titulo = scan.nextLine();
    
    System.out.println("Ingrese el contenido de la nota:");
    String contenido = scan.nextLine();
    
    notas.add(titulo + " - " + contenido);

  }

  public static void mostrarNotas(ArrayList<String> notas) {

    for(String n : notas) {
      System.out.println(n);
    }

  }

}
```
2. Crear un ejemplo de Array y otro de ArrayList para visualizar sus diferencias.

# Actividad :

```public class EjemploArray {
    public static void main(String[] args) {
        
        int[] numeros = {1, 2, 3, 4, 5};

        System.out.println("Elementos del array:");
        for (int i = 0; i < numeros.length; i++) {
            System.out.println("Número en la posición " + i + ": " + numeros[i]);
        }
    }
}
```
```import java.util.ArrayList;

public class EjemploArrayList {
    public static void main(String[] args) {
        // Crear un ArrayList de cadenas (Strings)
        ArrayList<String> nombres = new ArrayList<>();

        // Agregar elementos al ArrayList
        nombres.add("Duber");
        nombres.add("Jasmin");
        nombres.add("Carlos");

        // Acceder y mostrar elementos del ArrayList
        System.out.println("Elementos del ArrayList:");
        for (String nombre : nombres) {
            System.out.println(nombre);
        }

        // Obtener el tamaño del ArrayList
        int tamano = nombres.size();
        System.out.println("Tamaño del ArrayList: " + tamano);

        // Eliminar un elemento del ArrayList
        nombres.remove("Jasmin");
        System.out.println("Después de eliminar a Jasmin:");
        for (String nombre : nombres) {
            System.out.println(nombre);
        }
    }
}
```





