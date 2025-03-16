import java.util.Scanner;
import  java.util.Arrays;
//GERONIMO SALVO
public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int xsd;
        int amer =10;
        int cort =20;
        int cap =40;




//aca es lo primero que mustra al usuario
    System.out.println("BIENVENIDOS A CAFETERIA  GS");

    System.out.println("¿Como te llamas ?");
        String nombre = scanner.nextLine();
        System.out.println("");

    System.out.println("Elija una opcion para continuar");
        do {
            System.out.println("Menu:");
            System.out.println("1. Americano");
            System.out.println("2. Cortado");
            System.out.println("3. Capuchino");
            System.out.println("4. Salir");
            xsd = scanner.nextInt();
            System.out.println("cuantos quieres llevar ?");
            int cant = scanner.nextInt();


            switch (xsd) {

                case 1:
                    System.out.println("Elegiste "+cant + " cafe americano con costo total  "+ (amer * cant) + " gracias por elegirnos "+nombre);
                    break;
                case 2:
                    System.out.println("Elegiste "+ cant +" cortado con un costo de $"+ (cort*cant)+ " Gracias por elegirnos "+ nombre);
                    break;
                case 3:
                    System.out.println("Elegiste "+cant+" capuchino con un costo de $"+ (cap*cant)+ " Gracias por elegirnos "+ nombre);
                    break;
                case 4:
                    System.out.println("Gracias por elegirnos");
                default:
                    System.out.println("·············");
                    System.out.println("·············");
                    System.out.println("·············");
                    System.out.println("·············");
            }

            System.out.println();
        } while (xsd != 4);
        scanner.close();

    }
}
