import java.util.Scanner;

public class IntegerOperations {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Prompting for two integers
        System.out.print("Enter number 1: ");
        int firstNumber = scanner.nextInt();

        System.out.print("Enter number 2: ");
        int secondNumber = scanner.nextInt();

        // Performing various operations
        int sum = firstNumber + secondNumber;
        int difference = firstNumber - secondNumber;
        int product = firstNumber * secondNumber;
        double average = (firstNumber + secondNumber) / 2.0;
        int absoluteValue = Math.abs(difference);
        // Calculating maximum without using max function
        int maximum = (firstNumber + secondNumber + absoluteValue) / 2;
        // Calculating minimum without using min function
        int minimum = (firstNumber + secondNumber - absoluteValue) / 2;

        // Displaying the results
        System.out.println("Original numbers are " + firstNumber + " and " + secondNumber);
        System.out.println("Sum = " + sum);
        System.out.println("Difference = " + difference);
        System.out.println("Product = " + product);
        System.out.printf("Average = %.1f%n", average);
        System.out.println("Absolute value = " + absoluteValue);
        System.out.println("Maximum = " + maximum);
        System.out.println("Minimum = " + minimum);

        // Close the scanner
        scanner.close();
    }
}
