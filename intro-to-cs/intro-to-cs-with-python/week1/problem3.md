Problem 3 iterations

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

This has one failing test. When the longest letter, is one letter.

```python
# same stuff above
        if count > len(highest)-1:
            highest = s[index-1:index+count]
    else:
        count = 0
print(highest)
```

To fix, initialize with first letter. Result

```python
index = 0 
count = 0
highest = s[0:1] # added first letter
for n in range(1,len(s)):
    if(count == 0):
        index = n
    if(s[n] >= s[n-1]):
        count+=1
        if count > len(highest)-1:
            highest = s[index-1:index+count]
    else:
        count = 0
print(highest)
```
