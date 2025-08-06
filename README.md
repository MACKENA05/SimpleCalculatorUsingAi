# Simple Java Calculator 🧮

A beginner-friendly command-line calculator built with Java that performs basic arithmetic operations.

## 📋 Table of Contents
- [About the Project](#about-the-project)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [How to Run](#how-to-run)
- [Usage Examples](#usage-examples)
- [Troubleshooting](#troubleshooting)
- [What I Learned](#what-i-learned)
- [Future Improvements](#future-improvements)

## 🎯 About the Project

This project was created as part of Moringa School's  capstone project. The goal was to use AI prompts to learn Java programming and create a functional application that demonstrates core programming concepts.

**Technologies Used:**
- Java (JDK 11+)
- Command Line Interface
- AI-assisted development 

## ✨ Features

- ➕ Addition
- ➖ Subtraction  
- ✖️ Multiplication
- ➗ Division (with zero-division protection)
- 🛡️ Basic error handling
- 👥 User-friendly interface with clear prompts

## 📦 Prerequisites

Before running this project, make sure you have:

- **Java Development Kit (JDK) 11 or higher** installed
- **Command line/Terminal** access
- **Text editor** (optional, for viewing code)

### Check if Java is installed:
```bash
java --version
javac --version
```

If Java is not installed, download it from:
- [Oracle JDK](https://www.oracle.com/java/technologies/downloads/)
- [OpenJDK](https://openjdk.org/)

## 🚀 Installation

1. **Clone or download this project:**
   ```bash
   git clone <your-repo-url>
   cd SimpleCalculator
   ```

2. **Or create the files manually:**
   - Create a folder called `SimpleCalculator`
   - Create a file called `Calculator.java`
   - Copy the code from the project files

## ▶️ How to Run

### Step 1: Compile the Java file
```bash
javac Calculator.java
```

### Step 2: Run the program
```bash
java Calculator
```

### Alternative: One-line compile and run
```bash
javac Calculator.java && java Calculator
```

## 🎮 Usage Examples

### Example 1: Addition
```
🧮 Simple Java Calculator
========================
Enter first number: 15
Enter operation (+, -, *, /): +
Enter second number: 25
✅ Result: 15.0 + 25.0 = 40.0
```

### Example 2: Division
```
🧮 Simple Java Calculator
========================
Enter first number: 100
Enter operation (+, -, *, /): /
Enter second number: 4
✅ Result: 100.0 / 4.0 = 25.0
```

### Example 3: Division by Zero (Error Handling)
```
🧮 Simple Java Calculator
========================
Enter first number: 10
Enter operation (+, -, *, /): /
Enter second number: 0
❌ Error: Cannot divide by zero!
```

### Example 4: Invalid Operation
```
🧮 Simple Java Calculator
========================
Enter first number: 5
Enter operation (+, -, *, /): %
Enter second number: 3
❌ Error: Invalid operation!
```

## 🔧 Troubleshooting

### Common Issues and Solutions:

#### 1. "javac is not recognized" or "command not found"
**Problem:** Java is not installed or not in PATH
**Solution:** 
- Install JDK from Oracle or OpenJDK
- Add Java to your system PATH
- Restart your terminal

#### 2. "Could not find or load main class Calculator"
**Problem:** Wrong directory or compilation failed
**Solution:**
- Make sure you're in the same directory as `Calculator.java`
- Compile first: `javac Calculator.java`
- Check that `Calculator.class` file was created

#### 3. Program crashes with InputMismatchException
**Problem:** Entered text instead of numbers
**Solution:**
- Only enter numbers when prompted
- Use decimal point (.) not comma (,) for decimals
- Restart the program if it crashes

#### 4. Weird decimal results (like 0.333333333)
**Problem:** This is normal Java behavior
**Solution:** This is expected! Java shows many decimal places for precision

## 🧠 What I Learned

Through this AI-assisted project, I learned:

### Java Concepts:
- **Variables and Data Types**: `double`, `char`, `boolean`
- **User Input**: Using `Scanner` class
- **Control Structures**: `switch` statements and `if-else`
- **Error Handling**: Basic validation and error messages
- **Methods**: Understanding `main()` method

### AI-Assisted Development:
- How to write effective prompts for coding help
- Iterating on AI suggestions to improve code
- Using AI to debug and explain error messages
- Documenting the AI learning process

### Development Process:
- Compiling and running Java programs
- Basic debugging techniques
- Writing user-friendly console applications

## 🚀 Future Improvements

Ideas for extending this project:

### Easy Extensions:
- [ ] Add more operations (square root, power, modulus)
- [ ] Allow multiple calculations without restarting
- [ ] Format decimal output to 2 places
- [ ] Add calculation history

### Medium Extensions:
- [ ] Create a simple GUI using JavaFX
- [ ] Add scientific calculator functions
- [ ] Save calculation history to a file
- [ ] Add unit tests

### Advanced Extensions:
- [ ] Build a web version using Spring Boot
- [ ] Add expression parsing (e.g., "2+3*4")
- [ ] Create a mobile app version
- [ ] Add graphing capabilities

## 📁 Project Structure
```
SimpleCalculator/
├── Calculator.java          # Main calculator program
├── README.md               # This file
├── toolkit.md             # Development toolkit for prompts and resources
└── Calculator.class        # Compiled Java file (created after compilation)
```

## 🤝 Contributing

This is a learning project, but suggestions are welcome! If you find bugs or have ideas for improvements:

1. Fork the project
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📜 License

This project is for educational purposes as part of Moringa School's curriculum.

## 🙏 Acknowledgments

- **Moringa School** for the capstone project framework
- **AI Platform** for coding assistance and learning support
- **Java Community** for excellent documentation and resources

---

**Created by:** [Monicah Mackena]  
**Date:** August 2024  
**Course:** Moringa School - Prompt-Powered Kickstart Capstone  

*This project demonstrates Java fundamentals through AI-assisted learning and iterative development.*