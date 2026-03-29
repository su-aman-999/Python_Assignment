# Python Assignment (MySirG)

## Assignment-1: Warmup

1. Who developed Python? - **Guido Van Rossum**
2. When was the first version of Python launched? - **20 February 1991 (Python 0.9.0.)**
3. “Python is a platform independent language” - **True**
4. How to make single line comment in a python file? - `#`
5. “Python is a statically typed programming language” - **True**

## Assignment-2: Fundamentals of Python

1. Write a command to get the Python version you are using. - `python --version`
2. What is PVM? - **Python Virtual Machine**
3. How to create .pyc (Byte Code) file from Python source file? - `python -m compileall myfile.py`
4. How to run a Python file from command prompt or terminal? - `Python file_name.py`
5. “Data Types in Python are not keywords” - **True**

## Assignment-3: Simple problems on print

1. Write a python script to print MySirG on the screen. <br>

```python
print("MySirG")
```

2. Write a python script to print MySirG on the first line and Education Services on the second line.

```python
print("MySirG", "\nEucation Services",)
```

3. Write a python script to print "MySirG" on the screen. (Remember to print double quotes)

```python
print("\"MySirG\"")
```

4. Write a Python script to print "Teacher’s Day" on the screen. (Remember to print double quotes and
   single quote)

```python
print("\"Teacher's Day\"")
```

5. Write a python script to print \n on the screen.

```python
print("\\n")
```

## Assignment-4: Playing with Variables

1. Write a python script containing a variable with some integer value, print value of this variable.

```python
num = 10
print("Value: ", num)
```

2. Write a python script to print the value of a variable. Variable contains your name as data.

```python
name = "aman kumar"
print("name: ", name)
```

3. Write a python script to print values of three variables, each in a new line. All three variables are filled with some integer values.

```python
num1 = 10
num2 = 20
num3 = 30

print("num1:", num1)
print("num2:", num2)
print("num3:", num3)
```

4. Create 5 variables each of them containing different types of data (like 35, True, “MySirG”, 5.46,3+4j, etc). Write a python script to print values of all the variables along with their data types.

```python
number = 35
indian = True
string = "MySirG"
decimalNum = 5.7
complexNum = 3+4j

print("number:", number, "->", type(number))
print("indian:", indian, "->", type(indian))
print("string:", string, "->", type(string))
print("decimalNum:", decimalNum, "->", type(decimalNum))
print("complexNum:", complexNum, "->", type(complexNum))
```

5. Create three variables and assign current date to them, first variable contains day number, second variable contains month number and third variable contains year number. Write a python script to display date in standard way (e.g. 29/11/2022).

```python
day = 21
month = 3
year = 2026
print(day,month,year, sep = "/")
print(f"{day:02d}/{month:02d}/{year}")
```

> **Note:** <br>
> f"" = formatted string <br>
> {} → variable/expr insert <br>
> {num:02d} → 2 digit (zero add) <br>

## Assignment-5: Import and Keywords

1. Write a python script to print all the keywords on the screen.

```python
import keyword
print(keyword.kwlist)
```

> **Keyword:** [`False`, `None`, `True`, `and`, `as`, `assert`, `async`, `await`, `break`, `class`, `continue`, `def`, `del`, `elif`, `else`, `except`, `finally`, `for`, `from`, `global`, `if`, `import`, `in`, `is`, `lambda`, `nonlocal`, `not`, `or`, `pass`, `raise`, `return`, `try`, `while`, `with`, `yield`]

2. Use help section on python shell to see all the keywords.

```python
help("keywords")
```

3. Create two Python files A0.py and A1.py. Create a variable in A1.py and assign some value to it Write a Python script to import A1 module in A0 and print value of the variable created in A0.py

- In, **A1.py**

```python
num1 = 10
```

- In, **A0.py**

```python
from A1 import num1 as value
print(value)
```

4. Out of all the keywords, name those keywords which are used as data.

   > **Ans:** `True`, `False` and `None`

5. What is the use of del keyword?
   > **Ans:** We use del keywprd fro delete any `variables` or `objects`

## Assignment-6: Type Conversion

1. Write a python script to convert a number into str type.

```python
num = 10
print(f"Data: {num}, Type: {type(num)}")
num = str(num)
print(f"Data: {num}, Type: {type(string)}")
```

> **Type Conversion Method**
>
> - `int()` <br>
> - `float()` <br>
> - `str()` <br>
> - `bool()` <br>
> - `complex()`

> **In Number System** <br>
> `num = 5` <br>
>
> - `bin(num)` → `'0b11001'` <br>
> - `oct(num)` → `'031'` <br>
> - `hex(num)` → `'0x19'` <br>

2. Write a python script to print Unicode of the character 'm'

```python
v1 = "m"
v2 = 97
print(ord(v1))
print(chr(v2))
```

> **unicode**
>
> - **UTF:** `Unicode Transformation formate`
> - **Methods** <br>
>   - `chr(m)` → `109`
>   - `ord(97)` → `a`

3. Write a python script to print character representation of a given unicode 100.

```python
print(chr(100))
```

4. Write a python script to convert a str type data into an int type. Also describe when a str type value is not possible to convert into an int type.

```python
data = "10"
print(f"data is {int(data)} and type is {type(int(data))}")
```

> - `int("abc")` → alphabets <br>
> - `int("10a")` → mixed <br>
> - `int("")` → empty string
> - Always return **String**

5. How to convert an integer value into a bool value?

```python
num = 10
print(bool(num))
```

## Assignment-7: Number System

**Note**

```python
repr("aman") # "'aman'"
str("aman") # 'aman'
print("aman") # aman
```

- `import math`

```python
import math
math.floor(3.4) # Closed Value
math.trunc(2.8) # 2 -> 0 <-
math.trunc(-2.8) # -2
```

- `import random`

```python
import random
random.random() # 0.34486464583559906

random.randint(1, 10) # 8

l1 = ["mumbai", "patna", "meerut", "varanasi", "gaya"]

random.choice(l1) # random values in array

random.shuffle(l1) # element postion changes
```

- `from decimal import Decimal`
  solution of this problem (0.2 + 0.1)

```python
from decimal import Decimal
Decimal("0.1") + Decimal("0.2") # Decimal('0.3')
```

1. Write a python script to print any number and its binary equivalent.

```python
num = 10
print(bin(num))
```

2. Write a python script to store binary number 1100101 in a variable and print it in decimal format.

```python
bin1 = 0b1100101
dec1 = int(bin1)
print(dec1)

bin2 = "1100101"
dec2 = int(bin2, 2)
print(dec2)
```

> **Note**
>
> - `int("10110", 2)` → binary → decimal <br>
> - base = 2 → binary
> - only `int()` supports and `bin()`, `hex()` and `oct()` don't support.
> - First of all **any string numbers** → `integer` → `binary`, `hexa decimal` and `octal`

3. Write a python script to store a hexadecimal number 2F in a variable and print it in octal format.

```python
hex1 = 0x1f6a
oct1 = oct(hex1)
print(oct1)

hex2 = "1f6a"
dec = int(hex2, 16)
oct2 = oct(dec)
print(oct2)
```

4. Write a python script to store an octal number 125 in a variable and print it in binary format.

```python
octal = 0o125
print(bin(octal))
```

5. Write a python script to add two numbers 25 (in octal) and 39 (in hexadecimal) and display the result in binary format.

```python
oNum = 0o25
hNum = 0x39
print(int(oNum + hNum))
```

## Assignment-8: Input from keyboard

1. Write a python script to take your name as input from the user and then print it.

```python
print(input("Enter your name: "))
```

2. Write a python script to take input two numbers form the user, then calculate their sum and display the result.

```python
print(f"Result: {int(input("num1: ")) + int(input("num2:"))}")
```

3. Write a python script which takes the radius from the user and display area of the circle.

```python
print(f"Area: {3.14 * int(input("Enter Radius: "))}")
```

4. Write a python script to calculate square of a number. Number is entered by the user.

```python
print(int(input("Enter Number: ")) ** 2)
```

5. Write a python script which takes a character from the user and display its unicode.

```python
print(f"Unicode {ord(input("Enter Character: "))}")
```

## Assignment-9: Simple calculations on user data

1. Write a python script to calculate simple interest.

```python
print(f"SI: { float(input("amm: ")) * float(input("time: ")) * float(input("inte: "))/100}")
```

2. Write a python script to calculate area of a rectangle.

```python
print(f"Area: {int(input("Width: ")) * int(input("Height: "))}")
```

3. Write a python script to calculate average of three numbers entered by user.

