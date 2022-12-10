def prime(x):
    c=1
    for i in range(2,x):
        if x%i==0:
            c=0
            break
    return c
#main
a=int(input("enter the starting range:"))
b=int(input("enter the ending range:"))
for i in range(a,b+1):
    if i<=0:
        print("please enter positive number greater then 0")
    elif i==1:
        print("1 is neither prime nor composite its a special number")
    else:
        t=prime(i)
        if t==0:
            print(i,"is a composite number")
        elif t==1:
            print(i,"is a prime number")

