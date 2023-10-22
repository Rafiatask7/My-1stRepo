# My-1stRepo
This repository contains a Python script that calculates the factorial of a number using a recursive function. Factorial of a non-negative integer 'n' is the product of all positive integers less than or equal to 'n.'

def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n - 1)

if __name__ == "__main__":
    try:
        num = int(input("Enter a non-negative integer: "))
        if num < 0:
            print("Please enter a non-negative integer.")
        else:
            result = factorial(num)
            print(f"The factorial of {num} is {result}")
    except ValueError:
        print("Invalid input. Please enter a non-negative integer.")

