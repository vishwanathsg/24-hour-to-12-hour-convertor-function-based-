# 24-hour-to-12-hour-convertor-function-based-
This code converts 24 hour time into 12 hour time format

#Function_Conversion: Input some numbers, do some simple arithmetic to do silly conversions
#Filip has a problem of not understanding 24 hour time format.
#So I have made a program that converts time in 24 hour time format into 12 hour time format.
#24 hour time looks like : 1300/ 13:00, 2244/ 22:44
#NOTE : Enter value in both units & tens while entering hour values

def twel(X):
    Z=X-12
    return Z
"""
Input: X, a positive integer
Returns True if X is a positive integer, otherwise False
"""

X=int(input("Enter Hour: "))
#Took input in 24 hour format

Y=int(input("Enter minutes: "))
#Noted minutes

result=twel(X)

if X < 12:
    print("The time in 12 hour format is {}:{} AM".format(X,Y))

elif X == 12:
    print ("The time in 12 hour format is {}:{} PM".format(X,Y))

elif X > 12 :
    print("The time in 12 hour format is {}:{} PM".format(result,Y))
