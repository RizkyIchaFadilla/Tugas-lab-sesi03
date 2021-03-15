# Tugas-lab-sesi03
package com.xsis.example;
import java.util.Scanner;


public class Main
{

    public static void main(String[] args)
    {

        int n = (int)(Math.random() * 100);


        Scanner input = new Scanner(System.in);
            System.out.println("What number do you want to guess [0-100] : ");
            n = input.nextInt();

        int tebakan = -1 ;

        while (tebakan != n )
        {
            System.out.println("Enter your guess : ");
            tebakan = input.nextInt();


        if (tebakan == n )
            System.out.println("Yes,the number is : " + n);
        else if ( tebakan > n )
            System.out.println("Your guess is to high");
        else
            System.out.println("Your number is too low");
        }


    }
}
