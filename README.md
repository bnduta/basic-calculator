def calculator():
    print("Welcome to the Simple Calculator! 🧮")
    
    num1 = float(input("Enter the first number: "))
    num2 = float(input("Enter the second number: "))
    
    print("\nChoose an operation: ")
    print("1) Addition (+)")
    print("2) Subtraction (-)")
    print("3) Multiplication (*)")
    print("4) Division (/)")

    operation = input("\nEnter the operation (+, -, *, /): ")

    # Perform the calculation
    if operation == "+":
        result = num1 + num2
        print(f"\nResult: {num1} + {num2} = {result}")
    elif operation == "-":
        result = num1 - num2
        print(f"\nResult: {num1} - {num2} = {result}")
    elif operation == "*":
        result = num1 * num2
        print(f"\nResult: {num1} * {num2} = {result}")
    elif operation == "/":
        if num2 != 0:
            result = num1 / num2
            print(f"\nResult: {num1} / {num2} = {result}")
        else:
            print("\nError: Division by zero is not allowed.")
    else:
        print("\nInvalid operation! Please enter +, -, *, or /.")

calculator()
