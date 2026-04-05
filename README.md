# Proyecto Java sin IDE
![Logo AIEP](evidencias/AIEP.png)

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

    public static void main(String[] args) { // Método principal: aquí inicia la ejecución del programa
        Scanner entrada = new Scanner(System.in); // Crea un objeto Scanner para capturar datos del usuario

        String marca; // Variable para almacenar la marca del vehículo
        String modelo; // Variable para almacenar el modelo del vehículo
        int cilindrada; // Variable para almacenar la cilindrada del vehículo
        String combustible; // Variable para almacenar el tipo de combustible
        int pasajeros; // Variable para almacenar la capacidad de pasajeros

        System.out.print("Ingrese la marca: "); // Muestra un mensaje para pedir la marca
        marca = entrada.nextLine(); // Lee la marca ingresada por el usuario

        System.out.print("Ingrese el modelo: "); // Muestra un mensaje para pedir el modelo
        modelo = entrada.nextLine(); // Lee el modelo ingresado por el usuario

        System.out.print("Ingrese la cilindrada: "); // Muestra un mensaje para pedir la cilindrada
        cilindrada = entrada.nextInt(); // Lee un número entero para la cilindrada

        entrada.nextLine(); // Limpia el buffer para evitar errores al leer texto después de un entero

        System.out.print("Ingrese el tipo de combustible: "); // Muestra un mensaje para pedir el combustible
        combustible = entrada.nextLine(); // Lee el combustible ingresado por el usuario

        System.out.print("Ingrese la capacidad de pasajeros: "); // Muestra un mensaje para pedir pasajeros
        pasajeros = entrada.nextInt(); // Lee un número entero para la capacidad de pasajeros

        System.out.println("La marca que ha ingresado es: " + marca); // Muestra la marca ingresada
        System.out.println("El modelo que ha ingresado es: " + modelo); // Muestra el modelo ingresado
        System.out.println("La cilindrada que ha ingresado es: " + cilindrada); // Muestra la cilindrada ingresada
        System.out.println("El tipo de combustible es: " + combustible); // Muestra el combustible ingresado
        System.out.println("Tiene una capacidad de " + pasajeros + " pasajeros."); // Muestra la capacidad de pasajeros

        entrada.close(); // Cierra el objeto Scanner
    }
}
```

## Compilación y ejecución
```bash
javac VehiculoApp.java
java VehiculoApp

Ingrese la marca: Toyota
Ingrese el modelo: Yaris
Ingrese la cilindrada: 1500
Ingrese el tipo de combustible: Bencina 93 oc
Ingrese la capacidad de pasajeros: 5

La marca que ha ingresado es: Toyota
El modelo que ha ingresado es: Yaris
La cilindrada que ha ingresado es: 1500
El tipo de combustible es: Bencina 93 oc
Tiene una capacidad de 5 pasajeros.
```

## Estructura del proyecto
```text
ProyectoJava/
├── VehiculoApp.java
├── README.md
├── documentacion_proceso.md
├── historias_usuario.md
└── evidencias/
    ├── compilacion y ejecucion.png
    ├── CRONOGRAMA.png
    ├── Codigo aplicado.png
    ├── Ubicacion archivo.png
```
