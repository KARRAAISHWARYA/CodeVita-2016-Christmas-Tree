# CodeVita-2016-Christmas-Tree

k = int(input())
 
for i in range(0,k):
    n = int(input())
    if(n<=1):
        print("You cannot generate christmas tree")
    elif(n>20):
        print("Tree is no more")
    elif(n>1 and n<=20):
        for p in range(1,n):
            if(p==1):
                print(" "*n,end="")
                print("*")
            for r in range(2,n+3-p):
                print(" "*(n-r+1),end="")
                print("*"*(r*2-1))
        print(" "*n,end="")
        print("*")
        print(" "*n,end="")
        print("*")
