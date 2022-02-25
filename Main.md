package com.company;

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        Scanner num = new Scanner(System.in);
        System.out.println("Enter first and second numbers to have some expressions: ");
        int first = num.nextInt(), second = num.nextInt();
        System.out.println("Enter the character to have some arithmetic expression: /,*,+,-,% ");
        char character = num.next().charAt(0);
        for(;;){
            if(character == '/'){
                System.out.println(Double.valueOf(first) / Double.valueOf(second));
            }
            else if(character == '*'){
                System.out.println(first * second);
                break;
            }
            else if(character == '+'){
                System.out.println(first + second);
                break;
            }
            else if(character == '-'){
                System.out.println(first - second);
                break;
            }
            else if(character == '!'){
                break;
            }
            else if(character == '%'){
                System.out.println(first % second);
                break;
            }
            else{
                System.out.println("Please enter the character that fits");
                break;
            }
        }
        System.out.println("Your program has done compilation");

    }
}
