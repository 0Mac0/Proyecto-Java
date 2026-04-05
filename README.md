# Proyecto Java sin IDE

## Descripción
Aplicación básica desarrollada en Java sin utilizar IDE, compilada desde línea de comando con `javac` y ejecutada mediante la JVM con `java`.

## Objetivo
Solicitar datos de un vehículo y mostrarlos en pantalla usando entrada por teclado.

## Datos solicitados
- Marca
- Modelo
- Cilindrada
- Tipo de combustible
- Capacidad en pasajeros

## Requerimientos funcionales
- Solicitar marca.
- Solicitar modelo.
- Solicitar cilindrada.
- Solicitar tipo de combustible.
- Solicitar capacidad de pasajeros.
- Mostrar los datos ingresados por el usuario.

## Requerimientos no funcionales
- El programa debe desarrollarse sin una herramienta IDE.
- El código debe compilarse mediante `javac`.
- La ejecución debe realizarse mediante `java`.
- El proyecto debe documentarse en GitHub.
- El código debe incluir comentarios explicativos.

## Código fuente
```java
import java.util.Scanner;

public class VehiculoApp {
    public static void main(String[] args) {
        Scanner entrada = new Scanner(System.in);

        System.out.print("Ingrese la marca: ");
        String marca = entrada.nextLine();

        System.out.println("La marca es: " + marca);
    }
}