```python
print(f"Average: {(int(input("Num1: ")) + int(input("Num2:  ")) + int(input("Num3: ")))/3}")
```

4. Write a python script to calculate volume of a cuboid.

```python
print(f"Volume: {int(input("l: ")) * int(input("b: ")) * int(input("h: "))}")
```

5. Write a python script to take two numbers from user (say x and y), now calculate xy and display the result.

```python
print(f"XY: {int(input("X: ")) * int(input("Y: "))}")
```

## Assignment-10: Operators

### Note

> | No. | Operator Name      | Symbol   | Example        |
> | --- | ------------------ | -------- | -------------- |
> | 0   | Addition           | +        | a + b          |
> | 1   | Concatenation      | +        | "a" + "b"      |
> | 2   | Containment        | in       | a in obj       |
> | 3   | Division (True)    | /        | a / b          |
> | 4   | Division (Floor)   | //       | a // b         |
> | 5   | Bitwise AND        | &        | a & b          |
> | 6   | Bitwise XOR        | ^        | a ^ b          |
> | 7   | Exponentiation     | \*\*     | a \*\* b       |
> | 8   | Bitwise NOT        | ~        | ~a             |
> | 9   | Bitwise OR         | \|       | a \| b         |
> | 10  | Identity           | is       | a is b         |
> | 12  | Identity (Not)     | is not   | a is not b     |
> | 12  | Indexed Assignment | =        | obj[i] = a     |
> | 13  | Indexed Assignment | =        | obj[i] = a     |
> | 14  | Indexing           | []       | a[0]           |
> | 15  | Left Shift         | <<       | a << b         |
> | 16  | Logical AND        | and      | a and b        |
> | 17  | Logical OR         | or       | a or b         |
> | 18  | Modulo             | %        | a % b          |
> | 19  | Multiplication     | \*       | a \* b         |
> | 20  | Negation           | -        | -a             |
> | 21  | Logical NOT        | not      | not a          |
> | 22  | Positive           | +        | +a             |
> | 23  | Right Shift        | >>       | a >> b         |
> | 24  | Slice Assignment   | [::] = v | a[i:j] = value |
> | 25  | Slice Deletion     | del [::] | del a[i::j]    |
> | 26  | Slicing            | [::]     | a[i::j]        |
> | 27  | String Formatting  | %        | "Hi %s" % name |
> | 28  | Subtraction        | -        | a - b          |
> | 29  | Less Than          | <        | a < b          |
> | 30  | Greater Than       | >        | a > b          |
> | 31  | Less Than Equal    | <=       | a <= b         |
> | 32  | Greater Than Equal | >=       | a >= b         |
> | 33  | Equality           | ==       | a == b         |
> | 34  | Not Equal          | !=       | a != b         |

> | Category   | Operators                                           | Use                     |
> | ---------- | --------------------------------------------------- | ----------------------- |
> | Arithmetic | `+  -  *  /  //  %  **`                             | Math operations         |
> | Relational | `>  <  >=  <=  ==  !=`                              | Comparison (True/False) |
> | Logical    | `and  or  not`                                      | Conditions combine      |
> | Bitwise    | `&  \|  ^  ~  >>  <<`                               | Binary operations       |
> | Assignment | `=  +=  -=  *=  /=  //=  %=  **= &= ^= \|= >>= <<=` | Assign/update value     |
> | Identity   | `is  is not`                                        | Memory comparison       |
> | Membership | `in  not in`                                        | Check element present   |

> **Arithemetic Operator**
>
> - **`/`:** Always return float value <br>
> - **`//`:** Always return float vlue, int type or float type
> - **`+`:** use for `int`, `float`, `complex`, `bool`
> - **`+`:** use for **concatenation**
> - **`+`:** invalid for `5 + "string"`
> - **`*`:** repeat for `"string" * 5`

> **Relataion Operators** <br>
>
> - **`<, >, <=, >=`: Inequality Operator**
> - **`==, !=`: Equality Operator** and can be used for two complex type values.
> - **Relation Operator:** Its can be used **compare two string** return `True` and `False`

> **Logical Operators** <br>
>
> - **Logical Operator** must be written in lowercase.
> - When **operands are non-bool** then result will also be **non-bool**

> **Indentity** (`is`, `is not`)<br>
>
> - **Chack References**

> **Membership Operator** (`in`, `not in`)<br>
>
> - Only for **Containers (Iterables)**
> - `int`, `float`, `complex`, `bool`, are not iterable and `str`, `range`, `list`, `tuple`, `set`, `dict`, are iterable.

1. Write a python script to remove the last digit from a given number. (for example, if user enters 2534 then your output should be 253)

```python
num = 1234
print(f"Orginal Number: {num} \nNew Number: {num//10}")
```

2. Write a python script to get the last digit from a given number. (for example, if user enters 2089 then your output should be 9)

```python
num = 1234
print(num%10)
```

3. Write a python script to swap data of two variables

```python
num1 = 10
num2 = 20
print(f"Num1: {num1}, Num2: {num2}")
num1, num2 = num2, num2
print(f"Num1: {num1}, Num2: {num2}")
```

4. Write a python script which takes a three digit number from the user and displays only its first digit.

```python
num = int(input("Enter three digits number: "))
print(f"First Digit: {num//100}")
```

5. Write a python script which takes a three digit number from the user and displays only its middle digit.

```python
num = int(input("Enter three digits number: "))
print(f"Middle Digit: {(num//10)%10}")
```

## Assignment-11: More on Operators

1. Write a python script to print True if the string 'my' is a member in a string entered by user.

```python
uStr = input("Enter String: ")
print("my" in uStr)
```

2. Write a python script to input two strings from the user and display whether the two variables referred to the same object or not. Print True or False.

```python
uStr1 = input("Enter 1st String: ")
uStr2 = input("Enter 2nd String: ")
print(uStr1 is uStr2)
```

> **Note:** When we store same values in any variable through user then each variable refer deffer reference.

3. What will be the output of the python expression 5>10<5 ? - `Flase`

4. What will be the output of the python expression "Red" and "White" ? - `White`

5. What will be the output of the python expression True or False ? - `True`

## Assignment-12: Decision Control

1. Write a python script to check whether a given number is positive or non-positive.

```python
num = int(input("Enter Number: "))
print(f"Result: { "Non-Positive" if num <= 0 else "Positive" }")
```

2. Write a python script to check whether a given number is divisible by 5 or not

```python
num = int(input("Enter Number: "))
print(f"{"Divisible by 5" if not (num % 5) else "Divisible by 5 not"}")
```

3. Write a python script to check whether a given number is even or odd.

```python
num = int(input("Enter Number: "))
print(f"Result: {"Even" if not (num%2) else "Odd" }")
```

4. Write a python script to print greater between two numbers. Print number only once even if the numbers are the same.

```python
num1 = int(input("Num1: "))
num2 = int(input("Num2: "))
print(f"Result: { num1 if num1 > num2 else num2 }")
```

5. Write a python script to print two given words in dictionary order

```python
uStr1 = input("uStr1: ")
uStr2 = input("uStr2: ")
print(f"{ "Dictionary Order" if uStr1.lower() < uStr2.lower() else "Not Dictionary"}")
```

## Assignment-13: More on Decision Control

1. Write a python script to check whether a given number is a three digit number or not.

```python
num = int(input("Enter Number: "))
print(f"{"Yes" if str(num).length() else "No"}")
```

2. Write a python script to check whether a given number is positive, negative or zero.

```python
num = int(input("Enter number: "))

if num > 0:
    print("Positive")
elif num < 0:
    print("Negative")
else:
    print("Zero")
```

3. Write a python script to check whether a given quadratic equation has two real & distinct roots, real & equal roots or imaginary roots

```python
a = int(input("Enter a: "))
b = int(input("Enter b: "))
c = int(input("Enter c: "))

d = b**2 - 4*a*c   # discriminant

if d > 0:
    print("Two real & distinct roots")
elif d == 0:
    print("Real & equal roots")
else:
    print("Imaginary roots")
```

> Concept <br>
> d = b² - 4ac <br>
> d > 0 → real & distinct <br>
> d = 0 → real & equal <br>
> d < 0 → imaginary

4. Write a python script to check whether a given year is a leap year or not.

```python
year = int(input("Enter Year: "))
if year%4 == 0 and year%100 != 0:
   print("Leap Year")
elif year%100 == 0 and year%400 == 0:
   print("Leap Year")
else:
   print("Not Leap Year")
```

5. Write a python script to print greater among three numbers. Print number only once even if the numbers are the same.

