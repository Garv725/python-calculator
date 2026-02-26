# A PYTHON CALCULATER

## 📌 Overview : 
This is a beginner-level Python calculator project that performs basic arithmetic operations such as addition, subtraction, multiplication, and division. The program includes proper error handling to ensure smooth execution.

## 🚀 Features : 
- Addition (+)
- Subtraction (-)
- Multiplication (*)
- Division (/)
- Division by zero handling
- Invalid input handling

## 🛠️ Technologies Used : 
Python 3

## ▶️ How to Run : 
1. Download the calculator.py file.
2. Open terminal or command prompt.
3. Run the file using:
python calculator.py

## 📚 Learning Purpose : 
This project was created to practice:
- Conditional statements
- User input handling
- Exception handling
- Basic program structure in Python


## 👤 Author : 
**Garv (GitHub: Garv725)**

```python
print("=" * 30)
print(" SIMPLE CALCULATOR")
print("=" * 30)
print("Operations available:")
print("+ Addition")
print("- Subtraction")
print("* Multiplication")
print("/ Division")
print("=" * 30)

try:
    num1 = float(input("Enter first number: "))
    op = input("Enter operator (+, -, *, /): ")
    num2 = float(input("Enter second number: "))

    if op == '+':
        result = num1 + num2
    elif op == '-':
        result = num1 - num2
    elif op == '*':
        result = num1 * num2
    elif op == '/':
        if num2 == 0:
            print("Error: Division by zero is not allowed!")
            exit()
        result = num1 / num2
    else:
        print("Invalid operator! Please use +, -, * or /")
        exit()

    print("Result:", result)

except ValueError:
    print("Error: Please enter valid numbers only!")
