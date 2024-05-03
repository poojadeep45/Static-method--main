package Pack1; // Package declaration

public class CalculatorDemo { // Class to demonstrate Calculator and Mathutils usage

    // Main method, the entry point for executing the program
    public static void main(String[] args) throws Exception {
        // Create an instance of the Calculator class
        Calculator cal = new Calculator(); 
        
        // Perform basic arithmetic operations using the Calculator instance
        double sum = cal.add(3, 8);        // Add 3 and 8
        double sub = cal.sub(9, 5);        // Subtract 5 from 9
        double product = cal.multiply(4, 3); // Multiply 4 and 3
        double quotient = cal.divide(9, 3);  // Divide 9 by 3
        
        // Display the results of the arithmetic operations
        System.out.println("Sum: " + sum);             // Outputs: 11
        System.out.println("Subtraction: " + sub);     // Outputs: 4
        System.out.println("Product: " + product);     // Outputs: 12
        System.out.println("Quotient: " + quotient);   // Outputs: 3
        
        // Demonstrate the use of Mathutils for additional mathematical operations
        int number = 7; // Test number for factorial and prime check
        long fact = Mathutils.factorial(number); // Calculate the factorial of 7
        boolean isPrime = Mathutils.isPrime(number); // Check if 7 is prime
        
        // Display the results of the mathematical operations
        System.out.println("The factorial of " + number + " is " + fact); // Outputs: The factorial of 7 is 5040
        System.out.println(number + " is prime: " + isPrime);             // Outputs: 7 is prime: true
    }
}