```python
num1 = int(input("Num1: "))
num2 = int(input("Num2: "))
num3 = int(input("Num3: "))

# 1st Way
if num1 > num2:
   if num1 > num3:
      print(num1)
   else:
      print(num3)
else:
   if num2 > num3:
      print(num2)
   else:
      print(num3)

# 2nd Way
if num1 >= num2 and num1 >= num3:
   print(num1)
elif num2 >= num1 and num2 >= num3:
   print(num2)
else:
   print(num3)

# 3rd Way
print(max(num1, num2, num3))
```

6. Password Strength Checker

```python
nums = "1234567890"
charsUpper = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
charsLower = "abcdefghijklmnopqrstuvwxyz"
charsSpecial = "~!@#$%^&*()_+"

isNums = False
isCharsUpper = False
isCharsLower = False
isCharsSpecial = False

password = input("Enter Password: ")

if len(password) >= 8 :
    if set(password) & set(nums):
        isNums = True
    if set(password) & set(charsUpper):
        isCharsUpper = True
    if set(password) & set(charsLower):
        isCharsLower = True
    if set(password) & set(charsSpecial):
        isCharsSpecial = True

if isNums and isCharsUpper and isCharsLower and isCharsSpecial:
    print(f"Password Strng: {password}")
else:
    print(f"Password Weak: {password}")
```

## Assignment-14: Match

1. Write a python script to check whether a given number is a three digit number or not.

```python
num = int(input("Num: "))
"""
if num < 0:
   num = -num
"""
abs(num)
if num >= 100 and num <= 999:
   print("Yes")
else:
   print("No")

```

2. Write a python script to check whether a given number is positive, negative or zero.

```python
num = int(input("Enter number: "))

if num > 0:
   print("Positive")
elif num < 0:
   print("Negative")
else:
   print("Zero")
```

3. Write a python script to make a menu driven program in which user has to choose one of the optionfrom four given options -
   1. Odd-Even,
   2. positive - Non Positive
   3. Simple Interest
   4. Find roots of quadratic equation. <br>
      Match and execute appropriate code on user selection

```python
operations = "1. Odd-Even\n2. Positive - Non Positive\n3. Simple Interest\n4. Find roots of quadratic\nEnter choice: "
operationNo = int(input(operations))

match operationNo:
    case 1:
        num = int(input("Enter number: "))
        if num % 2 == 0:
            print("Even")
        else:
            print("Odd")

    case 2:
        num = int(input("Enter number: "))
        if num > 0:
            print("Positive")
        else:
            print("Non-Positive")

    case 3:
        p = float(input("Principal: "))
        r = float(input("Rate: "))
        t = float(input("Time: "))
        si = (p * r * t) / 100
        print("Simple Interest =", si)

    case 4:
        a = float(input("Enter a: "))
        b = float(input("Enter b: "))
        c = float(input("Enter c: "))

        d = b**2 - 4*a*c   # discriminant

        if d > 0:
            root1 = (-b + d**0.5) / (2*a)
            root2 = (-b - d**0.5) / (2*a)
            print("Roots are real and different:", root1, root2)
        elif d == 0:
            root = -b / (2*a)
            print("Roots are real and equal:", root)
        else:
            print("Roots are imaginary")

    case _:
        print("Invalid Choice")
```

4. Write a python script to take one data from user and evaluate the type of data. If the data is of int type then print Monday, if the data is of float type then print Tuesday, if the data is of complex type then print Wednesday, if the data is of type bool then print Thursday.

```python
data = eval(input("Enter data: "))

if type(data) == int:
    print("Monday")
elif type(data) == float:
    print("Tuesday")
elif type(data) == complex:
    print("Wednesday")
elif type(data) == bool:
    print("Thursday")
```

5. Write a python script to take a string from the user. If the string is a part of "mystring" then print "One", if the string is a part of "education" then print "Two" and if the string is a part of "services" then print "Three".

```python
userStr = input("Enter String: ")

match True:
    case _ if userStr in "mystring":
        print("One")
    case _ if userStr in "education":
        print("Two")
    case _ if userStr in "services":
        print("Three")
    case _:
        print("Not Found")
```

## Assignment-15: while loop

1. Write a python script to print MySirG 5 times on the screen.

```python
i = 1
while i <= 5:
   print("MySirG")
   i+=1
```

2. Write a python script to print first 10 natural numbers.

```python
n = 1
while i <= 10:
   print(i)
   i+=1
```

3. Write a python script to print first 10 natural numbers in reverse order

```python
n = 10
while n > 0:
   print(n)
   n-=1
```

4. Write a python script to print first 10 odd natural numbers

```python
n = 1
while n <= 10:
   print( (n*2)-1 )
   n+=1
```

5. Write a python script to print first 10 odd natural numbers in reverse order

```python
n = 10
while n > 0:
   print((n*2) - 1)
   n-=1
```

## Assignment-16: more on while loop

1. Write a python script to print first 10 even natural numbers.

```python
n = 1
while n <= 10:
   print(n*2)
   n+=1
```

2. Write a python script to print first 10 even natural numbers in reverse order.

```python
n = 10
while n > 0:
   print(n *2)
   n-=1
```

3. Write a python script to print squares of first 10 natural numbers.

```python
n = 1
while n <= 10:
   print(n**2)
   n+=1
```

4. Write a python script to print cubes of first 10 natural numbers.

```python
n = 1
while n <= 10:
   print(n**3)
   n+=1
```

5. Write a python script to print first 10 multiples of 5

```python
n = 1
while n <= 10:
   print(n*5)
   n+=1
```

## Assignment-17: while loop with user input

1. Write a python script to print MySirG N times on the screen.

```python
n = int(input("n: "))
while n > 0:
   print("MySirG")
   n-=1
```

2. Write a python script to print first N natural numbers.

```python
n = int(input("n: "))
i = 1
while n > 0:
   print(i)
   n-=1
   i+=1
```

3. Write a python script to print first N natural numbers in reverse order.

```python
n = int(input("n: "))
while n > 0:
   print(n)
   n-=1
```

4. Write a python script to print first N odd natural numbers

```python
n = int(input("n: "))
i = 1
while n > 0:
   print(i*2-1)
   n-=1
   i+=1
```

5. Write a python script to print first N odd natural numbers in reverse order

```python
n = int(input("n: "))
while n > 0:
   print(n*2-1)
   n-=1
```

## Assignment-18: more on while loop with user input

1. Write a python script to print first N even natural numbers.

```python
n = int(input("n: "))
i = 1
while i <= n:
   print(i*2)
   i+=1
```

2. Write a python script to print first N even natural numbers in reverse order.

```python
n = int(input("n: "))
while n > 0:
   print(n*2)
   n-=1
```

3. Write a python script to print squares of first N natural numbers.

```python
n = int(input("n: "))
i = 1
while i <= n:
   print(i**2)
   i+=1
```

4. Write a python script to print cubes of first N natural numbers.

```python
n = int(input("n: "))
i = 1
while i <= n:
   print(i**3)
   i+=1
```

5. Write a python script to print first 10 multiples of N

```python
n = int(input("n: "))
i = 1
while i <= 10:
   print(n*i)
   i+=1
```

## Assignment-19: for loop

1. Write a python script to print each character of a string with its corresponding Unicode.

```python
userStr = input("Enter String: ")
for char in userStr:
   print(f"{char} : {ord(char)}")
```

2. Write a Python script to print only vowels of the given string

```python
userStr = input("Enter String: ")
for char in userStr:
   if char in "aeiouAEIOU":
    print(char)
```

3. Write a Python script to count occurrence of spaces in a given string.

```python
userStr = input("Enter String: ")
spaceCount = 0
for char in userStr:
   if char in " ":
      spaceCount+=1
print(f"Occurrence of Spaces: {spaceCount}")
```

4. Write a Python script to print unique digits of a given integer.

```python
# 1st Way
num = int(input("Num: "))
strNum = str(num)
for char in strNum:
   occurrence = 0
   for c in strNum:
      if char == c:
         occurrence+=1
      if occurrence == 2:
         break
   if occurrence == 1:
      print(char)

# 2nd Way
num = int(input("Num: "))
strNum = str(num)
for char in strNum:
   if strNum.count(char) == 1:
      print(char)
```

5. Write a Python script to count number of digits in a given number.

```python
num = int(input("Num: "))

# 1st
digitsCount = 0
if num == 0:
   digitsCount += 1
else:
   while num > 0:
   digitsCount+=1
   num//=10
print(digitsCount)

#2nd
print(len(str(num)))
```

