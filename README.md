# Great-internshala_IN8787_task1-calculator-
*CODE*
java
Copy code
import java.util.Scanner;

public class Calculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        double num1, num2, result;
        char operator;

        System.out.print("Enter first number: ");
        num1 = scanner.nextDouble();

        System.out.print("Enter operator (+, -, *, /): ");
        operator = scanner.next().charAt(0);

        System.out.print("Enter second number: ");
        num2 = scanner.nextDouble();

        switch (operator) {
            case '+':
                result = num1 + num2;
                break;
            case '-':
                result = num1 - num2;
                break;
            case '*':
                result = num1 * num2;
                break;
            case '/':
                if (num2 != 0)
                    result = num1 / num2;
                else {
                    System.out.println("Error: Division by zero!");
                    return;
                }
                break;
            default:
                System.out.println("Error: Invalid operator!");
                return;
        }

        System.out.println("Result: " + result);
    }
}
*Here's a detailed explanation about my project :*

Import Statements:

import java.util.Scanner;: This imports the Scanner class from the java.util package, which is used for taking user input.
Class Declaration:

public class Calculator {: This declares a class named Calculator, which will contain the main method and other components of the calculator application.
Main Method:

public static void main(String[] args) {: This is the entry point of the program. It's a special method that Java looks for when starting the program.
Variable Declarations:

Scanner scanner = new Scanner(System.in);: Creates a Scanner object named scanner to read input from the console.
double num1, num2, result;: Declares three double variables to store the numbers and result of the calculation.
char operator;: Declares a char variable to store the operator (+, -, *, /).
User Input:

System.out.print("Enter first number: ");: Prompts the user to enter the first number.
num1 = scanner.nextDouble();: Reads the first number input by the user.
System.out.print("Enter operator (+, -, *, /): ");: Prompts the user to enter the operator.
operator = scanner.next().charAt(0);: Reads the operator input by the user (only the first character).
System.out.print("Enter second number: ");: Prompts the user to enter the second number.
num2 = scanner.nextDouble();: Reads the second number input by the user.
Performing Calculation:

switch (operator) { ... }: Uses a switch statement to perform different operations based on the operator entered by the user.
Inside the switch statement, different cases handle different operators (+, -, *, /).
For each case, it performs the corresponding arithmetic operation and assigns the result to the result variable.
If the user tries to divide by zero, it displays an error message and terminates the program using return.
Output Result:

System.out.println("Result: " + result);: Prints the result of the calculation to the console.
End of Main Method:

The main method ends here.
End of Class:

The Calculator class ends here.
This code creates a simple command-line calculator that takes two numbers and an operator as input from the user, performs the calculation, and then displays the result.





