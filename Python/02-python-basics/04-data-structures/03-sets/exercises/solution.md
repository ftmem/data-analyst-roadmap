# ✅ Solutions — Set در پایتون

## تمرین 1

```python
numbers = {1, 2, 3, 4, 5}

print(numbers)
print(type(numbers))
```

---

## تمرین 2

```python
numbers = [1, 2, 2, 3, 3, 3, 4, 5, 5]

numbers_set = set(numbers)

print(numbers_set)
```

اعضای تکراری هنگام تبدیل `list` به `set` حذف می شوند.

---

## تمرین 3

```python
numbers = set()

numbers.add(10)

print(numbers)
```

---

## تمرین 4

```python
numbers = {1, 2, 3}

numbers.add(4)
numbers.add(5)

print(numbers)
```

---

## تمرین 5

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}

print(set1)
print(set2)
```

---

## تمرین 6

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}

result = set1.union(set2)

print(result)
```

خروجی:

```text
{1, 2, 3, 4, 5}
```

---

## تمرین 7

```python
set1 = {1, 2, 3, 4}
set2 = {3, 4, 5, 6}

result = set1.intersection(set2)

print(result)
```

خروجی:

```text
{3, 4}
```

---

## تمرین 8

```python
set1 = {1, 2, 3, 4}
set2 = {3, 4, 5, 6}

print(set1.difference(set2))
print(set2.difference(set1))
```

خروجی:

```text
{1, 2}
{5, 6}
```

نکته: `difference()` جهت دار است.

---

## تمرین 9

```python
set1 = {1, 2, 3, 4}
set2 = {3, 4, 5, 6}

result = set1.symmetric_difference(set2)

print(result)
```

خروجی:

```text
{1, 2, 5, 6}
```

---

## تمرین 10

```python
set1 = {1, 2, 3}
set2 = {4, 5, 6}

result = set1.isdisjoint(set2)

print(result)
```

خروجی:

```text
True
```

چون هیچ عضو مشترکی ندارند.

---

## تمرین 11

```python
set1 = {1, 2}
set2 = {1, 2, 3, 4}

result = set1.issubset(set2)

print(result)
```

خروجی:

```text
True
```

---

## تمرین 12

```python
set1 = {1, 2}
set2 = {1, 2, 3, 4}

result = set2.issuperset(set1)

print(result)
```

خروجی:

```text
True
```

---

## تمرین 13

```python
set1 = {1, 2, 3}
set2 = {1, 2, 3}

print(set1.issubset(set2))
print(set1.issuperset(set2))
```

خروجی:

```text
True
True
```

چون دو Set دقیقاً اعضای یکسانی دارند.

---

## تمرین 14

```python
numbers = {1, 2, 3, 4, 5}

numbers.remove(3)

print(numbers)
```

خروجی:

```text
{1, 2, 4, 5}
```

---

## تمرین 15

```python
numbers = {10, 20, 30, 40}

removed = numbers.pop()

print("Removed:", removed)
print("Set:", numbers)
```

نکته: در `set` ترتیب مشخصی وجود ندارد؛ بنابراین نباید انتظار داشته باشیم `pop()` همیشه یک عضو خاص را حذف کند.

---

## تمرین 16

```python
numbers = {1, 2, 3, 4, 5}

numbers.clear()

print(numbers)
```

خروجی:

```text
set()
```

---

## تمرین 17

```python
names = [
    "Ali",
    "Sara",
    "Ali",
    "Reza",
    "Sara",
    "Mina",
    "Ali"
]

unique_names = set(names)

print(unique_names)
```

اعضای تکراری حذف می شوند.

---

## تمرین 18

```python
python_students = {"Ali", "Sara", "Reza", "Mina"}
data_students = {"Sara", "Mina", "Hamed", "Nima"}

common_students = python_students.intersection(data_students)

print(common_students)
```

خروجی:

```text
{'Sara', 'Mina'}
```

---

