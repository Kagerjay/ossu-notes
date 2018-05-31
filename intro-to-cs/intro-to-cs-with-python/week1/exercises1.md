## Problem 1

Count vowels in string

```python
s = 'azcbobobegghakl'
count = 0

for i in s:
    if(i == "a" or i=="e" or i=="i" or i=="o" or i=="u"):
        count += 1

print("Number of vowels: " + str(count)) # Number of vowels 5
```

## Problem 2

Counting number of times 'bob' occurs in string
The solution is to take the index's current value + 3, and check if it is equal to bob.

```python
s = 'azcbobobegghakl'
count = 0;
for n in range(len(s)):
    if(s[n:n+3] == 'bob'):
        count+=1
print('Number of times bob occurs is ' + str(count)) # 2
```

## Problem 3

Now half working solution. Half test cases don't work. s = 'ywbjcgojcsshqotxlv' expects `cgo`, not `bj`
```python
index = 0
count = 0
highest = ''
for n in range(1,len(s)):
    if(count == 0):
        index = n
    if(s[n] >= s[n-1]):
        count+=1
    else:
        if count > len(highest):
            highest = s[index-1:index+count]
        count = 0
print(highest)
```