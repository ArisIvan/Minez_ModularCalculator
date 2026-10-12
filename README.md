# Modular Calculator Mini-Program

def add_numbers(num1, num2):
    return num1 + num2

def subtract_numbers(num1, num2):
    return num1 - num2

def multiply_numbers(num1, num2):
    return num1 * num2

def divide_numbers(num1, num2):
    if num2 == 0:
        return "Cannot divide by zero."
    return num1 / num2

# A. Input
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

print("\nChoose operation:")
print("1 - Addition")
print("2 - Subtraction")
print("3 - Multiplication")
print("4 - Division")

choice = input("\nEnter choice: ")

# B. Process
if choice == '1':
    result = add_numbers(num1, num2)
elif choice == '2':
    result = subtract_numbers(num1, num2)
elif choice == '3':
    result = multiply_numbers(num1, num2)
elif choice == '4':
    result = divide_numbers(num1, num2)
else:
    result = "Invalid operation choice."

# C. Output
print("\nResult:", result)
