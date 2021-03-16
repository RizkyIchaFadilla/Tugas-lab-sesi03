# Tugas-lab-sesi03
package com.xsis.example;
import java.util.Scanner;
import java.util.Random;


public class Main {

    public static void main(String[] args) {
        Random rand = new Random();
        int n = rand.nextInt(100);
        int tebakan;


        Scanner input = new Scanner(System.in);
        System.out.println("Guess a magic number between 0 and 100\n");


        do {
            System.out.println("Enter your guess : \n");
            tebakan = input.nextInt();

            if (tebakan == n) {
                System.out.println("Yes,the number is : " + n);
            } else if (tebakan < n) {
                System.out.println("Your guess is to low \n");
            } else if (tebakan > n) {
                System.out.println("Your number is too high \n");
            }
        } while (tebakan != n);
    }
}