## Assignment-20: for loop and range

**Note**

> | Type      | Definition (Kya hai)                      | Mutable? | Ordered? | Duplicate Allowed? | Example          | Loop Example                    |
> | --------- | ----------------------------------------- | -------- | -------- | ------------------ | ---------------- | ------------------------------- |
> | **range** | Numbers generate karta hai (start → end)  | ❌ No    | ✅ Yes   | ❌ No              | `range(1,5)`     | `for i in range(1,5): print(i)` |
> | **list**  | Collection of items (mixed types allowed) | ✅ Yes   | ✅ Yes   | ✅ Yes             | `[1, "Aman", 3]` | `for x in list: print(x)`       |
> | **tuple** | List jaisa but immutable                  | ❌ No    | ✅ Yes   | ✅ Yes             | `(1, 2, 3)`      | `for x in tuple: print(x)`      |
> | **str**   | Characters ka sequence                    | ❌ No    | ✅ Yes   | ✅ Yes             | `"Aman"`         | `for ch in "Aman": print(ch)`   |
> | **set**   | Unique items ka unordered collection      | ✅ Yes   | ❌ No    | ❌ No              | `{1,2,3}`        | `for x in set: print(x)`        |
> | **dict**  | Key-value pairs                           | ✅ Yes   | ✅ Yes\* | ❌ Keys unique     | `{"a":1,"b":2}`  | `for k in dict: print(k)`       |

**range**

> - range is a **class**
> - range is **immutable sequence**
> - range can contain only **int type values**
> - range contain sequence of **integer with common defference** (Arithmetic Prgression)
> - range elements are **indexed**

> - **How to create range object ?** <br>
>   `r = range( beg, end, step )`
>   - `beg` - inclusion
>   - `end` - exclusion
>   - `step` - common gap

> - **Other ways to create range object ?** <br>
>   - `r = range( end )`
>     - `beg` = 0
>     - `step` = 1
>   - `r = range( beg, end )`
>     - `beg` = 0

> - **Indexing** <br>
>   **-index** - `-5,-4,-3,-2,-1` <br>
>   **+index** - `0, 1, 2, 3, 4` <br>
>   **range** - `[1, 2, 3, 4, 5]`

1. Write a python script to print the first 10 multiples of 5.

```python
r = range(1, 11, 1)
for i in r:
    print(i*5)
```

2. Write a python script to print first 10 multiples of N.

```python
n = int(input("n: "))
r = range(1, 11, 1)
for i in r:
    print(i*n)
```

3. Write a python script to print first M multiples of N.

```python
n = int(input("n: "))
m = int(input("m: "))
r = range(1, m+1, 1)
for i in r:
    print(i*n)
```

4. Write a python script to print the first 10 multiples of N in reverse order.

```python
n = int(input("n: "))
r = range(10, 0, -1)
for i in r:
    print(i*n)
```

5. Write a python script to print table of user's choice

```python
n = int(input("n: "))
r = range(1, 11)
for i in r:
    print(i*n)
```

## Assignment-21: more on for loop and range

1. Write a python script to print first N even natural numbers.

```python
n = int(input("N: "))
r = range(1, n+1)
for i in r:
    print(i*2)
```

2. Write a python script to print first N odd natural numbers.

```python
n = int(input("N: "))
r = range(1, n+1)
for i in r:
    print(i*2-1)
```

3. Write a python script to print squares of first N natural numbers.

```python
n = int(input("N: "))
r = range(1, n+1)
for i in r:
    print(i**2)
```

4. Write a python script to print cubes of first N natural numbers.

```python
n = int(input("N: "))
r = range(1, n+1)
for i in r:
    print(i**3)
```

5. Write a python script to display all prime numbers within a range. (range start = 15 end = 45)

```python
r = range(15, 45+1)
for i in r:
    for n in range(2, i+1):
        if not(i%n):
            break
    if n == i:
        print(n)
```

## Assignment-22: Loops

1. Write a Python script to calculate sum of first n natural numbers.

```python
n = int(input("n: "))
r = range(1, n+1)
sum = 0
for i in r:
    sum+=i
print(f"Sum: {sum}")
```

2. Write a Python script to calculate sum of squares of first N natural numbers.

```python
n = int(input("n: "))
r = range(1, n+1)
sum = 0
for i in r:
    sum+=i**2
print(f"Sum: {sum}")
```

3. Write a Python script to calculate sum of cubes of first N natural numbers

```python
n = int(input("n: "))
r = range(1, n+1)
sum = 0
for i in r:
    sum+=i**3
print(f"Sum: {sum}")
```

4. Write a Python script to calculate sum of first N odd natural numbers.

```python
n = int(input("n: "))
r = range(1, n+1)
sum = 0
for i in r:
    sum = sum + ((i*2)-1)
print(f"Sum: {sum}")
```

5. Write a Python script to calculate sum of first n even natural numbers.

```python
n = int(input("n: "))
r = range(1, n+1)
sum = 0
for i in r:
    sum = sum + (i*2)
print(f"Sum: {sum}")
```

## Assignment-23: Loops again

1. Write a Python script to calculate factorial of a given number.

```python
n = int(input("n: "))
for i in range(1, n):
    if not(n%i):
        print(i)
```

2. Write a Python script to count digits in a given number.

```python
num = input("Enter Number: ")

count = 0

for i in range(len(num)):
    count += 1

print("Total digits:", count)
```

3. Write a Python script to calculate sum of digits of a given number.

```python
str_num = str(num)
list_str_num = list(str_num)
sum = 0
for n in list_str_num:
    sum = sum + int(n)
print(sum)
```

4. Write a Python script to print binary equivalent of a given decimal number. (Do not use bin() method)

```python
num = int(input("Num: "))
binNum = ""
if num ==0:
    binNum = "0"
else:
    while num > 0:
        binNum = str(num%2) + binNum
        num = num//2
print(binNum)
```

5. Write a Python script to print the octal equivalent of a given decimal number. (Do not use oct()method)

```python
num = int(input("Num: "))
binNum = ""
if num ==0:
    binNum = "0"
else:
    while num > 0:
        binNum = str(num%8) + binNum
        num = num//8
print(binNum)
```

### 🐍 Python Built-in Functions

## Assignment-24: list

### Note - Part 1

> - list is **class**.
> - list is an **iterable sequence**.
> - list is **mutable**.
> - list is **growable**.
> - list can store **heterogeneous data**.
> - list element are **indexed**.

> - **How to create list object ?**
>   - `l1 = [10, 20, 30]` → Square brackets are used to denote a list.
>   - `l2 = []` → empty list object.
>   - `l2 = [50, 3.2, "abc"]` → Heterogeneous element

> - **How to access list object ?**
>   - `l1 = [30, 20, 80, 10, 60, 40]`
>   - `print( l1 )` → [ 30, 20, 80, 10, 60, 40 ]
>   - `print( l1[0] )` → 30
>   - `print( l1[1], l1[2] )` → 20, 80

> - **How to delete an element from list object ?**
>   - `l1 = [30, 20, 80, 10, 60, 40]`
>   - `del l1[2]` → [ 30, 20, 10, 60, 40 ]

> - **How to edite an element of list object ?**
>   - `l1 = [30, 20, 80, 10, 60, 40]`
>   - `l1[2] = 42` → [ 30, 20, 42, 10, 60, 40 ]

> - **How to add more elements in list object ?**
>   - `l1 = [30, 20, 80, 10, 60, 40]`
>   - `l1[6] = 70` → **_index error_**
>   - `listObject [ invalidIndex ]` is an **ERROR**

> - **There are two standard ways to add elemets in the list.**
>   1. `append( value )` → `listObj.append(5)`
>   1. `insert( index, value )` → `listObj.append(2, 5)`
>      - if `index` > `last_index` then value will start at `last_index + 1`

### Note - Part 2

> - **Packing and Unpacking** <br>
>   `l1 = [20, 60, 80]`<br>
>   `num1, num2, num3 = l1` → **_unpacking_**
>
>   **note**: number of variable in the left hand side **_must be same_** as the number of elements in the list.
>
>   `num1 = 2` <br>
>   `num2 = 6` <br>
>   `num3 = 10` <br>
>   `l2 = [num1, num2, num3]` → **_packing_**

> - **list() method** <br>
>   <br>`l1 = list()`
>   <br>`l1 = list(10)` **_→ ERROR_** `list()` method can take at most one argument and argument should must be `iterable`
>   <br>`l1 = list(10, 20, 30)`
>   <br>`l1 = list("MySirG")`
>   <br>`l1 = list(range(6))`
>   <br>`l1 = list([10, 20])`

