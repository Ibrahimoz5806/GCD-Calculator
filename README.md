# GCD-Calculator

import java.util.Scanner;

public class gcd_calculator {




    public static int find_gcd (int number1, int number2){

        int gcd = 1;

        for (int i = 1; i<=number1 && i<=number2; i++){


            if ((number1 % i == 0) && (number2 % i ==0)){

                gcd = i;


            }

        }

        return gcd;

    }

    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        System.out.println("First number: ");
        int first_number = scanner.nextInt();

        System.out.println("Second number: ");
        int second_number = scanner.nextInt();

        System.out.println("Result = " + find_gcd(first_number, second_number));


    }



}
