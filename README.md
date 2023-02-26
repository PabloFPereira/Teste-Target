# Teste-Target
teste em java para target sistemas

import java.util.Scanner;

public class Fibonacci {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Digite um número: ");
        int num = sc.nextInt();
        sc.close();
        
        int a = 0;
        int b = 1;
        int c = a + b;
        
        while (c <= num) {
            if (c == num) {
                System.out.println(num + " pertence à sequência de Fibonacci.");
                return;
            }
            a = b;
            b = c;
            c = a + b;
        }
        
        System.out.println(num + " não pertence à sequência de Fibonacci.");
    }
}
