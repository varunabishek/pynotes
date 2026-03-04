---
title: Looping
date: 2026-03-04
author: Your Name
cell_count: 8
score: 5
---

```python
print("hello world")
```

    hello world
    


```python
##Multiplication Table using For loop 

n = int(input("enter the number: "))

for i in range(1,11):
    print(n,"X",i,"==",n*i)
    i+=1



```


```python
##factorial

num = int(input("enter number: "))
factorial=1
for i in range(1, num+1):
    factorial = factorial*i
print(factorial)
```


```python
##

num=0
for i in range(1,101):
    num = num + i
    i=+1
print(num)
```


```python
   ## linear search in list - 3.3.26
arr = [2,4,5,6,8,9,10,15]
guess = int(input("enter number to be found: "))
for i in arr:
    if(guess == i):
        print("the element thats to be found is  found at position",i)
        break
else:
    print("the element is not present here") 
```


```python
##vowel counter
userinput = str(input("enter string: "))
count= 0
for char in str(userinput):
    if char in ("a","e","i","o","u"):
        count +=1
print("number of vowels in the string you entered is:",count)


                
```


```python
##multiplication tables using while loop



n = int(input("enter number: "))
i=1

while i<11:
    print(n,"x",i,"==",n*i)
    i = i+1
    

```


```python
##greatest number from a user inputted array
n=int(input("enter number of elements: "))
lista = []
for i in range(n):
    element = int(input("enter elements: "))
    lista.append(element)

largest = lista[0]
for num in lista:
    if num > largest:
        largest = num
print("array: ",lista)
print("largest number is: ",largest)


    
```


---
**Score: 5**