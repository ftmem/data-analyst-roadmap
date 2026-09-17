# حل تمرین های Tuple در Python

## تمرین 1 — ساخت Tuple

```python
numbers = (10, 20, 30, 40, 50)

print(type(numbers))
```

خروجی:

```text
<class 'tuple'>
```

---

## تمرین 2 — Tuple با انواع داده مختلف

```python
data = ("Ali", 25, 18.5)

print(data)
```

---

## تمرین 3 — Tuple یک عضوی

```python
x = (10,)

print(type(x))
```

خروجی:

```text
<class 'tuple'>
```

نکته مهم:

```python
x = (10)
```

یک `int` است، اما:

```python
x = (10,)
```

یک `tuple` است.

---

## تمرین 4 — تبدیل List به Tuple

```python
numbers = [1, 2, 3, 4, 5]

numbers = tuple(numbers)

print(numbers)
```

خروجی:

```text
(1, 2, 3, 4, 5)
```

---

## تمرین 5 — تبدیل String به Tuple

```python
text = "Python"

result = tuple(text)

print(result)
```

خروجی:

```text
('P', 'y', 't', 'h', 'o', 'n')
```

---

## تمرین 6 — دسترسی به اعضای Tuple

```python
names = ("Ali", "Sara", "Reza", "Mina")

print(names[0])
print(names[1])
print(names[-1])
```

خروجی:

```text
Ali
Sara
Mina
```

---

## تمرین 7 — اندیس منفی

```python
numbers = (10, 20, 30, 40, 50)

print(numbers[-1])
print(numbers[-2])
```

خروجی:

```text
50
40
```

---

## تمرین 8 — Slicing

```python
numbers = (0, 1, 2, 3, 4, 5, 6, 7, 8, 9)

print(numbers[0:4])
print(numbers[4:])
print(numbers[0:10:2])
```

خروجی:

```text
(0, 1, 2, 3)
(4, 5, 6, 7, 8, 9)
(0, 2, 4, 6, 8)
```

---

## تمرین 9 — divmod

```python
result = divmod(17, 5)

print(result)
print(type(result))
```

خروجی:

```text
(3, 2)
<class 'tuple'>
```

---

## تمرین 10 — تکرار Tuple

```python
x = (1,)

print(x * 3)
```

خروجی:

```text
(1, 1, 1)
```

---

## تمرین 11 — Tuple تو در تو

```python
data = (10, (20, 30, 40))

print(data[0])
print(data[1])
print(data[1][1])
```

خروجی:

```text
10
(20, 30, 40)
30
```

---

## تمرین 12 — count

```python
numbers = (1, 2, 2, 3, 2, 4, 2)

print(numbers.count(2))
```

خروجی:

```text
4
```

---

## تمرین 13 — index

```python
names = ("Ali", "Sara", "Reza", "Sara", "Mina")

print(names.index("Sara"))
print(names.index("Mina"))
```

خروجی:

```text
1
4
```

---

## تمرین 14 — Tuple Unpacking

```python
data = (10, 20, 30)

a, b, c = data

print(a)
print(b)
print(c)
```

خروجی:

```text
10
20
30
```

---

## تمرین 15 — Unpacking از خروجی تابع

```python
def get_data():
    return 100, 200, 300


a, b, c = get_data()

print(a)
print(b)
print(c)
```

خروجی:

```text
100
200
300
```

---

## تمرین 16 — عدم تغییر Tuple

```python
numbers = (1, 2, 3)

numbers[0] = 10
```

این کد باعث خطا می شود، چون Tuple قابل تغییر نیست.

خطای اصلی:

```text
TypeError
```

---

## تمرین 17 — ساخت Tuple جدید

```python
numbers = (10, 20, 30)

new_numbers = (100,) + numbers[1:]

print(new_numbers)
```

خروجی:

```text
(100, 20, 30)
```

Tuple اصلی همچنان بدون تغییر باقی می ماند:

```python
print(numbers)
```

خروجی:

```text
(10, 20, 30)
```

---

## تمرین 18 — تمرین ترکیبی

```python
numbers = (10, 20, 20, 30, 40, 20, 50)

print(len(numbers))
print(numbers.count(20))
print(numbers.index(20))
print(numbers[-1])
print(numbers[:3])
```

خروجی:

```text
7
3
1
50
(10, 20, 20)
```

---

## تمرین 19 — ترکیب Tuple و List

```python
numbers = [1, 2, 3, 4]

numbers = tuple(numbers)

print(numbers[2])
```

خروجی:

```text
3
```

---

## تمرین 20 — تمرین نهایی Tuple

```python
data = (
    "Python",
    10,
    20,
    (30, 40, 50)
)

print(data[0])
print(data[1])
print(data[3][2])
print(data[3])
print(type(data))
print(type(data[3]))
```

خروجی:

```text
Python
10
50
(30, 40, 50)
<class 'tuple'>
<class 'tuple'>
```

---

# خلاصه Tuple

مهم ترین مواردی که در این بخش یاد گرفتیم:

```text
tuple()
()
اندیس گذاری
اندیس منفی
Slicing
count()
index()
Unpacking
Nested Tuple
divmod()
```

و مهم ترین ویژگی Tuple:

```text
Tuple → Immutable
```

یعنی بعد از ساخته شدن، اعضای آن را نمی توانیم مستقیماً تغییر دهیم.

