# A Simple Calculator
# Made by Garv

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
