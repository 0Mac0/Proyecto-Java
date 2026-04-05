# Proyecto Java sin IDE

## Descripción
Aplicación básica desarrollada en Java sin utilizar una herramienta IDE. El programa es compilado desde la línea de comandos utilizando `javac` y ejecutado mediante la máquina virtual de Java (JVM) con el comando `java`.

## Objetivo
Solicitar datos de un vehículo mediante teclado y mostrar la información ingresada en pantalla.

## Datos solicitados
- Marca
- Modelo
- Cilindrada
- Tipo de combustible
- Capacidad en pasajeros

## Requerimientos funcionales
- Solicitar la marca del vehículo.
- Solicitar el modelo del vehículo.
- Solicitar la cilindrada.
- Solicitar el tipo de combustible.
- Solicitar la capacidad de pasajeros.
- Mostrar todos los datos ingresados por el usuario.

## Requerimientos no funcionales
- El programa debe desarrollarse sin una herramienta IDE.
- El código debe compilarse mediante `javac`.
- La ejecución debe realizarse mediante `java`.
- El proyecto debe estar documentado en GitHub.
- El código debe incluir comentarios explicativos.

## Código fuente
```java
import java.util.Scanner; // Importa la clase Scanner para leer datos desde teclado

public class VehiculoApp { // Declara la clase principal del programa

    public static void main(String[] args) { // Método principal
        Scanner entrada = new Scanner(System.in); // Captura datos del usuario

        String marca;
        String modelo;
        int cilindrada;
        String combustible;
        int pasajeros;

        System.out.print("Ingrese la marca: ");
        marca = entrada.nextLine();

        System.out.print("Ingrese el modelo: ");
        modelo = entrada.nextLine();

        System.out.print("Ingrese la cilindrada: ");
        cilindrada = entrada.nextInt();

        entrada.nextLine(); // Limpia buffer

        System.out.print("Ingrese el tipo de combustible: ");
        combustible = entrada.nextLine();

        System.out.print("Ingrese la capacidad de pasajeros: ");
        pasajeros = entrada.nextInt();

        System.out.println("La marca que ha ingresado es: " + marca);
        System.out.println("El modelo que ha ingresado es: " + modelo);
        System.out.println("La cilindrada que ha ingresado es: " + cilindrada);
        System.out.println("El tipo de combustible es: " + combustible);
        System.out.println("Tiene una capacidad de " + pasajeros + " pasajeros.");

        entrada.close();
    }
}


