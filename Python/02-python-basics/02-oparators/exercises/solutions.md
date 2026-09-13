# Solutions — Operators

راه حل تمرین های مربوط به عملگرهای مقایسه ای، منطقی و Bitwise.

---

## تمرین 1 — عملگرهای مقایسه ای

```python
a = 10
b = 5

print(a == b)
print(a != b)
print(a > b)
print(a < b)
print(a >= b)
print(a <= b)
```

خروجی:

```text
False
True
True
False
True
False
```

---

## تمرین 2 — بررسی نوع Boolean

```python
print(type(10 > 5))
print(type(10 == 5))
print(type(10 != 5))
```

خروجی:

```text
<class 'bool'>
<class 'bool'>
<class 'bool'>
```

---

## تمرین 3 — محدوده عدد

```python
age = 25

print(age >= 18 and age <= 30)
```

خروجی:

```text
True
```

---

## تمرین 4 — استفاده از `and`

```python
x = 15
y = 8

print(x > 10 and y < 10)
```

خروجی:

```text
True
```

---

## تمرین 5 — استفاده از `or`

```python
score = 18

print(score >= 18 or score < 5)
```

خروجی:

```text
True
```

---

## تمرین 6 — استفاده از `not`

```python
x = 10

print(not (x > 5))
```

خروجی:

```text
False
```

---

## تمرین 7 — XOR

```python
print(True ^ False)
print(True ^ True)
print(False ^ False)
print(False ^ True)
```

خروجی:

```text
True
False
False
True
```

---

## تمرین 8 — چند متغیر در یک خط

```python
a, b, c = 10, 20, 30

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

## تمرین 9 — Bitwise AND

```python
a = 2
b = 3

print(a & b)
```

خروجی:

```text
2
```

محاسبه بیتی:

```text
  10
& 11
----
  10
```

---

## تمرین 10 — Bitwise OR

```python
a = 2
b = 3

print(a | b)
```

خروجی:

```text
3
```

محاسبه بیتی:

```text
  10
| 11
----
  11
```

---

## تمرین 11 — Bitwise XOR

```python
a = 2
b = 3

print(a ^ b)
```

خروجی:

```text
1
```

محاسبه بیتی:

```text
  10
^ 11
----
  01
```

---

## تمرین 12 — تبدیل به مبنای 2

```text
2  = 10
3  = 11
5  = 101
8  = 1000
10 = 1010
```

---

## تمرین 13 — شیفت به چپ

```python
x = 5

print(x << 1)
print(x << 2)
print(x << 3)
```

خروجی:

```text
10
20
40
```

هر بار شیفت یک واحد به چپ، مقدار عدد را برای اعداد مثبت در این مثال دو برابر می کند.

---

## تمرین 14 — شیفت به راست

```python
x = 40

print(x >> 1)
print(x >> 2)
print(x >> 3)
```

خروجی:

```text
20
10
5
```

هر بار شیفت یک واحد به راست، مقدار عدد صحیح مثبت را تقریباً به نصف می رساند.

---

## تمرین 15 — ترکیب عملگرها

```python
a = 12
b = 8

print(a > b)
print(a > 10 and b < 10)
print(a == b)
print(a != b)
print(a < 10 or b < 10)
```

خروجی:

```text
True
True
False
True
True
```

---

## نکته مهم

عملگرهای مقایسه ای نتیجه ای از نوع `bool` تولید می کنند:

```python
True
False
```

عملگرهای منطقی برای ترکیب این نتایج استفاده می شوند:

```python
and
or
not
```

و عملگرهای Bitwise روی بیت های اعداد کار می کنند:

```python
&
|
^
<<
>>
```
