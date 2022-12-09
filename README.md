import random 
while True:
    a=int(input("Enter Upper limit:"))
    b=int(input("Enter Lower limit:"))
    
    list=[]
    for i in range(a,b):
    
        list.append(i)
    print(list)
    c=random.choice(list)
    print("Randomly picked number is ",c)
    if c%2==0:
        print("The number is even")
    if c%2!=0:
        print("The number is odd")
    if c<0:
        print("The number is negative")
    if c>0:
        print("The number is positive")
    def prime(c):
        for j in range(2, c):
            if (c% j) == 0:
                return False
        return True
        
    if (c==1):
        print("1 is neither a prime number nor composite number")
    elif (prime(c)):
        print("the number is prime")
    else:
        print("the number is composite")
        break
