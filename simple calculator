import random


def random_calculator():

    random_or_not = input("would you like to use random numbers? (y/n)")

    if random_or_not == 'y':
        num1 = random.randint(0, 10)
        num2 = random.randint(0, 10)
    else:
        num1 = input("enter the first number")
        num2 = input("enter the second number")

    op = input("enter an operator (+/-/*/:"
               ")")
    if op == '+':
        print("the result of", num1, '+', num2, " is: ", int(num1) + int(num2))
    elif op == '-':
        print("the result of", num1, '-', num2, " is: ", int(num1) - int(num2))
    elif op == '*':
        print("the result of", num1, '*', num2, " is: ", int(num1) * int(num2))
    elif op == ':':
        print("the result of", num1, ':', num2, " is: ", int(num1) / int(num2))
    else:
        print("unsupported operator")


random_calculator()
answer = input("would you like to run the calculator again? (y/n)")

while answer != 'n':
    random_calculator()
    answer = input("run again? (y/n)")
