x=int(input("x:"))
y=int(input("y:"))


for i in range(1,20):
    if i==10:
        print("- "*10+"+"+" -"*10)
    else:
        print("  "*10+"'")
    # to track coordinate and print srounding
    if i!=10 and y<10:
        if x>0 and i==10-y:
            print("  "*(9+x)," #(",x,",",y,")")
        if x<0 and i==10-y:
            print("  "*(10-(-1*x))," #(",x,",",y,")")
        
    if i!=10 and y>10:
        if x>0 and i==10-(-1*y):
            print("  "*(9+x)," #(",x,",",y,")")
        if x<0 and i==10-y:
            print("  "*(10-(-1*x))," #(",x,",",y,")"