## تمرین 19

```python
python_students = {"Ali", "Sara", "Reza", "Mina"}
data_students = {"Sara", "Mina", "Hamed", "Nima"}

result = python_students.difference(data_students)

print(result)
```

خروجی:

```text
{'Ali', 'Reza'}
```

---

## تمرین 20

```python
python_students = {"Ali", "Sara", "Reza", "Mina"}
data_students = {"Sara", "Mina", "Hamed", "Nima"}

all_students = python_students.union(data_students)

print(all_students)
```

خروجی شامل:

```text
Ali
Sara
Reza
Mina
Hamed
Nima
```

ترتیب نمایش اعضای Set تضمین شده نیست.

---

## تمرین 21

```python
python_students = {"Ali", "Sara", "Reza", "Mina"}
data_students = {"Sara", "Mina", "Hamed", "Nima"}

result = python_students.symmetric_difference(data_students)

print(result)
```

خروجی شامل:

```text
{'Ali', 'Reza', 'Hamed', 'Nima'}
```

---

## تمرین 22

```python
A = {1, 2, 3}
B = {4, 5, 6}

print(A.isdisjoint(B))
```

خروجی:

```text
True
```

چون هیچ عضو مشترکی ندارند.

---

## تمرین 23

```python
A = {1, 2}
B = {1, 2, 3, 4, 5}

print(A.issubset(B))
print(B.issuperset(A))
print(not A.isdisjoint(B))
```

خروجی:

```text
True
True
True
```

---

## تمرین 24

```python
numbers = [1, 2, 2, 3, 4, 4, 5, 5, 5, 6]

unique_numbers = set(numbers)

print(unique_numbers)
print(len(unique_numbers))
```

تعداد اعضای یکتا:

```text
6
```

---

# ⭐ تمرین 25 — چالش نهایی

```python
list1 = [1, 2, 3, 4, 5, 5, 5]
list2 = [4, 5, 6, 7, 7, 8]

set1 = set(list1)
set2 = set(list2)
```

### 1. تمام اعضای موجود در هر دو مجموعه

```python
all_members = set1.union(set2)

print(all_members)
```

نتیجه:

```text
{1, 2, 3, 4, 5, 6, 7, 8}
```

### 2. اعضای مشترک

```python
common_members = set1.intersection(set2)

print(common_members)
```

نتیجه:

```text
{4, 5}
```

### 3. اعضایی که فقط در `list1` هستند

```python
only_list1 = set1.difference(set2)

print(only_list1)
```

نتیجه:

```text
{1, 2, 3}
```

### 4. اعضایی که فقط در `list2` هستند

```python
only_list2 = set2.difference(set1)

print(only_list2)
```

نتیجه:

```text
{6, 7, 8}
```

### 5. اعضایی که فقط در یکی از دو مجموعه هستند

```python
only_one = set1.symmetric_difference(set2)

print(only_one)
```

نتیجه:

```text
{1, 2, 3, 6, 7, 8}
```

### 6. بررسی `disjoint`

```python
result = set1.isdisjoint(set2)

print(result)
```

خروجی:

```text
False
```

چون دو مجموعه اعضای مشترک `4` و `5` دارند.

---

# 📌 خلاصه متدهای مهم Set

| متد | کاربرد |
|---|---|
| `add()` | اضافه کردن یک عضو |
| `union()` | اجتماع دو Set |
| `intersection()` | اشتراک دو Set |
| `difference()` | اعضای موجود در Set اول و نبودن در Set دوم |
| `symmetric_difference()` | اعضای غیرمشترک دو Set |
| `isdisjoint()` | بررسی نداشتن عضو مشترک |
| `issubset()` | بررسی زیرمجموعه بودن |
| `issuperset()` | بررسی ابرمجموعه بودن |
| `remove()` | حذف یک عضو |
| `pop()` | حذف و برگرداندن یک عضو |
| `clear()` | خالی کردن Set |
