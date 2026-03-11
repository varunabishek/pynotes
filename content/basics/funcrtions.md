---
title: Funcrtions
date: 2026-03-11
author: Your Name
cell_count: 14
score: 10
---

```python
def vowels_present(strx):
    count=0
    for char in strx:
        if char in ("a","e","i","o","u"):
            count = count + 1
    print(count)
    return(strx)

stry = str(input("Enter str: "))
result = vowels_present(stry)
print("the numbers of vowels present is: ",result) 





```


```python
#problems on args:

def sum_all(*numbers):
    return sum(numbers)
print(sum_all(1,2,4,5,6,8))
print(sum_all(9,4,5,6))

    
```

    26
    24
    


```python
#problems on args

def greet_all(*strs):
    for x in strs:
        print("Hello",x)
greet_all("varun","arun","poland")
```

    Hello varun
    Hello arun
    Hello poland
    


```python
def reverse_list(user_list):
    return list(reversed(user_list))

arr1 = []
n = int(input("enter num of elements: "))
for i in range(n):
    ele=input("enter elements: ")
    arr1.append(ele)
result = reverse_list(arr1)
print("reversed list is: ", result)

```


```python
def dc(**details):
    for key, values in details.items():
        print(f"{key}:{values}")
dc(name = "varun", age = 35, city = "omlette")
```

    name:varun
    age:35
    city:omlette
    


```python
#using args to filter even numbers and put in array
def filter_even(*numbers):
    evens = []
    for x in numbers:
        if x % 2 == 0:
            evens.append(x)
    return evens
result=filter_even(1,2,4,7,65,43,32,90,98)
print(result)
        
```

    [2, 4, 32, 90, 98]
    


```python
def  sum_list(numbers):
    total=0
    for num in numbers:
        total = total + num
    return (total)
my_list = [1,99,56,34,90]
result =  sum_list(my_list)
print("sum of list is", result)
```

    sum of list is 280
    


```python
def add(x,y):
    return x + y
result = add(5,4)
print(result)
```

    9
    


```python
def add(x,y):
    return x + y
x=int(input("enter x: "))
y=int(input("enter y: "))
result=add(x,y)
print("sum of x and y is",result)
```

    enter x:  90
    enter y:  98
    

    sum of x and y is 188
    


```python
#sum of n numbers using recursion:

def sum_n(x):
    if x == 0:
        return 1
    else:
        return x + sum_n(x-1)
print(sum_n(5))
```

    16
    


```python
#factorial by using recursion:

def factorial(x):
    if x == 0:
        return 1
    else:
        return x*factorial(x-1)
print(factorial(7))
```

    5040
    


```python
#fibbonacci numbers using recursion:

def fibonnaci(x):
    if x <=1:
        return x
    else:
        return fibonnaci(x-1)+fibonnaci(x-2)
print(fibonnaci(8))
```

    21
    


```python
#factorial using iteration:

def factorial(x):
    ans=1
    if x == 0:
        return x
    else:
        for i in range(1,x+1):
            ans *= i
        return ans
print(factorial(5))
```

    120
    


```python

```


---
**Score: 10**