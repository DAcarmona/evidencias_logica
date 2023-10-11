<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 10 


<!-- Su documentación aquí -->
#  Actividad: Prueba, ejecución y explicación de ejercicios de lógica de programación.
Selecciona dos ejercicios de la sesión 10, impleméntalos, ejecútalos y proporciona una explicación detallada de cada uno

## Ejercicios de Lógica de Programación
1. Crear un programa en Java para calcular el interés de un CDT
Un CDT (Certificado de Depósito a Término) es un producto financiero en el que un inversor deposita una cantidad de dinero en un banco por un plazo determinado y a cambio recibe una tasa de interés fija. Al final del plazo, el inversor recupera su inversión inicial más los intereses generados. Aquí hay un ejemplo de cómo crear un programa en Java para calcular el interés de un CDT:
```
import java.util.Scanner;
import java.text.DecimalFormat;

public class Main {
    public static void main(String[] args) {
        DecimalFormat decimalFormat = new DecimalFormat("#,###");
        Scanner scanner = new Scanner(System.in);

        System.out.println("Bienvenido al calculador de CDT!");

        // Pedir al usuario que ingrese los datos del CDT
        System.out.print("Ingrese el monto del depósito: ");
        double montoDeposito = scanner.nextDouble();

        System.out.print("Ingrese la tasa de interés anual (%): ");
        double tasaInteresAnual = scanner.nextDouble();

        System.out.print("Ingrese el plazo en meses: ");
        int plazoMeses = scanner.nextInt();

        // Calcular el interés y el monto total al vencimiento
        double tasaInteresMensual = tasaInteresAnual / 12 / 100;
        double interesMensual = montoDeposito * tasaInteresMensual;
        double montoTotalVencimiento = montoDeposito + (interesMensual * plazoMeses);

        // Mostrar el resumen del CDT
        System.out.println("Resumen del CDT:");
        System.out.println("- Monto del depósito: $" + decimalFormat.format(montoDeposito));
        System.out.println("- Tasa de interés anual: " + tasaInteresAnual + "%");
        System.out.println("- Plazo en meses: " + plazoMeses);
        System.out.println("- Interés mensual: $" + interesMensual);
        System.out.println("- Monto total al vencimiento: $" + decimalFormat.format(montoTotalVencimiento));
    }
}
```
# Analisis
Se pone el mensaje en consola, "bienvenido al calculador",
se ingresan los datos para imprimir y calcular con double. el monto,tasa,interés,plazo, se calcula tasa mensual igual monto depósito por la tasa de interés mensual,se imprime los datos porconsola, llamndo el resumen del CDT.
llamando el monto del depósito mas el decimal format, tsa interés anual mas porcentaje,plazo meses mas meses,intrés mensual, monto total al vencimiento mas decimal format





