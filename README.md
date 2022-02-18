### task A
```
A =  [int(i) for i in input().split()]
print(A[::2])
```
### task B
```
s = input()
z = []
y =s.split()
for c in y:
	if int(c) % 2 == 0:
		z.append(int(c))
print(*z)		
```
### task C
```
C =  [int(i) for i in input().split()]
temp = 0
for x in range(len(C)):
    if C[x] > 0:
        temp+=1
print(temp)
```
### task D
```
n = input()
m = n.split()
v = int(m[1])
for i in range(len(m)):
	if v < int(m[i]):
		print(int(m[i]), end=' ')
	v = int(m[i])
```
### task E
```
E =  [int(i) for i in input().split()]
resStrPos = ""
resStrNeg = ""
for x in range(len(E)):
    if E[x] < 0:
        resStrPos += str(E[x])
    else:
        resStrNeg += str(E[x])
    if len(resStrPos) > 2 | len(resStrNeg) >2:
        break
if len(resStrPos) < len(resStrNeg):
    print(resStrNeg)
else: 
    print(resStrPos)
```
### task F
```
s = [int(i) for i in input().split()]
counter = 0
for i in range(1, len(s) - 1):
    if s[i - 1] < s[i] > s[i + 1]:
        counter += 1
print(counter)
```
### task G
```
G =  [int(i) for i in input().split()]
Gmax = max(G)
GmaxIndex = G.index(Gmax)
print(f"Max ->{Gmax}\nPos ->{GmaxIndex+1}")
```
### task H
```
i=list(input().split())
min = 1000
for k in range(len(i)):
    s=int(i[k])
    if (s < min) and (s > 0):
        min=s
print(min)
```
### task I
```
I =  [int(i) for i in input().split()]
Iodd = []
for x in range(len(I)):
    if I[x] % 2 != 0:
        Iodd.append(I[x])
print(f"min odd element ->{min(Iodd)}")
```
### task G
```
G =  [int(i) for i in input().split()]
Gmax = max(G)
GmaxIndex = G.index(Gmax)
print(f"Max ->{Gmax}\nPos ->{GmaxIndex+1}")
```
### task K
```
n, count, sex = [int(i) for i in input().split()], 0, []
for c in n:
	if not(c in sex):
	    count += 1
	    sex.append(c)
print(count)	
```
### task L
```
n = [int(i) for i in input().split()]
print(*n[::-1])
```
### task M
```
M =  [int(i) for i in input().split()]
temp = 0
for x in range(len(M)//2):
    temp = M[len(M)-(x+1)]
    M[len(M)-(x+1)] = M[x]
    M[x] = temp
print(M)
```
### task N
```
n, m = [int(i) for i in input().split()], []
if len(n) % 2 == 0:
    for i in range(len(n)):
	    if i % 2 != 0:
		    m.append(n[i])
		    m.append(n[i-1])
elif len(n) % 2 != 0:
    for i in range(len(n)):
	    if i % 2 != 0:
		    m.append(n[i])
		    m.append(n[i-1])
    m.append(n[-1])		 		
print(*m)

```
### task O
```
k = 4
lst = [1,2,3,4,5]
k=k%len(lst)
ret=[0]*len(lst)
for i in range(len(lst)):
    if i+k<len(lst) and i+k>=0:
        ret[i]=lst[i+k]
    if i+k>=len(lst):
        ret[i]=lst[i+k-len(lst)]
    if i+k<0:
        ret[i]=lst[i+k+len(lst)]
print(ret)
```




