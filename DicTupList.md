
Tupples


```python
# tupples are immutable while Lists are mutable
```


```python
myTupple = (1,2,3,4,5,6,7)
```


```python
myTupple
```




    (1, 2, 3, 4, 5, 6, 7)




```python
myTupple[:4]
```




    (1, 2, 3, 4)




```python
del myTupple[3]
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-6-5c7827e9113c> in <module>
    ----> 1 del myTupple[3]
    

    TypeError: 'tuple' object doesn't support item deletion



```python
myTupple[4]="update"
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-7-f4ebabe2282f> in <module>
    ----> 1 myTupple[4]="update"
    

    TypeError: 'tuple' object does not support item assignment



```python
#Packing
cities = ("khi","lhr", "multan")

```


```python
#Unpacking
largest, bigger, small = cities
```


    ---------------------------------------------------------------------------

    ValueError                                Traceback (most recent call last)

    <ipython-input-15-e5ea000acbaf> in <module>
          1 #Unpacking
    ----> 2 largest, bigger, small,assa = cities
    

    ValueError: not enough values to unpack (expected 4, got 3)



```python
largest
```




    'khi'




```python
bigger
```




    'lhr'




```python
small
```




    'multan'




```python
largest = "asadsd"
```


```python
alist = [34,45,67]
```


```python
a,b,c = alist
```


```python
print(a,b,c)
```

    34 45 67
    

For Loops


```python
#Task
#to print your name ten times 
```


```python
print("nasir")
print("nasir")
print("nasir")
print("nasir")
print("nasir")
print("nasir")
print("nasir")
print("nasir")
print("nasir")
print("nasir")
print("nasir")
print("nasir")
```

    nasir
    nasir
    nasir
    nasir
    nasir
    nasir
    nasir
    nasir
    nasir
    nasir
    nasir
    nasir
    


```python
for a in range(10):
    print(a, "nasir")
```

    0 nasir
    1 nasir
    2 nasir
    3 nasir
    4 nasir
    5 nasir
    6 nasir
    7 nasir
    8 nasir
    9 nasir
    


```python
for a in range(5,10):
    print(a, "nasir")
```

    5 nasir
    6 nasir
    7 nasir
    8 nasir
    9 nasir
    


```python
for a in range(0,10,2):#(start,end-1,step)
    print(a, "nasir")
```

    0 nasir
    2 nasir
    4 nasir
    6 nasir
    8 nasir
    


```python
for a in range(1,10,2):#(start,end-1,step)
    print(a, "nasir")
```

    1 nasir
    3 nasir
    5 nasir
    7 nasir
    9 nasir
    


```python
for a in range(10,0,-1):#(start,end-1,step)
    print(a, "nasir")
```

    10 nasir
    9 nasir
    8 nasir
    7 nasir
    6 nasir
    5 nasir
    4 nasir
    3 nasir
    2 nasir
    1 nasir
    


```python
for name in ["khi","lhr", "multan"]:
    print(name)
```

    khi
    lhr
    multan
    


```python
for character in ["String"]:
    print(character)
```

    String
    


```python
# Pass , Break and Continue
```


```python
for a in range (10):
    if a==5:
        break
    print(a)
```

    0
    1
    2
    3
    4
    


```python
friends= ["a",'b','c','d','e','f','g']

for friend in friends:
    if friend!= "e":
        print("continue and enjoy party")
        
    else:
        print("party is over")
        break
```

    continue and enjoy party
    continue and enjoy party
    continue and enjoy party
    continue and enjoy party
    party is over
    


```python
for a in range (10):
    if a==5:
        continue
    print(a)
```

    0
    1
    2
    3
    4
    6
    7
    8
    9
    


```python
for a in range (10):
    pass

```


```python
tableNo = int(input("Enter the table number"))
for num in range(1,11):
    print(f"{tableNo} * {num} = {tableNo*num}")
```

    Enter the table number 5
    

    5 * 1 = 5
    5 * 2 = 10
    5 * 3 = 15
    5 * 4 = 20
    5 * 5 = 25
    5 * 6 = 30
    5 * 7 = 35
    5 * 8 = 40
    5 * 9 = 45
    5 * 10 = 50
    


