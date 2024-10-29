# Hacktoberfest2024_avi_1
Make your first PR. A beginner friendly repository made specifically for open source beginners. Add any program under any language (it can be anything from a simple program to a complex data structure algorithm). Happy coding...
import java.util.Scanner;

public class ReverseNumber {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Enter an integer: ");
        int number = scanner.nextInt();
        
        int reversedNumber = 0;
        int originalNumber = number;
        
        while (number != 0) {
            int digit = number % 10; // Get the last digit
            reversedNumber = reversedNumber * 10 + digit; // Build the reversed number
            number /= 10; // Remove the last digit from the original number
        }
        
        System.out.println("The reverse of " + originalNumber + " is " + reversedNumber);
        
        scanner.close();
    }
}