> - **Comparison Operator on list**
>   <br>`l1 = [1, 2, 3]`
>   <br>`l2 = [2, 3, 1]`
>   <br>`l3 = [1, 2, 3, 4, 5]`
>   <br>`l4 = [1, 2, 3]`
>   <br>`l1 == l2` → **_Flase_**
>   <br>`l1 == l3` → **_Flase_**
>   <br>`l1 == l4` → **_True_**
>   <br>`l1 > l2` → **_True_**

> - **Concatenation Operator**
>   <br>`l1 = [1, 2, 3]`
>   <br>`l2 = [2, 3, 1]`
>   <br>`l3 = l1 + l2` → **_[1, 2, 3, 2, 3, 1]_**
>   <br>`l1 += l2` → `l1 = l1 + l2` → **_[1, 2, 3, 2, 3, 1]_**

> - **Repeatation Operator**
>   <br>`l1 = [1, 2]`
>   <br>`l1 * 4` → **_[1, 2, 1, 2, 1, 2, 1, 2]_**

> - **Slicing Operator**
>   **Syntax:** `listObj[ brg : end : step]` <br>
>   `l1 = [20, 40, 10, 30, 60, 50]`
>   By Default
>   - beg = `0`
>   - end = `extreme emd`
>   - step = `1`

### Note - Part 3

> - **list of list** <br>
>   `l1 = [ [1,3,6], [2, 1, 8], [6, 4, 4] ]`
>   - `li[0]` = **[1, 3, 6]**
>   - `li[1]` = **[2, 1, 8]**
>   - `li[2]` = **[6, 4, 4]**
>   - `li[0][0]` = **1**
>   - `li[0][1]` = **3**
>   - `li[0][2]` = **6**

- **list methods**
  | Method | Definition | Example | Output |
  | --------- | ------------------------------------------------------------------------------------------------------- | -------------------------- | ----------- |
  | append() | Adds an element at the end of the list. | `l=[1,2]; l.append(3)` | `[1,2,3]` |
  | extend() | Adds all elements of an iterable to the list. | `l=[1,2]; l.extend([3,4])` | `[1,2,3,4]` |
  | insert() | Inserts an element at a specified position in the list. | `l=[1,2]; l.insert(1,99)` | `[1,99,2]` |
  | remove() | Removes the first occurrence of the specified element. It gives an error if the element is not present. | `l=[1,2,2]; l.remove(2)` | `[1,2]` |
  | pop() | Removes and returns the element at the specified index. If index is not given, removes last element. | `l=[1,2,3]; l.pop()` | `3` |
  | clear() | Removes all elements from the list. | `l=[1,2]; l.clear()` | `[]` |
  | index() | Returns the index of the first occurrence of the specified element. It gives an error if not found. | `l=[10,20]; l.index(20)` | `1` |
  | count() | Returns the number of times the specified element appears in the list. | `l=[1,2,2]; l.count(2)` | `2` |
  | sort() | Sorts the list in ascending order by default. | `l=[3,1,2]; l.sort()` | `[1,2,3]` |
  | reverse() | Reverses the order of the elements in the list. | `l=[1,2,3]; l.reverse()` | `[3,2,1]` |
  | copy() | Returns a shallow copy of the list. | `l1=[1,2]; l2=l1.copy()` | `[1,2]` |

- **list comprehension**
  - A concise way to create a list in a single line using a loop, with an optional condition.
  - **Syntax:** **[ `expression` `for variable in iterable` ]**
    - `[5 for i in range(4)]` → **_[ 5, 5 ,5, 5 ]_**
    - `[i**2 for i in range(4)]` → **_[ 0, 1 ,4, 9 ]_**

- **user input**
  > - `l = list(input())`

> - **Mutability and Hashability**
>   <br>👉 **Mutability** →
>   The ability of an object to be changed or modified after its creation.
>   <br>👉 **Immutable Objects** →
>   Objects whose values cannot be changed after creation are called immutable objects.
>   <br>👉 **Hashability** →
>   Hashability is a property of an object that allows it to have a fixed hash value which does not change during its lifetime.
>   <br>👉 **Hashable Objects** →
>   Objects that have a constant hash value and can be used as keys in dictionaries or elements in sets are called hashable objects.

| ababa     | Hashable | Mutable |
| --------- | -------- | ------- |
| `int`     | Yes      | No      |
| `float`   | Yes      | No      |
| `complex` | Yes      | No      |
| `bool`    | Yes      | No      |
| `str`     | Yes      | No      |
| `range`   | Yes      | No      |
| `list`    | No       | Yes     |
| `tuple`   | Yes      | No      |
| `set`     | No       | Yes     |
| `dict`    | No       | Yes     |

1. Write a python script to calculate sum of elements of a list.

```python
l1 = [1,2,3,4,5]

# 1st Way
result = 0
for e in l1:
   result+=e
print(result)

#2nd Way
print(sum(l1))
```

2. Write a Python script to calculate average of elements of a list.

```python
l1 = [1,2,3,4,5]
result = 0

#1st way
for e in l1:
   result += e
print(f"Result: {result}")

#2nd way
result = sum(l1)
print(f"Result: {result}")
```

3. Write a Python script to create a list of squares of numbers of a given list.

```python
nums = [1,2,3,4,5]
squares = []
for num in nums:
    squares.append(num**2)
print(squares)
```

4. Write a Python script to sort list elements in descending order.

```python
nums_str = input("Numbers: ").split(",")
nums = [int(num) for num in nums_str]
length = len(nums)


# 1st way
for i in range(0, length):
    for j in range(i+1, length):
        if nums[i] < nums[j]:
            nums[i],nums[j] = nums[j],nums[i]


# 2st way
nums.sort()
nums = nums[::-1]
print(nums.sort())

print(f"Nums: {nums}")
```

5. Write a Python script to create a list from a given list by selecting only even places elements.

```python
nums = [1,2,3,4,5,6,7,8,9,10]
nums_even = []
nums_odd = []

for num in nums:
    if num%2:
        nums_odd.append(num)
    else:
        nums_even.append(num)

print(f"Nums: {nums}")
print(f"Even Nums: {nums_even}")
print(f"Odd Nums: {nums_odd}")
```

## Assignment-25: more on list

1. Write a python script to create a list of first N even natural numbers.

```python
n = int(input("n: "))
even_nums = [num*2 for num in range(1, n+1)]
print(even_nums)
```

2. Write a Python script to create a list of first N terms of a Fibonacci series.

```python
n = int(input("n: "))

fibonacci_nums = []
fibo_num = 0
prev_num = 1

while len(fibonacci_nums) != n:
    fibonacci_nums.append(fibo_num)
    fibo_num = prev_num + fibo_num
    prev_num = fibo_num - prev_num

print(fibonacci_nums)
```

3. Write a Python script to create a list of first N prime numbers.

```python
n = int(input("n: "))

if n < 0:
    n = -n
if n == 0:
    n = 5

prime_num = 1
prime_nums = []


while len(prime_nums) < n:
    for num in range(2, prime_num+1):
        if prime_num % num == 0:
            if (num == prime_num):
                prime_nums.append(num)
            break

    prime_num+=1

print(prime_nums)
```

4. Write a Python script to add two matrices each of order 3 x 3. Store matrix elements in a list of lists.

```python
matrix_one = [[1,2,3],[1,2,3],[1,2,3]]
matrix_two = [[1,1,1],[2,2,2],[3,3,3]]
matrix_ans = []

for row in range(0,3):
   m_row = []
   for column in range(0,3):
      m_row.append(matrix_one[row][column] + matrix_two[row][column])
   matrix_ans.append(m_row)

print(matrix_ans)
```

5. Write a Python script to create two lists from a given list of numbers in such a way that the first list can have only positive numbers and second list can have only non positive numbers.

```python
nums = [12, -23, 171, 0, 2929, -1, 282, -78, -4]
positive_nums = []
negative_nums = []

for num in nums:
   if (num > 0):
      positive_nums.append(num)
   else:
      negative_nums.append(num)

print(f"Nums: {nums}")
print(f"Positive Nums: {positive_nums}")
print(f"Negative Nums: {negative_nums}")
```

## Assignment-26: str

### **Part - 1**

> - str is a class
> - str is immutable
> - str is iterable
> - str is hashable
> - str is a sequence

