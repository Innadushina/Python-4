Задача 22
mol = [int(x) for x in input().split()]
n = mol[0]
m = mol[1]
set_1 = set()
set_2 = set()
list_1 = list()
a = [int(x) for x in input().split()]
k = set(a)
for i in k:
set_1.add(i)
b = [int(x) for x in input().split()]
k1 = set(b)
for i in k1:
set_2.add(i)
lok = set_1 & set_2
kool = list(lok)
kool.sort()
for i in kool:
print(i, end=' ')

Задача 24
n = int( input( 'n = ' ) )
lis = [ int(x) for x in input( '-> ' ).split() ]
n = len(lis)
lis = lis + lis[:2]
ma = 0
for i in range(n):
    ma = max( ma, lis[i] + lis[i+1] + lis[i+2] )
print(ma)
