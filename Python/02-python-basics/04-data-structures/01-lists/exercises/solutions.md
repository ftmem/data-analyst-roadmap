# Solutions - List Exercises

## تمرین 1

```python
my_list = []

print(type(my_list))
```

خروجی:

```text
<class 'list'>
```

---

## تمرین 2

```python
fruits = ["Apple", "Orange", "Banana"]

print(len(fruits))
```

خروجی:

```text
3
```

---

## تمرین 3

```python
numbers = [10, 20, 30, 40]

print(numbers[0])
print(numbers[1])
```

خروجی:

```text
10
20
```

---

## تمرین 4

```python
fruits = ["Apple", "Orange", "Banana", "Kiwi"]

print(fruits[-1])
print(fruits[-2])
```

خروجی:

```text
Kiwi
Banana
```

---

## تمرین 5

```python
numbers = [4, 5, 7, 1]

print(numbers[0])
print(numbers[-4])
```

خروجی:

```text
4
4
```

---

## تمرین 6

```python
data = [10, "Python", 2.5]

print(data[0])
print(data[1])
print(data[2])
```

خروجی:

```text
10
Python
2.5
```

---

## تمرین 7

```python
x = ["Apple", "Orange"]
y = ["Carrot", "Potato"]

z = [x, y]

print(z)
```

خروجی:

```text
[['Apple', 'Orange'], ['Carrot', 'Potato']]
```

---

## تمرین 8

```python
x = ["Apple", "Orange"]
y = ["Carrot", "Potato"]

z = [x, y]

print(z[0])
print(z[1][0])
print(z[1][1])
```

خروجی:

```text
['Apple', 'Orange']
Carrot
Potato
```

---

## تمرین 9

```python
data = [
    ["Apple", "Orange"],
    [4, 5, 7, 1],
    ["Carrot", "Potato"],
    ["Kiwi", "Banana", "Mango"]
]

print(data[0])
print(data[0][0])
print(data[1][2])
print(data[3][1])
```

خروجی:

```text
['Apple', 'Orange']
Apple
7
Banana
```

---

## تمرین 10

```python
data = [
    ["Apple", "Orange"],
    [10, 20, 30],
    ["Carrot", "Potato", "Tomato", "Onion"]
]

print(data[0][1])
print(data[1][2])
print(data[2][3])
```

خروجی:

```text
Orange
30
Onion
```

---

## نکته مهم

برای دسترسی به عناصر لیست های تو در تو، باید برای هر سطح از لیست یک `[]` استفاده کنیم.

مثلاً:

```python
data[0][1]
```

یعنی:

1. `data[0]` → لیست اول
2. `[1]` → عنصر دوم آن لیست
