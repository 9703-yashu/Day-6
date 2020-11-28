#exercise 1


LIST=[1 2 3  4 5]
print(LIST)
for n in LIST:
	print("ELEMENTS AFTER ADDING +2:",n+2)


#exercise 2

ROWS=5
for i in range (0,ROWS+1):
	for j in range(ROWS-i,0,-1):
		print(j,end=' ')
print( )


#exercise 3

a=int(input("Enter the value to determine fibonacci series:"))
FE=0
S=1
if a<=0:
	print("The requested series is",FE)
else:
	print(FE,S,end=" ")
	for x in range(2,a):
		next=FE+S
		print(next,end=" ")
		FE=S
		S=next

#exercise 4

def Armstrong(n):
	n=int(input("ENETR THE NUMBER:"))
	sum=0
	temp=n
	while temp>0:
		digit=temp%10
		sum+=digit**3
		temp//=10
		if n==sum:
			print(n,"is an Armstrong number")
		else:
			print(n,"is not an Armstrong number")
print(Armstrong(n))



#exercise 5

mul=9
for i in range(1,11):
	print(mul,"x",i,"=",mul*i)


#exercise 6

V=int(input("ENTER THE VALUE:"))
if V==0:
	print("THE VALUE IS 0")
if V>0:
	print("THE VALUE IS POSITIVE")
if V<0:
	print("THE VALUE IS NEGATIVE")


#exercise 7

import math
X=math.sin(math.pi/6)
print("(sin(3.14/3)=",X)


#exercise 8

print("Enter days:")
days=int(input())
years=(days/365)
weeks=(days%365)/7
print("YEARS:",years)
print("WEEKS:",weeks)


#exercise 9

print("SIMPLE CALCULATOR")
print("Calculator")
print("1.Add")
print("2.Substract")
print("3.Multiply")
print("4.Divide")
ch=int(input("Enter Choice(1-4):"))

if ch==1:
	a=int(input("Enter A:"))
	b=int(input("Enter B:"))
	c=a+b
	print("Sum=",c)
elif ch==2:
	a=int(input("Enter A:"))
	b=int(input("Enter B:"))
	c=a-b
	print("Difference=",c)
elif ch==3:
	a=int(input("Enter A:"))
	b=int(input("Enter B:"))
	c=a*b
	print("Product=",c)
elif ch==4:
	a=int(input("Enter A:"))
	b=int(input("Enter B:"))
	c=a/b
	print("Quotient=",c)
else:
	print("Invalid Choice")
