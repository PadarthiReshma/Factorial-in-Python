# Factorial-in-Python

# Apporach-1
# Python 3 program to find factorial of given number
def factorial(n):
	if n < 0:
		return 0
	elif n == 0 or n == 1:
		return 1
	else:
		fact = 1
		while(n > 1):
			fact *= n
			n -= 1
		return fact

# Driver Code
num = 5
print("Factorial of",num,"is",
factorial(num))


# Apporach-2
# Python 3 program to find
# factorial of given number

# Function to find factorial of given number
def factorial(n):	
	res = 1
	for i in range(2, n+1):
		res *= i
	return res
# Driver Code
num = 5
print("Factorial of", num, "is",
factorial(num))

# Apporach-3

# Python program to find the factorial of a number provided by the user.
# change the value for a different result
num = 7
# To take input from the user
#num = int(input("Enter a number: "))
factorial = 1
# check if the number is negative, positive or zero
if num < 0:
   print("Sorry, factorial does not exist for negative numbers")
elif num == 0:
   print("The factorial of 0 is 1")
else:
   for i in range(1,num + 1):
       factorial = factorial*i
   print("The factorial of",num,"is",factorial)

# Apporach-4
# Using Recursion Method
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n-1)

print("Factorial of 7 =", factorial(7))