> - **How to create str object ?** <br>
>   `s1 = "MySirG"` <br>
>   `s2 = 'MySirG'` <br>
>   `s3 = """MySirG"""` <br>
>   `s4 = '''MySirG'''` <br>
>   `s5 = str()` <br>
>   `s6 = str(123)` <br>
>   `s7 = str(3.46)`

> - **Indexing** <br>
>   `s1 = "MySirG"` <br>
>   `s1[0]` → M <br>
>   `s1[-1]` → g <br>
>   `s1[2]` → S

> - **Accessing `str` element** <br>
>   `s1[index]` <br>
>   `print` <br>
>   `for loop` <br>
>   `slicing operator` <br>
>   `while loop` <br>
>   `print( s1[0], s2[1], s3[2] )`

> - **built in method** <br>
>   `len()` <br>
>   `min()` <br>
>   `max()` <br>
>   `sum()` → Not Sum **(only integer)**<br>
>   `sorted()` → It sorts string but **return list of sorted string** <br> - **those perform work on the basic of unicode**

> - **concatenation and repetition operation** <br>
>   `s1 = "ABC"` <br>
>   `s2 = "DE"` <br>
>   `s1 + s2` → **_ABCDE_** <br>
>   `s1 * 3` → **_DEDEDE_**

> - **comparrison operator** <br>
>   `s1 > s2` → time if is `s1` comes after `s2` in dictionary order.

**1. Case Conversion Methods**

| Method         | Definition                                                              | Advanced Example                           | Output             |
| -------------- | ----------------------------------------------------------------------- | ------------------------------------------ | ------------------ |
| `lower()`      | Returns a new string with all characters converted to lowercase.        | `python email = "USER@GMAIL.COM".lower() ` | `'user@gmail.com'` |
| `upper()`      | Returns a new string with all characters converted to uppercase.        | `python code = "error".upper() `           | `'ERROR'`          |
| `title()`      | Returns a string where first letter of each word is capitalized.        | `python name = "aman kumar".title() `      | `'Aman Kumar'`     |
| `capitalize()` | Returns a string with first character capitalized and rest lowercase.   | `python msg = "hello WORLD".capitalize() ` | `'Hello world'`    |
| `swapcase()`   | Returns a string with uppercase converted to lowercase and vice versa.  | `python text = "PyThOn Dev".swapcase() `   | `'pYtHoN dEV'`     |
| `casefold()`   | Returns a lowercase string for aggressive comparison (used in Unicode). | `python print("ß".casefold()) `            | `'ss'`             |

**2. Searching Methods**

| Method         | Definition                                                   | Advanced Example                                            | Output |
| -------------- | ------------------------------------------------------------ | ----------------------------------------------------------- | ------ |
| `find()`       | Returns the index of first occurrence of substring, else -1. | `python text = "order_id_123"; text.find("id") `            | `6`    |
| `index()`      | Returns index of substring but raises error if not found.    | `python text = "order_id_123"; text.index("id") `           | `6`    |
| `count()`      | Returns total number of occurrences of substring.            | `python logs = "error error success"; logs.count("error") ` | `2`    |
| `startswith()` | Returns True if string starts with given prefix.             | `python url = "https://site.com"; url.startswith("https") ` | `True` |
| `endswith()`   | Returns True if string ends with given suffix.               | `python file = "data.csv"; file.endswith(".csv") `          | `True` |

**3. Validation Methods**

| Method      | Definition                                       | Advanced Example                              | Output |
| ----------- | ------------------------------------------------ | --------------------------------------------- | ------ |
| `isalpha()` | Returns True if all characters are alphabets.    | `python name = "Aman"; name.isalpha() `       | `True` |
| `isdigit()` | Returns True if all characters are digits.       | `python otp = "456789"; otp.isdigit() `       | `True` |
| `isalnum()` | Returns True if all characters are alphanumeric. | `python user = "aman123"; user.isalnum() `    | `True` |
| `isspace()` | Returns True if string contains only whitespace. | `python s = "   "; s.isspace() `              | `True` |
| `islower()` | Returns True if all characters are lowercase.    | `python text = "hello"; text.islower() `      | `True` |
| `isupper()` | Returns True if all characters are uppercase.    | `python text = "HELLO"; text.isupper() `      | `True` |
| `istitle()` | Returns True if string is in title case.         | `python text = "Aman Kumar"; text.istitle() ` | `True` |

**4. Modification Methods**

| Method           | Definition                                                          | Advanced Example                                                 | Output         |
| ---------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------- | -------------- |
| `replace()`      | Returns a string where occurrences are replaced with new substring. | `python msg = "Hello user"; msg.replace("user", "Aman") `        | `'Hello Aman'` |
| `strip()`        | Returns string with leading and trailing spaces removed.            | `python data = "  aman  ".strip() `                              | `'aman'`       |
| `lstrip()`       | Returns string with leading spaces removed.                         | `python data = "   aman".lstrip() `                              | `'aman'`       |
| `rstrip()`       | Returns string with trailing spaces removed.                        | `python data = "aman   ".rstrip() `                              | `'aman'`       |
| `removeprefix()` | Returns string after removing given prefix.                         | `python url = "https://site.com"; url.removeprefix("https://") ` | `'site.com'`   |
| `removesuffix()` | Returns string after removing given suffix.                         | `python file = "data.csv"; file.removesuffix(".csv") `           | `'data'`       |

**5. Splitting & Joining**
| Method | Definition | Advanced Example | Output |
| -------------- | --------------------------------------------------- | --------------------------------------------------- | ------------------------ |
| `split()` | Returns list by splitting string using separator. | `python data = "name,email,age".split(",") ` | `['name','email','age']` |
| `rsplit()` | Returns split from right side. | `python text = "a-b-c"; text.rsplit("-",1) ` | `['a-b','c']` |
| `splitlines()` | Returns list of lines from multiline string. | `python text = "hi\nhello"; text.splitlines() ` | `['hi','hello']` |
| `join()` | Returns string formed by joining iterable elements. | `python words = ["Aman","Kumar"]; " ".join(words) ` | `'Aman Kumar'` |

**6. Alignment Methods**
| Method | Definition | Advanced Example | Output |
| ---------- | ------------------------------------------- | -------------------------------------- | -------------- |
| `center()` | Returns centered string with padding. | `python name = "Aman".center(10,"-") ` | `'---Aman---'` |
| `ljust()` | Returns left-aligned string with padding. | `python name = "Aman".ljust(10,"-") ` | `'Aman------'` |
| `rjust()` | Returns right-aligned string with padding. | `python name = "Aman".rjust(10,"-") ` | `'------Aman'` |
| `zfill()` | Returns string padded with zeros from left. | `python num = "42".zfill(5) ` | `'00042'` |

**7. Advanced Methods**
| Method | Definition | Advanced Example | Output |
| -------------- | ----------------------------------------------------- | ------------------------------------------------- | --------------------- |
| `partition()` | Returns tuple split at first occurrence of separator. | `python text = "key=value"; text.partition("=") ` | `('key','=','value')` |
| `rpartition()` | Returns tuple split from right side. | `python text = "a=b=c"; text.rpartition("=") ` | `('a=b','=','c')` |
| `format()` | Returns formatted string by inserting values. | `python msg = "Hello {}".format("Aman") ` | `'Hello Aman'` |
| `encode()` | Returns encoded byte version of string. | `python text = "Aman".encode("utf-8") ` | `b'Aman'` |
| `expandtabs()` | Returns string with tabs replaced by spaces. | `python text = "A\tB".expandtabs(4) ` | `'A   B'` |

**⭐ BONUS: MOST IMPORTANT METHODS\***
| Category | Methods |
| ---------- | ------------------------------- |
| Case | lower, upper, title, capitalize |
| Search | find, index, count |
| Validation | isalpha, isdigit, isalnum |
| Modify | replace, strip |
| Split/Join | split, join |
| Check | startswith, endswith |
| Format | format, partition |

1. Write a python script to check if a given string has only alphabets in it.

```python
sentence = input("Sentence: ")
print("Yes" if sentence.isalpha() else "No")
```

2. Write a python script to check if a given character is present in a given string or not.

```python
sentence = input("Sentence: ")
character = input("Character: ")
print("Yes" if character in sentence else "No")
```

3. Write a python script to count vowels in a given string.

```python
sentence = input("Sentence: ")
vowels_count = 0
for letter in sentence:
   if letter in "aeiouAEIOU":
      vowels_count+=1
print(f"vowels count: {vowels_count}")
```

4. Write a python script to count words in a given string

```python
sentence = input("Sentence: ")
print(f"Words count: {len(sentence.split(" "))}")
```

