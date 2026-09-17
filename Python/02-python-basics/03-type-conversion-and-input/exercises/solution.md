# Solutions — Type Conversion and Input

## تمرین 1 — تبدیل String به Integer

```python
number = "123"

number = int(number)

print(number)
print(type(number))
```

خروجی:

```text
123
<class 'int'>
```

---

## تمرین 2 — تبدیل String به Float

```python
number = "12.5"

number = float(number)

print(number)
print(type(number))
```

خروجی:

```text
12.5
<class 'float'>
```

---

## تمرین 3 — تفاوت String و Number

```python
print(100 * 2)
print("100" * 2)
```

خروجی:

```text
200
100100
```

عدد `100` یک `int` است، بنابراین در `2` ضرب می شود.

اما `"100"` یک `str` است و ضرب رشته در عدد باعث تکرار رشته می شود.

---

## تمرین 4 — تبدیل Integer به String

```python
number = 250

number = str(number)

print(number)
print(type(number))
```

خروجی:

```text
250
<class 'str'>
```

---

## تمرین 5 — `chr()`

```python
print(chr(65))
print(chr(66))
print(chr(97))
print(chr(98))
```

خروجی:

```text
A
B
a
b
```

---

## تمرین 6 — `ord()`

```python
print(ord("A"))
print(ord("B"))
print(ord("a"))
print(ord("b"))
```

خروجی:

```text
65
66
97
98
```

---

## تمرین 7 — `round()`

```python
number = 12.5867

print(round(number, 2))
```

خروجی:

```text
12.59
```

---

## تمرین 8 — `divmod()`

```python
result = divmod(25, 4)

print(result)
```

خروجی:

```text
(6, 1)
```

یعنی:

```text
خارج قسمت = 6
باقی مانده = 1
```

---

## تمرین 9 — `pow()`

```python
result = pow(2, 3)

print(result)
```

خروجی:

```text
8
```

---

## تمرین 10 — ورودی کاربر

```python
name = input("Enter your name: ")

print("Hello", name)
```

---

## تمرین 11 — ورودی عدد صحیح

```python
number = int(input("Enter a number: "))

print(number * 2)
```

مثلاً:

```text
Enter a number: 10
20
```

---

## تمرین 12 — ورودی عدد اعشاری

```python
number = float(input("Enter a number: "))

print(number / 2)
```

مثلاً:

```text
Enter a number: 5.5
2.75
```

---

## تمرین 13 — جمع دو عدد

```python
a = int(input("Enter the first number: "))
b = int(input("Enter the second number: "))

print(a + b)
```

مثلاً:

```text
Enter the first number: 10
Enter the second number: 20
30
```

---

## تمرین 14 — تبدیل مبنای 2

```python
number = int("1010", 2)

print(number)
```

خروجی:

```text
10
```

---

## تمرین 15 — ترکیب Input و Type Conversion

```python
name = input("Enter your name: ")
age = int(input("Enter your age: "))

next_year_age = age + 1

print(name, "will be", next_year_age, "next year.")
```

مثلاً:

```text
Enter your name: Fatemeh
Enter your age: 28

Fatemeh will be 29 next year.
```

---

## نکات مهم

### `input()` همیشه String برمی گرداند

```python
number = input("Enter a number: ")
```

برای تبدیل به عدد صحیح:

```python
number = int(input("Enter a number: "))
```

برای تبدیل به عدد اعشاری:

```python
number = float(input("Enter a number: "))
```

### تبدیل های مهم

```text
int()    → عدد صحیح
float()  → عدد اعشاری
str()    → رشته
chr()    → کد عددی به کاراکتر
ord()    → کاراکتر به کد عددی
```