```python
for tables in range(2,10, 2):
    print("=========")
    for num in range(1,11):
        print(f"{tables} * {num} = {tables*num}")
```

    =========
    2 * 1 = 2
    2 * 2 = 4
    2 * 3 = 6
    2 * 4 = 8
    2 * 5 = 10
    2 * 6 = 12
    2 * 7 = 14
    2 * 8 = 16
    2 * 9 = 18
    2 * 10 = 20
    =========
    4 * 1 = 4
    4 * 2 = 8
    4 * 3 = 12
    4 * 4 = 16
    4 * 5 = 20
    4 * 6 = 24
    4 * 7 = 28
    4 * 8 = 32
    4 * 9 = 36
    4 * 10 = 40
    =========
    6 * 1 = 6
    6 * 2 = 12
    6 * 3 = 18
    6 * 4 = 24
    6 * 5 = 30
    6 * 6 = 36
    6 * 7 = 42
    6 * 8 = 48
    6 * 9 = 54
    6 * 10 = 60
    =========
    8 * 1 = 8
    8 * 2 = 16
    8 * 3 = 24
    8 * 4 = 32
    8 * 5 = 40
    8 * 6 = 48
    8 * 7 = 56
    8 * 8 = 64
    8 * 9 = 72
    8 * 10 = 80
    


```python
first_names = ["BlueRay ", "Upchuck ", "Lojack ",
"Gizmo ", "Do-Rag "]
last_names = ["Zzz", "Burp", "Dogbone", "Droop"]
full_names = []
for a_first_name in first_names:
    for a_last_name in last_names:
        full_names.append(a_first_name + " " +a_last_name)
full_names
```




    ['BlueRay  Zzz',
     'BlueRay  Burp',
     'BlueRay  Dogbone',
     'BlueRay  Droop',
     'Upchuck  Zzz',
     'Upchuck  Burp',
     'Upchuck  Dogbone',
     'Upchuck  Droop',
     'Lojack  Zzz',
     'Lojack  Burp',
     'Lojack  Dogbone',
     'Lojack  Droop',
     'Gizmo  Zzz',
     'Gizmo  Burp',
     'Gizmo  Dogbone',
     'Gizmo  Droop',
     'Do-Rag  Zzz',
     'Do-Rag  Burp',
     'Do-Rag  Dogbone',
     'Do-Rag  Droop']




```python
"pakistan".upper()
```




    'PAKISTAN'




```python
"PAKISTAN".lower()
```




    'pakistan'



#Dictionary works on key value pair


```python
myDic = {}
```


```python
type(myDic)
```




    dict




```python
len(myDic)
```




    0




```python
myDic ={"name":"Asad", "age": 23, "degree":"BS", "cell":"45454545"}
        
```


```python
myDic["name"]
```




    'Asad'




```python
myDic["age"]
```




    23




```python
myDic["degree"]
```




    'BS'




```python
#methods in dictionary are keys(), values(), items()
```


```python
for k,v in myDic.items():
    print(f"the key is {k},and the value is {v}")
```

    the key is name,and the value is Asd
    the key is age,and the value is 23
    the key is degree,and the value is BS
    the key is cell,and the value is 45454545
    


```python
for k in myDic.keys():
    print(k)
```

    name
    age
    degree
    cell
    


```python
for k in myDic.keys():
    print(myDic[k])
```

    Asd
    23
    BS
    45454545
    


```python
for k in myDic.values():
    print(k)
```

    Asd
    23
    BS
    45454545
    
Method	Description
clear()	Removes all the elements from the dictionary
copy()	Returns a copy of the dictionary
fromkeys()	Returns a dictionary with the specified keys and values
get()	Returns the value of the specified key
items()	Returns a list containing the a tuple for each key value pair
keys()	Returns a list containing the dictionary's keys
pop()	Removes the element with the specified key
popitem()	Removes the last inserted key-value pair
setdefault()	Returns the value of the specified key. If the key does not exist: insert the key, with the specified value
update()	Updates the dictionary with the specified key-value pairs
values()	Returns a list of all the values in the dictionary
# List in List


```python
a = [11,22,33,44]
b = [55,66,77,88]
c = ["apple", "orange", a,b]
c
```




    ['apple', 'orange', [11, 22, 33, 44], [55, 66, 77, 88]]




```python
c[2]
```




    [11, 22, 33, 44]