5. Write a python script to reverse a string

```python
sentence = input("Sentence: ")
reverse_sentence = ""
for letter in sentence:
   reverse_sentence = letter + reverse_sentence
print(f"Sentence: {sentence}")
print(f"Reverse Sentence: {reverse_sentence}")
```

## Assignment-27: more on str

1. Write a python script to reverse a string word wise (for example- "mysirg education services" is a given string and resulting string should be "services education Mysirg")

```python
sentence = input("Sentence: ")
aman = " ".join(list(reversed(sentence.split(" "))))
print(aman)
```

2. Write a python script to extract numbers from a given text and store all the numbers in a list.

```python
text = input("Text: ")
nums = []

for letter in text:
    if letter in "12345678900":
        nums.append(int(letter))

print(f"Numbers: {nums}")
```

3. Write a python script to check whether it is a palindrome or not.

```python
word = input("Word: ")

#1st Way
reversed_word = "".join(list(reversed(list(word))))
if word == reversed_word:
    print("Palindrome")
else:
    print("Not Palindrome")

#2nd Way

reversed_word = ""
for letter in word:
    reversed_word = letter + reversed_word
if word == reversed_word:
    print("Palindrome")
else:
    print("Not Palindrome")
```

4. Write a python script to transform a given string to uppercase.

```python
sentence = input("sentence: ")

#1st Way
upper_sentence = ""
for letter in sentence:
    print(letter)
    if ord(letter) >= 97:
        upper_sentence = upper_sentence + chr(ord(letter)-32)
    else:
        upper_sentence = upper_sentence + letter

print(upper_sentence)

#1st Way
upper_sentence = sentence.upper()
print(upper_sentence)
```

5. Write a python script to find maximum length word in a given text.

```python
sentence = input("sentence: ")

long_word = ""

for word in sentence.split(" "):
    print(f"{word} : {len(word)}")
    if len(word) > len(long_word):
        long_word = word

print(f"Long Word: {long_word}")
```

## Assignment-28: list and str mixed

1. Write a python script to remove all non int values from a list

```python
string = input("string: ")
alpha_string = ""

for ch in string:
    if not (ch in "1234567890"):
        alpha_string = alpha_string + ch

print(alpha_string)
```

2. Write a python script to print distinct elements along with their frequencies of occurrences in the list.

```python
sentence = "aman_kumar_singh_chandravanshi"
unique_element = []
count_element = []

for i in range(len(sentence)):
    if not (sentence[i] in sentence[0:i]):

        element_count = 0

        for ch in sentence:
            if ch == sentence[i]:
                element_count += 1

        unique_element.append(sentence[i])
        count_element.append(element_count)

for i in range(len(unique_element)):
    print(f"{unique_element[i]} : {count_element[i]}")
```

3. Write a python script to sort a list of strings

```python
sentence = input("Sentence: ").split(" ")
sorted_sentence = []

print(sentence)

for i in range(0, len(sentence)):
    for j in range(i+1, len(sentence)):
        if sentence[i].upper() > sentence[j].upper():
            sentence[i], sentence[j] = sentence[j], sentence[i]

print(sentence)
```

4. Write a python script to find first repeated string in a list of strings

```python
sentence = input("Sentence: ").split(" ")

for i in range(0, len(sentence)):
    if sentence[i] in sentence[i+1: len(sentence)]:
        print(sentence[i])
        break
```

5. Write a python script to count strings which ends at character 's' in a list of strings.

```python
sentence = input("Sentence: ").split(" ")
word_count = 0

for word in sentence:
    if word.endswith("s"):
        word_count += 1

print(word_count)
```

## Assignment-29: tuple

> - tuple is class
> - tuple is iterable
> - tuple is immutable
> - tuple is hashable
> - tuple is sequence
> - tuple can contain values of different types

> - **Sequence:** Thats can be applied loop and slicing. <br>
>   **tuple** = immutable <br>
>   **list** = mutable

> - How to create tuple objects ? <br>
>   `t1 = (1,2,3,4,5)` <br>
>   `t2 = ()` <br>
>   `t3 = (10)` → **_tuple (not)_** <br>
>   `t4 = (10,)` <br>
>   `t5 = 10, 20, 30`

> - Indexing <br>
>   `t1 = (1,2,3,4,5)` → [ 0, 1, 2, 3, 4 ] <br>

> - Accessing tuple elements <br>
>   1. `indexing` <br>
>   2. `while loop` <br>
>   3. `do while` <br>

> - Concatenation and Repetition Operator <br>
>   `t1 = (10, 20)` <br>
>   `t2 = (1, 2)` <br>
>   `t1 + t2` → **_(10, 20, 1, 2)_** <br>
>   `t1 * 5` → **_(10, 20, 10, 20, 10, 20, 10, 20, 10, 20,)_**

> - Comparision Operator <br>
>   `t1 = (10, 20)` <br>
>   `t2 = (11, 12)` <br>
>   `t1 > t2` → **_False_** <br>
>   `t1 == t2` → **_False_** <br>
>   `t2 > t1` → **_True_**

> - nasted tuple
>   `t1 = ( "sentence1", (10, 20), "sentence2" )`

> - tuple object methods <br>
>   1. `index()`
>   2. `count()`

> - slicing operator <br>
>   `t1 [beg: end: step]`
>   `t1 [::-1]` → **_REVERSE_**

> - user input <br>
>   `t1 = tuple([int(e) for e in input().split(",")])` <br>
>   `t1 = tuple()` <br>
>   `t2 = tuple([1,2,3])` <br>
>   `t3 = tuple(range(6))` <br>

1. Write a python script to create a tuple from a given list.

```python
t1 = tuple([int(num) for num in input("Nums: ").split(" ")])
print(t1)
```

2. Write a python script to reverse a tuple.

```python
nums = (1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15)
reversed_nums = nums[::-1]
print(reversed_nums)
```

3. Write a python script to create a list of tuples from a given list of strings, where each tuple is a collection of strings begin with the same character.

```python
que = "Write a python script to create a list of tuples from a given list of strings, where each tuple is a collection of strings begin with the same character."

words = que.split(" ")

words_same = []
tuples_list = []
unique_letters = ""

for word in words:
    if not (word[0].upper() in unique_letters.upper()):
        unique_letters += word[0]

for letter in unique_letters:
    for word in words:
        if word.startswith(letter):
            words_same.append(word)
    tuples_list.append(tuple(words_same))
    words_same = []

print(tuples_list)
```

4. Write a python script to create a list of tuples, where each tuple is a pair of elements, first element is uppercase character and second element is its unicode.

```python
sentence = input("Sentence: ")
list_of_tuples = []

for letter in sentence:
    list_of_tuples.append((letter.upper(), ord(letter.upper())))

print(list_of_tuples)
```

5. Write a python script to find the sum of all odd numbers stored in a tuple.

```python
nums = (1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15)
odd_sum = 0
for num in nums:
    if not (num % 2):
        odd_sum += num
print(odd_sum)
```

## Assignment-30: set

1. Write a python script to print all distinct element of a list. Use set to solve the problem.
2. Create two sets from a given set of numbers to separate even and odd numbers.
3. Given a set of five player names. Write a Python script to form all possible pairs of players that is
   selecting two players at a time.
4. You have a list of names of candidates, some of them are wearing black hat, some of them are
   wearing red shoes and some of them are wearing both. Now you have given a list of names of
   candidates wearing black hat. There is another list of names of candidates wearing red shoes. Write
   a python script to find out the names of the candidates wearing black hat and red shoes.
5. Write a python script to create a set of tuples, where each tuple has two elements representing dice
   upper face number. Take a number N from the user and generate all possible tuples, in such a way
   that tuple elements sums to N.

## Assignment-31: dict

1. Create a dict object where first N natural numbers are keys and their squares are data values.
2. Sort a dictionary by its keys in descending order.
3. Write a python script to create a dictionary where key values are cricket player names and data
   values are tuple of 4 elements - matches played, total runs, half centuries and centuries. All data
   should be taken from user.
4. Write a python script to find maximum size batch code from a dictionary where key-values in the
   dictionary are batch codes and data-values are size of the batch.
5. Write a python script to create a dict object from a list of city names in such a way the alphabets are
   keys of the dictionary and list of city names starting from that alphabet will be its data value.

## Assignment-32: Functions-1

1. Write a Python function to calculate sum of two numbers. (TSRS)
2. Write a Python function to calculate area of a circle(TSRS)
3. Write a Python function to calculate average of three numbers. (TSRS)
4. Write a Python function to calculate compound interest. (TSRS)
5. Write a Python function to calculate volume of a cuboid. (TSRS)

