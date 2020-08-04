# Calculator
Java code where you can do basic calculator functions with 2 or 4 different numbers. 

/**
 * Tharaneshan Sivabalan
 */

import java.util.Scanner;

/**
 * Goes to calculator according to users input.
 * Pre:
 * Post: Calls the method.
 */

public class Calculator {
  public static void main(String[]args){
    int choice;
    
    Scanner input = new Scanner(System.in);
    System.out.println("What kind of calculator would you like 1(normal calculator), 2(difficult calculator)");
    choice = input.nextInt();
    
    switch (choice) {
      case 1:normalCal(); break;
      case 2:fourCal(); break;
    }
  }
  
/**
 * Recieves input and displays answer.
 * Pre:
 * Post: Displays answer.
 */
  
  public static void normalCal() {
    
    int fnum = 0, n;
    int snum = 0;
    int operator;
    double answer = 0.0;
    
    Scanner num = new Scanner(System.in);

    do {
    System.out.println("Enter your first number: ");
    fnum = num.nextInt();
    System.out.println("Enter your second number: ");
    snum = num.nextInt();
    System.out.println("What would you like to do with these numbers(1 = +, 2 = -, 3 = *, 4 = /)?");
    operator = num.nextInt();
    
    switch (operator) {
      case 1: answer = fnum + snum; 
        System.out.println(answer);
        break;
      case 2: answer = fnum - snum; 
        System.out.println(answer);
        break;
      case 3: answer = fnum * snum; 
        System.out.println(answer);
        break;
      case 4: answer = fnum / snum; 
        System.out.println(answer);
        break;
    }
    System.out.println(" Would you like to continue(0)?");
    n = num.nextInt();
    System.out.println();
    } while ( n == 0); 
      System.out.println("Thank you for using my calculator.");
    }

/**
 * Recieves input and displays answer.
 * Pre:
 * Post: Displays answer.
 */
  
  public static void fourCal() {
    
    int fnum = 0, n;
    int snum = 0;
    int tnum = 0;
    int fournum = 0;
    int operator;
    double answer = 0.0;
    
    Scanner num = new Scanner(System.in);

    do {
    System.out.println("Enter your first number: ");
    fnum = num.nextInt();
    System.out.println("Enter your second number: ");
    snum = num.nextInt();
    System.out.println("Enter your third number: ");
    tnum = num.nextInt();
    System.out.println("Enter your fourth number: ");
    fournum = num.nextInt();
    System.out.println("What would you like to do with these numbers(1 = +, 2 = -, 3 = *, 4 = /)?");
    operator = num.nextInt();
    
    switch (operator) {
      case 1: answer = fnum + snum + tnum + fournum; 
        System.out.println(answer);
        break;
      case 2: answer = fnum - snum - tnum - fournum; 
        System.out.println(answer);
        break;
      case 3: answer = fnum * snum * tnum * fournum; 
        System.out.println(answer);
        break;
      case 4: answer = fnum / snum / tnum / fournum; 
        System.out.println(answer);
        break;
    }
    System.out.println(" Would you like to continue(0)?");
    n = num.nextInt();
    System.out.println();
    } while ( n == 0); 
      System.out.println("Thank you for using my calculator.");
    }
    
}
