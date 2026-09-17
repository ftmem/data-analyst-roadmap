# حل تمرین های List در Python

## تمرین 1 — ساخت لیست

```python
fruits = ["Apple", "Orange", "Banana", "Mango"]

print(type(fruits))
print(len(fruits))
```

خروجی:

```text
<class 'list'>
4
```

---

## تمرین 2 — دسترسی به اعضای لیست

```python
numbers = [10, 20, 30, 40, 50]

print(numbers[0])
print(numbers[-1])
print(numbers[2])
print(numbers[-2])
```

خروجی:

```text
10
50
30
40
```

---

## تمرین 3 — اندیس منفی

```python
names = ["Ali", "Sara", "Reza", "Mina", "Nima"]

print(names[-1])
print(names[-2])
print(names[-4])
```

خروجی:

```text
Nima
Mina
Sara
```

---

## تمرین 4 — تغییر عضو لیست

```python
numbers = [1, 2, 3, 4, 5]

numbers[2] = 10

print(numbers)
```

خروجی:

```text
[1, 2, 10, 4, 5]
```

---

## تمرین 5 — Slicing

```python
numbers = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

print(numbers[0:4])
print(numbers[4:])
print(numbers[0:10:2])
print(numbers[0:10:3])
```

خروجی:

```text
[0, 1, 2, 3]
[4, 5, 6, 7, 8, 9]
[0, 2, 4, 6, 8]
[0, 3, 6, 9]
```

---

## تمرین 6 — len ،min و max

```python
numbers = [15, 8, 23, 4, 42, 10]

print(len(numbers))
print(min(numbers))
print(max(numbers))
```

خروجی:

```text
6
4
42
```

---

## تمرین 7 — بررسی وجود یک عضو

```python
names = ["Ali", "Sara", "Reza", "Mina"]

print("Reza" in names)
print("Mehdi" in names)
```

خروجی:

```text
True
False
```

---

## تمرین 8 — ترکیب دو لیست

```python
a = [1, 2, 3]
b = [4, 5, 6]

result = a + b

print(result)
```

خروجی:

```text
[1, 2, 3, 4, 5, 6]
```

---

## تمرین 9 — append

```python
numbers = [1, 2, 3]

numbers.append(4)
numbers.append(5)
numbers.append(6)

print(numbers)
```

خروجی:

```text
[1, 2, 3, 4, 5, 6]
```

---

## تمرین 10 — count

```python
numbers = [1, 2, 2, 3, 2, 4, 5, 2]

print(numbers.count(2))
```

خروجی:

```text
4
```

---

## تمرین 11 — append و extend

### حالت اول: append

```python
a = [1, 2, 3]
b = [4, 5, 6]

a.append(b)

print(a)
```

خروجی:

```text
[1, 2, 3, [4, 5, 6]]
```

در این حالت کل `b` به عنوان **یک عضو** به `a` اضافه شده است.

### حالت دوم: extend

```python
a = [1, 2, 3]
b = [4, 5, 6]

a.extend(b)

print(a)
```

خروجی:

```text
[1, 2, 3, 4, 5, 6]
```

در `extend()` اعضای `b` به صورت جداگانه به انتهای `a` اضافه می شوند.

---

## تمرین 12 — index

```python
names = ["Ali", "Sara", "Reza", "Sara", "Mina"]

print(names.index("Sara"))
print(names.index("Sara", 2))
```

خروجی:

```text
1
3
```

در دستور دوم، جستجو از اندیس `2` شروع می شود.

---

## تمرین 13 — insert

```python
numbers = [1, 2, 4, 5]

numbers.insert(2, 3)

print(numbers)
```

خروجی:

```text
[1, 2, 3, 4, 5]
```

---

## تمرین 14 — pop و del

```python
numbers = [10, 20, 30, 40, 50]

numbers.pop()
print(numbers)

numbers.pop(1)
print(numbers)

del numbers[0]
print(numbers)
```

خروجی:

```text
[10, 20, 30, 40]
[10, 30, 40]
[30, 40]
```

---

## تمرین 15 — reverse

```python
numbers = [1, 2, 3, 4, 5]

numbers.reverse()

print(numbers)
```

خروجی:

```text
[5, 4, 3, 2, 1]
```

