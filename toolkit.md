# Simple Calculator Project Using Java

## Title & Objective

**Technology**: Java Programming Language

**Project Title**: Simple Calculator

**Why I chose Java**: Java is widely used in enterprise applications and Android development. It's beginner-friendly with strong typing and clear syntax.

**End Goal**: Create a simple command-line calculator that can perform basic math operations (add, subtract, multiply, divide).

## Quick Summary of the Technology

**What is Java?**
Java is a popular programming language that runs on any device with the Java Virtual Machine (JVM). It's known for "write once, run anywhere."

**Where is it used?**
- Android apps
- Web applications
- Desktop software
- Enterprise systems

**Real-world example**: Minecraft was originally written in Java.

## System Requirements

**Operating System**: Windows, macOS, or Linux

**Tools Required**:

- Java Development Kit (JDK) 11 or higher
- Text editor or simple IDE
- Terminal/Command Prompt


# Java Calculator Tutorial

## 4. Installation & Setup Instructions

### Step 1: Install Java
- **Download JDK**: Go to [Oracle JDK](https://www.oracle.com/java/technologies/downloads/) or use [OpenJDK](https://openjdk.org/)
- **Verify Installation**:
```bash
java --version
javac --version
```

### Step 2: Create Project Folder
```bash
mkdir SimpleCalculator
cd SimpleCalculator
```

## 5. Minimal Working Example

### What the Example Does
A simple calculator that:
- Takes two numbers from user
- Asks for operation (+, -, *, /)
- Shows the result
- Handles basic errors

### Code (Calculator.java)
```java
import java.util.Scanner;

public class Calculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.println("🧮 Simple Java Calculator");
        System.out.println("========================");
        
        // Get first number
        System.out.print("Enter first number: ");
        double num1 = scanner.nextDouble();
        
        // Get operation
        System.out.print("Enter operation (+, -, *, /): ");
        char operation = scanner.next().charAt(0);
        
        // Get second number
        System.out.print("Enter second number: ");
        double num2 = scanner.nextDouble();
        
        // Calculate result
        double result = 0;
        boolean validOperation = true;
        
        switch (operation) {
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
                if (num2 != 0) {
                    result = num1 / num2;
                } else {
                    System.out.println("❌ Error: Cannot divide by zero!");
                    validOperation = false;
                }
                break;
            default:
                System.out.println("❌ Error: Invalid operation!");
                validOperation = false;
        }
        
        // Show result
        if (validOperation) {
            System.out.println("✅ Result: " + num1 + " " + operation + " " + num2 + " = " + result);
        }
        
        scanner.close();
    }
}
```

### How to Run
```bash
# Compile the Java file
javac Calculator.java

# Run the program
java Calculator
```
#### Alternative: One-line compile and run
```bash
javac Calculator.java && java Calculator
```

### Expected Output
```
🧮 Simple Java Calculator
========================
Enter first number: 10
Enter operation (+, -, *, /): +
Enter second number: 5
✅ Result: 10.0 + 5.0 = 15.0
```

## 6. AI Prompt Journal (Using ai.moringaschool.com)

### Prompt 1: Basic Structure
**Prompt Used**: "Create a simple calculator program using Java that takes two numbers and performs basic operations. Include proper variable naming and comments."

**AI Response Summary**: The AI provided a clean structure with Scanner for input, switch statement for operations, and basic error handling. It also suggested using descriptive variable names and adding user-friendly output messages.

**Evaluation**: Very helpful - gave me the exact structure I needed with clear explanations. The AI understood the context well.

### Prompt 2: Error Handling
**Prompt Used**: "How do I handle division by zero and invalid operations in Java? Show me best practices for input validation."

**AI Response Summary**: AI suggested using if-else conditions for division by zero, a default case in switch for invalid operations, and mentioned try-catch blocks for more advanced error handling.

**Evaluation**: Perfect for making the program more robust and user-friendly. The AI provided both simple and advanced solutions.

### Prompt 3: Code Improvement
**Prompt Used**: "Review my Java calculator code and suggest improvements for readability and functionality. What Java best practices should I follow?"

**AI Response Summary**: The AI recommended:
- Adding comments for clarity
- Using meaningful variable names
- Consistent formatting and indentation
- Proper resource management (closing Scanner)
- Adding user-friendly output with emojis

**Evaluation**: Excellent feedback that helped improve code quality and user experience.

### Prompt 4: Learning Reflection
**Prompt Used**: "What key Java concepts does this calculator project demonstrate? How can I extend it to learn more advanced concepts?"

**AI Response Summary**: The AI identified key concepts (variables, data types, input/output, control structures, methods) and suggested extensions like:
- Adding a loop for multiple calculations
- Creating separate methods for each operation
- Adding more mathematical functions
- Implementing a simple GUI

**Evaluation**: Great for understanding the learning objectives and planning next steps.

## 7. Common Issues & Fixes

### Issue 1: "javac not recognized"
**Problem**: Command not found when trying to compile.
**Solution**: Make sure Java is installed and added to PATH environment variable.

### Issue 2: InputMismatchException
**Problem**: Program crashes when user enters text instead of numbers.
**Solution**: For now, just restart the program. Advanced: Add try-catch blocks.

### Issue 3: Wrong decimal results
**Problem**: Division results look weird (like 0.33333333).
**Solution**: This is normal! Java shows many decimal places.

## 8. References

### Official Documentation
- [Java Documentation](https://docs.oracle.com/en/java/)

### Learning Resources
- [W3Schools Java Tutorial](https://www.w3schools.com/java/)
- [Java Tutorial for Beginners](https://www.oracle.com/java/technologies/javase/codeconventions-introduction.html)

### Tools
- VS Code with Java Extension Pack