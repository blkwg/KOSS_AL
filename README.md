a = [input().split()]
a = [map(int, a)]
b = []
for i in range(a[0]):
    b.append(int(input()))
b.sort()
#2, 3, 3, 4, 6, 8, 9

def asdf(x, y):
    z = (x+y)//2
    s = 0
    for i in b:
        s += z//i
    if s > a[1]:
        if z-x == 1:
            print(b[0]*z)
        else:     
            asdf(x, z)
    elif s< a[1]:
        if y-z == 1:
            print(b[0]*z)
        else:
            asdf(z, y)
    else:
        print(b[0]*z)
    
asdf(b[0], b[-1])
    
