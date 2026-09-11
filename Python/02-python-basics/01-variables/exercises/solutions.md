# Solutions — Variables

در این فایل، راه‌حل تمرین‌های مربوط به متغیرها، نوع داده، `print()`، `type()` و عملگرهای ریاضی قرار دارد.

---

## تمرین 1 — تعریف متغیر

```python
x = 10
y = 5

print(x)
print(y)
```

---

## تمرین 2 — جمع دو متغیر

```python
a = 15
b = 7

print(a + b)
```

خروجی:

```text
22
```

---

## تمرین 3 — بررسی نوع متغیر

```python
x = 20
name = "Python"

print(type(x))
print(type(name))
```

خروجی:

```text
<class 'int'>
<class 'str'>
```

---

## تمرین 4 — محاسبات ریاضی

```python
a = 20
b = 6

print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a // b)
print(a % b)
print(a ** b)
```

---

## تمرین 5 — تفاوت عدد و رشته

```python
a = 1
b = "1"

print(type(a))
print(type(b))
```

خروجی:

```text
<class 'int'>
<class 'str'>
```

توضیح:

`a` یک عدد صحیح از نوع `int` است، اما `b` یک رشته از نوع `str` است.

---

## تمرین 6 — محاسبه با متغیرها

```python
a = 10
b = 5
c = 2

print((a + b) * c)
```

خروجی:

```text
30
```

---

## تمرین 7 — استفاده از عبارت داخل print

```python
print(10 + 5)
print(20 - 8)
print(6 * 4)
print(20 / 5)
print(20 // 3)
print(20 % 3)
print(2 ** 4)
```

خروجی:

```text
15
12
24
4.0
6
2
16
```

---

## تمرین 8 — ساخت چند متغیر

```python
name = "Roya"
age = 28
score = 18.5

print(name)
print(age)
print(score)

print(type(name))
print(type(age))
print(type(score))
```

خروجی:

```text
Roya
28
18.5
<class 'str'>
<class 'int'>
<class 'float'>
```

---

## تمرین 9 — نام‌گذاری متغیرها

نام‌های معتبر:

```text
name
age2
my_name
studentName
```

نام‌های نامعتبر:

```text
2name
for
my-name
```

دلیل:

- `2name` → نام متغیر نمی‌تواند با عدد شروع شود.
- `for` → کلمه رزروشده در Python است.
- `my-name` → علامت `-` برای نام‌گذاری متغیر مناسب نیست.

---

## تمرین 10 — محاسبه میانگین

```python
score1 = 15
score2 = 18
score3 = 17

average = (score1 + score2 + score3) / 3

print(average)
```

خروجی:

```text
16.666666666666668
```
