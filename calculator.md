def add(a,b):
    return a + b

def subtract(a,b):
    return a - b

def multiply(a,b):
    return a * b

def divide(a,b):
    if b != 0:
        return a/b
    else:
        return "cannot divide by zero"
    
print("select operation")
print("1.add")
print("2.subtract")
print("3.multiply")
print("4.divide")

choice = input("Enter choice(1/2/3/4): ")

num1 = float(input("Enter first number:"))
num2 = float(input("Enter second number:"))

if choice == '1':
    print(num1,"+",num2,"=",add(num1,num2))
elif choice == '2':
    print(num1,"-",num2,"=",subtract(num1,num2))
elif choice == '3':
    print(num1,"*",num2,"=",multiply(num1,num2))
elif choice == '4':
    print(num1,"/",num2,"=",divide(num1,num2))
else:
    print("Invalid input")    
