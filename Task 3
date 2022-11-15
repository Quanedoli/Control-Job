import math
class Point:
    def __init__(self,x, y):
        self.x=x
        self.y=y
    def __str__(self):
        return f"{self.x,self.y}"
    def __repr__(self):
        return f"{self.x,self.y}"
    def distance(self,other):
        x1=self.x
        y1=self.y
        x2=other.x
        y2=other.y
        dist=math.hypot(x1-x2,y1-y2)
        print (f"Distance between {self} and {other}: {dist}")
        return dist
n=int(input("Введите кол-во точек:\n"))
A=[input().split() for i in range(n)]
B=[]
for val in A:
    x = int(val[0])
    y = int(val[1])
    p=Point(x,y)
    B.append(p)
C=[]
for p1 in B:
    for p2 in B:
        if p1==p2:
            continue
        l=p1.distance(p2)
        C.append(l)
print("Min",min(C))
print("Max",max(C))

