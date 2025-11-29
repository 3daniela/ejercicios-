public class ContadorSimple {
    public static void main(String[] args) {
        int i = 1;
        
        do {
            System.out.println("Número: " + i);
            i++;
        } while (i <= 5);
    }
}



public class ConversorMoneda {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        char otra;
        double tipoCambio = 18.50; // pesos por dólar
        
        do {
            System.out.print("Ingresa cantidad en dólares: ");
            double dolares = scanner.nextDouble();
            double pesos = dolares * tipoCambio;
            
            System.out.println("$" + dolares + " dólares = $" + pesos + " pesos");
            System.out.print("¿Convertir otra cantidad? (s/n): ");
            otra = scanner.next().charAt(0);
            
        } while (otra == 's');
        
        scanner.close();
    }
}

import java.util.Scanner;

public class Suma {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a, b;
        
        do {
            System.out.print("Número 1: ");
            a = sc.nextInt();
            System.out.print("Número 2: ");
            b = sc.nextInt();
            System.out.println("Suma: " + (a + b));
        } while (a != 0);
        
        sc.close();
    }
}

import java.util.Scanner;

public class Menu {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int op;
        
        do {
            System.out.println("1. Hola 2. Adiós 3. Salir");
            op = sc.nextInt();
            
            if (op == 1) System.out.println("Hola");
            if (op == 2) System.out.println("Adiós");
        } while (op != 3);
        
        sc.close();
    }
}

public class Regresivo {
    public static void main(String[] args) {
        int cont = 3;
        
        do {
            System.out.println(cont);
            cont--;
        } while (cont > 0);
        
        System.out.println("¡Ya!");
    }
}

public class Pares {
    public static void main(String[] args) {
        int num = 2;
        
        do {
            System.out.println(num);
            num += 2;
        } while (num <= 6);
    }
}

import java.util.Scanner;

public class Saludo {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        char resp;
        
        do {
            System.out.println("¡Hola!");
            System.out.print("¿Otro saludo? (s/n): ");
            resp = sc.next().charAt(0);
        } while (resp == 's');
        
        sc.close();
    }
}

import java.util.Scanner;

public class Calculadora {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        char resp;
        
        do {
            System.out.print("Número: ");
            int a = sc.nextInt();
            System.out.print("Número: ");
            int b = sc.nextInt();
            System.out.println("Suma: " + (a + b));
            
            System.out.print("¿Continuar? (s/n): ");
            resp = sc.next().charAt(0);
        } while (resp == 's');
        
        sc.close();
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);

        double nota;
        do {
            System.out.print(" Ingresa una nota entre 0 y 5: ");
            nota = s.nextDouble();
        } while(nota < (double)0.0F || nota > (double)5.0F);

        System.out.println("Nota válida: " + nota);
    }
}

