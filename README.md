# chethan
create programme
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b

def divide(a, b):
    if b != 0:
        return a / b
    else:
        return "Error! Division by zero."

def calculator():
    print("")
    print("hii");
    print("Select an operation:")
    print("1. Addition (+)")
    print("2. Subtraction (-)")
    print("3. Multiplication (*)")
    print("4. Division (/)")
    print("5. Exit")

    while True:
        choice = input("\nEnter your choice (1/2/3/4/5): ")

        if choice in ['1', '2', '3', '4']:
            num1 = float(input("Enter the first number: "))
            num2 = float(input("Enter the second number: "))

            if choice == '1':
                print(f"The result of {num1} + {num2} is {add(num1, num2)}")
            elif choice == '2':
                print(f"The result of {num1} - {num2} is {subtract(num1, num2)}")
            elif choice == '3':
                print(f"The result of {num1} * {num2} is {multiply(num1, num2)}")
            elif choice == '4':
                print(f"The result of {num1} / {num2} is {divide(num1, num2)}")
        elif choice == '5':
            print("Exiting the calculator. Goodbye!")
            break
        else:
            print("Invalid input. Please enter a number between 1 and 5.")