```python
c[3]
```




    [55, 66, 77, 88]




```python
c[3][2]
```




    77




```python
def add():
    print(10+20)
```


```python
c[3][1:]
```




    [66, 77, 88]




```python
del c[3][1]
```


```python
c
```




    ['apple', 'orange', [11, 22, 33, 44], [55, 77, 88]]




```python
r = ["asd"]
r.remove("asd")
```


```python
r
```




    []




```python
c[2].remove(44)
```


```python
c
```




    ['apple', 'orange', [11, 22, 33], [55, 77, 88]]




```python
# list in list
# dict in list
# tuple in list
# list in dic
# dic in dic
# tuple in dic
# tuple in tuple
# list in tuple
# dic in tuple
```

# Dictionary in List


```python
aa = [11,22,33, myDic]
aa
```




    [11, 22, 33, {'name': 'Asad', 'age': 23, 'degree': 'BS', 'cell': '45454545'}]




```python
aa[3]["age"]
```




    23




```python
pp = [111,222,{'name':[0,999]}]
```


```python
pp[2]['name'][1]
```




    999




```python
del aa[3]["age"]
```


```python
aa
```




    [11, 22, 33, {'name': 'Asad', 'degree': 'BS', 'cell': '45454545'}]



DYS ======>>> Tuple in list

# List in dictionary


```python
dd = {'names':['a','b','c','d','e','f','g','h'] }
```


```python
dd['names']
```




    ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h']




```python
dd['names'][4]
```




    'e'




```python
dd['names'].remove("g")
```


```python
dd
```




    {'names': ['a', 'b', 'c', 'd', 'e', 'f', 'h']}



# dictionary in dictionary


```python
qq = {"names":myDic}
```


```python

```


```python
qq
```




    {'names': {'name': 'Asad', 'degree': 'BS', 'cell': '45454545'}}




```python
qq['names']['cell'] = "333"
qq
```




    {'names': {'name': 'Asad', 'degree': 'BS', 'cell': '333'}}




```python
myDic
```




    {'name': 'Asad', 'degree': 'BS', 'cell': '333'}




```python
tt = {"name":"Saylani", "age":40, "name":"wajahat"}
```


```python
tt
```




    {'name': 'wajahat', 'age': 40}




```python
tt["hello"]="python","piaic", 'nasir'
```


```python
tt
```




    {'name': 'wajahat', 'age': 40, 'hello': ('python', 'piaic', 'nasir')}




```python
x =1,2,3,4,5,6,7,8
```


```python
x
```




    (1, 2, 3, 4, 5, 6, 7, 8)



# How to append a new dictionary to a
list of dictionaries


```python
k =[]

```


```python
k.append({1:1,3:9,4:16})
k
```




    [{1: 1, 3: 9, 4: 16}]



# Functions


```python
#Functions Methods Routines 
```


```python
# def add():  #parameter less
#     print(10+20)
# add()
```


```python
def add(a,b):#PARAMETERS
    print(a+b)
```


```python
add(100,200)#ARGUMENTS
print("The func has run")
```

    300
    The func has run
    


```python
add(1,2)
```

    3
    


```python
add(45,56)
```

    101
    


```python
def full_name(wife_name, husband_name):
    
    print(f"the name if the female is {wife_name} {husband_name}")
```


```python
full_name("saleem","sana")# positional arguments
```

    the name if the female is saleem sana
    


```python
def add(a,b):
    c =a+b
    return c
    print("hello")
```


```python
answer = add(1,2)
```


```python
answer
```




    3




```python
def add(a,b):
    return a+b

```


```python
result  = add("asad", 'khan')
```


```python
result
```




    'asadkhan'




```python
def operation(a,b,operator):
    if operator == "+":
        c = a+b
        return c
    elif operator == "-":
        c = a - b
        return c
    elif operator == '*':
        c = a*b
        return c
    elif operator == "//":
        c = a // b
        return c
    else:
        print("This operator is not define")
```


```python
operation(5 , 4 , "%")
```

    This operator is not define
    


```python
# default parameters 
def name(f_name, m_name=" ", l_name="khan"):
    full_name = f_name + m_name + l_name
    print(full_name)
    
```


```python
name("haasan")
```

    haasan khan 
    


```python
print()
```
