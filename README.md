# SquareRoot_Python
How to find the square root of a number using Python

# SQUARE ROOT FINDER BY PHILIP FURNESS

print ('Hello, give me a number.' )


def contains_number(s):
    return next((True for char in s if char.isdigit()), False)

while True:
    myNumber = input('Response : ')
    is_digit = contains_number(myNumber)


    if is_digit == True:
        myNumber = float(myNumber)
        break
    if is_digit == False:
        print (f'{myNumber} is not a number! ')

print ('Thanks')

x: int = 0
y: float = 0

while True:

    if x * x == myNumber:
        print (f'{x}, is the square root of {myNumber}')
        break
    if x * x > myNumber:
        y = x -1
        while True:
            if y * y == myNumber:
                print(f'{y}, is the square root of {myNumber}')
            if y * y > myNumber:
                print (f'{y} is very close to the quare root of {myNumber}')
                break
            y = y + 0.0001
    if x * x > myNumber:
        break
    x = x + 1

print('The end')