## Assignment-33: Functions-2

1. Write a Python function to check if a number is even. (TSRS)
2. Write a Python function to find greater among three numbers(TSRS)
3. Write a Python function to check whether a number is Prime (TSRS)
4. Write a Python function to check if an year is leap year (TSRS)
5. Write a Python function to calculate factorial of a number (TSRS)

## Assignment-34: Functions-3

1. Write a Python function to print first N odd natural numbers. (TSRN)
2. Write a Python function to print first N Prime numbers (TSRN)
3. Write a Python function to print all prime numbers between two given numbers (TSRN)
4. Write a Python function to print first N terms of Fibonacci series (TSRN)
5. Write a Python function to print all factors of a given number (TSRN)

## Assignment-35: Functions-4

1. Write a Python function to calculate LCM of two number. (TSRS)
2. Write a Python function to count words in a string (TSRS)
3. Write a Python function to create a list of Prime numbers between two given numbers (TSRS)
4. Write a Python function to filter out words from a text starting from same alphabet and store them
   in a list. Now create a dict with alphabets as key-values and list of words starting from that alphabet
   as data values. Take text as an argument and return dict object (TSRS)
5. Write a Python function to find all the common factors of two given numbers. Return a tuple of
   such factors (TSRS)

## Assignment-36: Functions-5

1. Write a Python function to remove duplicate elements from a given list. (TSRS)
2. Write a Python function to count frequency of each element of the list and store list elements in the
   dict object as keys and element frequency as data values (TSRS)
3. Write a Python function to find numbers in a given text, store numbers in a list and return list.
   (TSRS)
4. Write a Python function to find largest sorted subsequence in a given list. Return the largest
   subsequence as a list. (TSRS)
5. Write a Python function to check if two given list have same elements in any order or not. Return
   True or False. (TSRS)

## Assignment-37: Recursion-1

1. Write a recursive function to print first N natural numbers
2. Write a recursive function to print first N natural numbers in reverse order
3. Write a recursive function to print first N odd natural numbers
4. Write a recursive function to print first N odd natural numbers in reverse order.
5. Write a recursive function to print MySirG N times on the screen.

## Assignment-38: Recursion-2

1. Write a recursive function to print first N even natural numbers
2. Write a recursive function to print first N even natural numbers in reverse order
3. Write a recursive function to print squares of first N natural numbers
4. Write a recursive function to print cubes of first N natural numbers.
5. Write a recursive function to print reverse of a given number.

## Assignment-39: Recursion-3

1. Write a recursive function to calculate sum of first N natural numbers.
2. Write a recursive function to calculate sum of first N odd natural numbers.
3. Write a recursive function to calculate sum of first N even natural numbers.
4. Write a recursive function to calculate sum of squares of first N natural numbers.
5. Write a recursive function to calculate sum of cubes of first N natural numbers.

## Assignment-40: Recursion-4

1. Write a recursive function to calculate sum of digits of a given number.
2. Write a recursive function to calculate factorial of a given number.
3. Write a recursive function to print binary of a given decimal number.
4. Write a recursive function to print octal of a given decimal number.
5. Write a recursive function to calculate sum of first N Prime numbers.

## Assignment-41: lambda

1. Write a lambda expression to check if a number is even.
2. Write a lambda expression to find nth term of Fibonacci series
3. Write a lambda expression to calculate area of a circle.
4. Write a lambda expression to find HCF of two numbers.
5. Write a lambda expression to count words in a given text.

## Assignment-42: Variable Length Arguments

1. Write a function which receives variable length arguments to calculate average of integers. It
   returns the average of numbers.
2. Write a function which receives variable length arguments to find greatest element. It returns the
   greatest element
3. Write a function which receives variable length arguments to filter odd and even numbers. Store all
   odd numbers in a list and all even numbers in another list. Store both the lists in a tuple and return.
4. Write a function which takes variable length arguments to receive strings. Return the list of max
   length string or strings if multiple strings have the same length.
5. Write a function which takes variable length arguments to receive integers. Filter out Prime
   numbers and return a list of those Prime numbers.

## Assignment-43: map, reduce and filter

1. Write a python script to find number of vowels in each of the string in a given list of strings. Use
   map function.
2. Write a python script to find number of digits in each of the element in a given tuple of numbers.
   Use map function.
3. Write a python script to create a list of numbers greater than a given number N (taken from user)
   for each element in a given set of numbers. Use filter function.
4. Write a python script to filter only int type values in a given list of elements. Use filter function.
5. Write a python function to calculate HCF (Highest Common Factor) of a list of numbers. Use reduce
   function.

## Assignment-44: Decorator

1. Write a function to calculate HCF of two numbers. Define a decorator for HCF function to tell
   whether the two numbers are co-prime or not.
2. Define a decorator to display "Happy New Year" message at the beginning.
3. Define a decorator to display "Good Bye" message at the end.
4. Write a function to check if a given number N is a Prime or not. Define a decorator to print total
   number of Prime numbers before N.
5. Write a function to check if the given sides of a triangle can form a valid triangle or not. Define a
   decorator to print "Right Angled Triangle" if the triangle is right angled triangle.

## Assignment-45: Classes and Objects-1

1. Define a python class Person with instance object variables name and age. Set instance object
   variables in init() method. Also define show() method to display name and age of a person.
2. Define a class Circle with instance object variable radius. Provide setter and getter for radius. Also
   define getArea() and getCircumference() methods.
3. Define a class Rectangle with length and breadth as instance object variables. Provide
   setDimensions(), showDimensions() and getArea() method in it.
4. Define a class Book with instance object variables bookid, title and price. Initialise them via init()
   method. Also define method to show book variables.
5. Define a class Team with instance object variable a list of team member names. Provide methods to
   input member names and display member names.

## Assignment-46: Inheritance

1. Define a class Person with instance object variables name and age. Provide init() method to set
   instance object variables. Also define methods to show name and age. Now define a subclass
   Employee of Person with instance object variable salary. Provide init() method to initialise instance
   object variable. Also define instance method to show Employee data.
2. Define a class Account with instance object variables accountNo, balance and static variable
   rate_of_interest. Provide needful methods. Define subclass FixedDeposit of Account class with
   instance object variable time. Provide setter and getter. Also define a method to calculate simple
   interest.
3. Demonstrate the use of super() in inheritance.
4. Define a class Account with instance object variable balance with initial value as 0. Provide
   withdraw and deposit methods. Now define a subclass MinimumBalanceAccount of Account with
   provided minimum balance. Override withdraw method according to minimum balance condition.
5. Define a class Polygon with instance object variable to store number of sides and a list of n side
   length values. Define a subclass Triangle of Polygon with instance methods getArea().

## Assignment-47: Polymorphism

1. Define a Python class Person with name and age as instance object variables. Define Student and
   Teacher two subclasses of Person. Provide rollNo as instance object variable in Student, provide
   subject as instance object variable in Teacher class. Now define a function show to print values of
   instance object variables in both the classes. Demonstrate polymorphic behaviour or show function.
2. Overload greater than (>) operator in Time class which has instance object variables hour, min, sec.
3. Define a class Result to hold result data for a test (attempt, right and wrong). Overload + operator to
   combine the result of two tests.
4. Define a class matrix with member variables rows, columns and a list to hold matrix elements.
   Overload + operator to add two matrix objects.
5. In Question 4, define - operator to subtract two matrix objects.

## Assignment-48: Exception Handling

1. Define a Python function to calculate factorial of a number. Handle all possible exceptions.
2. Define a function to find greater value among three given data. Handle all possible exceptions.
3. How many else can be used with one try block?
4. When finally is executed?
5. Can we write try block without except clause?

## Assignment-49: Iterators and Generators

1. Write a generator to produce first N prime numbers
2. Write a generator to produce first N terms of the Fibonacci series.
3. Write a generator to produce squares of first N natural numbers.
4. Use iter and next method to print values of a given list using while loop which works equivalent to
   for loop.
5. Use iter and next method to check if all the elements of a list are even numbers using while loop
   which should work equivalent to for loop

## Assignment-50: File Handling

1. Write a function to write a given string in a given file.
2. Write a function to read text from a given file and display it on the screen.
3. Write a function to copy one file data to another file.
4. Write a function to read and store all the numbers found in a given text file into a list.
5. A file contains N lines, each line consist of a name and age separated by comma. Write a function to
   read this file and store data in a dict object with name as keys and age as value. Assuming the
   names are unique.

```

```

```

```