---

## تمرین 16 — تبدیل String به List

```python
name = "Python"

letters = list(name)

print(letters)
```

خروجی:

```text
['P', 'y', 't', 'h', 'o', 'n']
```

---

## تمرین 17 — sort

### مرتب سازی صعودی

```python
numbers = [5, 2, 9, 1, 7, 3]

numbers.sort()

print(numbers)
```

خروجی:

```text
[1, 2, 3, 5, 7, 9]
```

### مرتب سازی نزولی

```python
numbers = [5, 2, 9, 1, 7, 3]

numbers.sort(reverse=True)

print(numbers)
```

خروجی:

```text
[9, 7, 5, 3, 2, 1]
```

---

## تمرین 18 — مرتب سازی رشته ها

```python
names = ["Ali", "Mohammad", "Sara", "Reza", "Mina"]

names.sort()

print(names)
```

خروجی:

```text
['Ali', 'Mina', 'Mohammad', 'Reza', 'Sara']
```

---

## تمرین 19 — مرتب سازی بر اساس طول

```python
words = ["cat", "elephant", "dog", "computer", "hi"]

words.sort(key=len)

print(words)
```

خروجی:

```text
['hi', 'cat', 'dog', 'computer', 'elephant']
```

---

## تمرین 20 — لیست تو در تو

```python
x = ["Apple", "Orange"]
y = ["Carrot", "Potato"]

z = [x, y]

print(z[0][0])
print(z[0][1])
print(z[1][0])
print(z[1][1])
```

خروجی:

```text
Apple
Orange
Carrot
Potato
```

---

## تمرین 21 — لیست های تو در تو با طول متفاوت

```python
data = [
    [1, 2],
    [3, 4, 5],
    [6],
    [7, 8, 9, 10]
]

print(data[1][2])
print(data[2][0])
print(data[3][2])
print(data[3][3])
```

خروجی:

```text
5
6
9
10
```

---

## تمرین 22 — کار با اعضای عددی به شکل String

```python
numbers = ["1", "94", "93", "1000"]

print(max(numbers))
```

خروجی:

```text
94
```

دلیل این است که اعضای لیست **رشته هستند، نه عدد**.

بنابراین `max()` آن ها را به صورت رشته ای مقایسه می کند.

مثلاً:

```text
"94"
```

از نظر مقایسه رشته ای می تواند از:

```text
"1000"
```

بزرگ تر باشد، چون مقایسه از اولین کاراکتر شروع می شود.

---

## تمرین 23 — تبدیل اعضای لیست

```python
numbers = ["10", "20", "30", "40"]

numbers = [int(x) for x in numbers]

print(numbers)
```

خروجی:

```text
[10, 20, 30, 40]
```

نکته: در اینجا هر عضو جداگانه به `int` تبدیل شده است.

---

## تمرین 24 — تمرین ترکیبی

```python
numbers = [10, 20, 30, 20, 40, 20, 50]

print(len(numbers))
print(max(numbers))
print(min(numbers))
print(numbers.count(20))
print(numbers.index(20))
```

خروجی:

```text
7
50
10
3
1
```

---

# تمرین 25 — تمرین نهایی List

```python
numbers = [5, 2, 8, 2, 10, 3, 8, 1]

# 1. بزرگ ترین عدد
print(max(numbers))

# 2. کوچک ترین عدد
print(min(numbers))

# 3. تعداد اعضا
print(len(numbers))

# 4. تعداد تکرار عدد 2
print(numbers.count(2))

# 5. اضافه کردن 6
numbers.append(6)

# 6. اضافه کردن 7 در جایگاه مناسب
numbers.insert(5, 7)

# 7. مرتب سازی صعودی
numbers.sort()

# 8. چاپ لیست نهایی
print(numbers)
```

خروجی:

```text
10
1
8
2
[1, 2, 2, 3, 5, 6, 7, 8, 8, 10]
```

## نکته مهم

در تمرین های این بخش با مهم ترین عملیات List کار کردیم:

```text
Indexing
Negative Indexing
Slicing
len()
min()
max()
in
+
append()
extend()
count()
index()
insert()
pop()
del
reverse()
sort()
```

این ها پایه ی کار با `list` در پایتون هستند.
