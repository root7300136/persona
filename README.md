# persona
tambien sus materias






import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Ingrese el nombre de la persona:");
        String nombre = scanner.nextLine();

        System.out.println("Ingrese el apellido de la persona:");
        String apellido = scanner.nextLine();

        System.out.println("Ingrese la edad de la persona:");
        int edad = scanner.nextInt();
        scanner.nextLine(); // Consumir el salto de línea pendiente

        System.out.println("Ingrese la profesión de la persona:");
        String profesion = scanner.nextLine();

        int cedula = 0;
        String materias = "";

        if (profesion.equalsIgnoreCase("maestro")) {
            System.out.println("Ingrese la cédula del maestro:");
            cedula = scanner.nextInt();
            scanner.nextLine(); // Consumir el salto de línea pendiente

            System.out.println("Ingrese las materias que imparte el maestro:");
            materias = scanner.nextLine();
        }

        // Imprimir los datos ingresados
        System.out.println("Nombre: " + nombre);
        System.out.println("Apellido: " + apellido);
        System.out.println("Edad: " + edad);
        System.out.println("Profesión: " + profesion);

        if (profesion.equalsIgnoreCase("maestro")) {
            System.out.println("Cédula: " + cedula);
            System.out.println("Materias que imparte: " + materias);
        }

        scanner.close(); // Cerrar el scanner para liberar recursos
    }
}
