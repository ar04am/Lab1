# Lab1
def calculator():
    print("Simple Calculator")
    print("Available operations: + , - , * , /")
    
    try:
        num1 = float(input("Enter the first number: "))
        operator = input("Enter the operation (+, -, *, /): ")
        num2 = float(input("Enter the second number: "))

        if operator == '+':
            result = num1 + num2
        elif operator == '-':
            result = num1 - num2
        elif operator == '*':
            result = num1 * num2
        elif operator == '/':
            if num2 == 0:
                print("Error: Division by zero is not allowed.")
                return
            result = num1 / num2
        else:
            print("Invalid operation!")
            return
        
        print(f"Result: {result}")

    except ValueError:
        print("Error: Please enter valid numbers.")

calculator()
