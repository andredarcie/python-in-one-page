---
jupyter:
  jupytext:
    text_representation:
      extension: .md
      format_name: markdown
      format_version: '1.2'
      jupytext_version: 1.5.2
  kernelspec:
    display_name: Python 3
    name: python3
---

<!-- #region id="view-in-github" colab_type="text" -->
<a href="https://colab.research.google.com/github/andredarcie/python-in-one-page/blob/master/python_in_one_page.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
<!-- #endregion -->

<!-- #region id="Ufmoz5FB7IBt" colab_type="text" -->
# 📜 Python in one page
<!-- #endregion -->

<!-- #region id="dJIZpYWK7Qkp" colab_type="text" -->
## What is Python?

Python is a popular programming language. It was created by Guido van Rossum, and released in 1991.

To focus on the language itself this guide not includes any built-in modules like math, random, datetime, json, re, random, etc
<!-- #endregion -->

<!-- #region id="8Ry3S_PficPi" colab_type="text" -->
## 🧘 The Zen of Python
The Zen of Python is a collection of 19 **guiding principles** for writing computer programs that influence the design of the Python programming language.
<!-- #endregion -->

```python id="cO-Y8VZKibg_" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 374} outputId="2622fb4d-3675-4e76-edd9-6cab29bfb4c5"
import this
```

<!-- #region id="1Rwa7_m_7aXn" colab_type="text" -->
Make a simple hello world
<!-- #endregion -->

```python id="mjkYYWFp7DSp" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="70113632-3497-4e85-dac5-c0f968f5540e"
print('Hello, World!')
```

<!-- #region id="6752HQqs7AjA" colab_type="text" -->
**Help**
<!-- #endregion -->

```python id="z6z6XqsJ7DE2" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 221} outputId="4c50cb84-beca-4478-8abf-7fb4b7cfd8f0"
help(print)
```

<!-- #region id="6rVqe_fh7MX1" colab_type="text" -->
**Comments**
<!-- #endregion -->

```python id="IGRidkbj7OjW" colab_type="code" colab={}
#This is a comment
```

```python id="PZ-DoyxH7WSq" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="e6c7d410-9e00-4a4b-90c0-a0af56de77aa"
#Variables
name = 'John'
age = 42

x, y, z = 1, 2, 3

print('Name: ' + name)
```

```python id="C8CXc0xAReQy" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 68} outputId="c6d0c9ae-ba27-445d-9997-f4706a033f21"
# User input
# favorite_comedy_series = input('Enter your favorite comedy series: \n')
# print(favorite_comedy_series)
# output: Monty Python's Flying Circus
```

<!-- #region id="G8TtGB3N7ZSE" colab_type="text" -->
## 🔣 Data Types

Python has the following data types built-in by **default**
<!-- #endregion -->

```python id="wVZZdlFiLgDV" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="e694b38c-f499-4357-b913-6c99537eb967"
my_number = 42
print(type(my_number))
```

```python id="iotFWEk57agM" colab_type="code" colab={}
# Text
my_string = 'Hello World'

# Numeric
my_integer_number = 20
my_float_number = 20.5
my_complex_number = 1j

# Sequence
my_list = ['apple', 'banana', 'cherry']
my_tuple = ('apple', 'banana', 'cherry') # immutable sequence 
my_other_tuple = tuple(('apple', 'banana', 'cherry')) # immutable sequence 
my_range = range(4) # range(0, 4)

# Mapping
my_dictionary = {'name' : 'John', 'age' : 36}
my_other_dictionary = dict(name='John', age=36)

# Set - No duplicate members
my_set_value = {"apple", "banana", "cherry"}
my_other_set_value = set({"apple", "banana", "cherry"})
my_frozenset_value = frozenset({"apple", "banana", "cherry"})

# Boolean
my_boolean = True # Can be True of False
bool(0) # Return a Boolean value

# Binary
my_bytes = b"Hello"
my_bytearray = bytearray(5) # bytearray(b'\x00\x00\x00\x00\x00')
my_memoryview = memoryview(bytes(5)) # <memory at 0x01368FA0>
```

```python id="M4kgxFxk8GaG" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="4d8fcdd6-25a7-473c-bd28-147c28ce9880"
# Convert an integer number to a binary
print(bin(2))
```

```python id="UU1EIDks8KUT" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="f394e297-467a-4634-abee-f1ca4c032b5c"
# Convert an integer number to an octal
print(oct(8))
```

```python id="BeyAQirc8MQp" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="c197f7cd-521a-401a-fa17-45e0b4901753"
print(type(string))
```

```python id="JlzDEc158Pdp" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="f2280c89-4662-466c-9a57-0af4f6d9a239"
print(int('1'))
```

```python id="XzMz1ZE892MK" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="ceaf2483-dd5d-4716-c6d0-191c08225b36"
print(float(1))
```

```python id="Yy4X6975CIxW" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="89017586-ad6d-4623-ce2d-1cc1772ad39c"
# Convert an integer number to a lowercase hexadecimal string prefixed with '0x'
print(hex(255))
```

```python id="6yN8uJDo8ScS" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="28ec9cfc-ac1a-4461-a9d7-c898b6382f84"
# Represents a null value
x = None
print(x) # None
```

<!-- #region id="Ki_-evek8g9Y" colab_type="text" -->
## 🧵 Strings
A **string** is a sequence of Unicode **characters**
<!-- #endregion -->

```python id="n0Gtmes68ihx" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="8e85a7da-4a92-41f7-f7b8-335a9bba89cf"
hello = 'Hello, World! '
print(hello[0])
```

```python id="UxAvDzvC8mBR" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="0714ce62-2f50-4d53-8039-1a1891534814"
print(hello[-2])
```

```python id="O2i6hLn78tDw" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="2c5268ff-cbbf-4db4-adb0-f01b47448a5b"
print(hello[2:5])
```

```python id="iOGWD9TT8wQM" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="905edb4f-0ba9-4ccb-f8de-c4be9b3ac39f"
print(len(hello)) # returns the size of hello
```

```python id="DFt2XEB481u4" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="cce9a887-a155-418e-a3a1-0df2762aae2a"
print(hello.strip()) # removes whitespaces
```

```python id="u-yfaZX386jR" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="6ff7c689-d28d-4f27-bf5f-57ec9cb51830"
print(hello.lower())
```

```python id="b4M3ACDG87Xh" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="a41021d8-1b5b-416e-d808-38c61b64d20b"
print(hello.upper())
```

```python id="SbIe4Xwk89eS" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="ed3784d2-6dfc-44f2-d12d-ee70c05c7225"
print(hello.replace("H", "A"))
```

```python id="dFJqsnlz8_Ej" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="30cc890d-e08c-4e20-a3ab-a8037bef3885"
print(hello.split(","))
```

```python id="PC3l_YeI9AkW" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="0aa77f37-fc76-4fbf-863c-e8a51f6a0d82"
# Membership Operators
print("Hello" in hello)
print("Hello" not in hello)
```

```python id="_SlannlY9GQh" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="7e232d2b-1d25-46ba-c7c3-d056d4ac5ecb"
print('Hello, ' + 'World!')
```

```python id="vRvrYJyJ9HEX" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="65ea2a2b-3a44-4e24-d83d-08294bc4da4d"
print('Hello, ' 'World!')
```

```python id="kFhjB9yI9JqQ" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="f5657204-8a7e-4fd1-dd9e-8f6196adbc5b"
print("{0}, World!".format('Hello'))
```

```python id="s27Htl0f9Lap" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="4a216e89-e304-4563-8ba6-4cc1589c7301"
print('Hello, \n World!')
```

```python id="IDEaBAXT9NPR" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="ff8c75c6-a518-4b49-e280-e91f8cf31cab"
print(chr(97)) # Return the string representing a character
```

```python id="tN1jFCCH9Q7S" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="94d98778-a9ea-4827-93bd-b69f533967c4"
print(ord('a')) # Return an integer representing the Unicode
```

```python id="L_9D3fCTKT6h" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="91906547-6856-459b-e2ef-1c3c577abc01"
# print('Number is: ' + 1)
# TypeError: must be str, not int

# 'str()' return a string version of object
print('Number is: ' + str(1))
```

<!-- #region id="CamroSC1-3gL" colab_type="text" -->
## 🧮 Arithmetic
The arithmetic operators are used to perform **math operations**, such as addition, subtraction, multiplication, and division.
<!-- #endregion -->

```python id="P3NDAINl-6H0" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="7183a5f5-25d6-4462-e296-87f99e631d84"
x, y = 1, 2
print(x + y) # Addition
```

```python id="2Nl9eBRa-9B6" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="fab442e4-a168-4f65-f5b2-af4fe211bf36"
print(x - y) # Subtraction
```

```python id="MOtE63mK_A4M" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="8a71ec24-01af-4a01-c4f1-6a05ca316b19"
print(x * y) # Multiplication
```

```python id="-qBbKFgw_Cg_" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="9dbf84e7-37b7-4308-98b9-a93ed5dc3479"
print(x / y) # Division
```

```python id="Qu1a-OQS_EKi" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="05bb4313-e7b7-4af3-a80e-1e11178168a1"
print((50 - 5*6) / 4) # 5.0
```

```python id="DPRxB4Pb_Fxy" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="649caa12-8c7e-4c73-de7e-db265813bfda"
print(x % y) # Modulus
```

```python id="GBrC1v37_HU_" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="eae03427-8cc8-4c09-bc8b-8fdfdfb754a5"
print(x ** y) # Exponentiation
```

```python id="5RtkWd0Q_JZ2" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="020ae9a1-a22c-4606-ae01-5a2281a0b441"
print(x // y) # Floor division
```

```python id="i8iPP-ev_KvI" colab_type="code" colab={}
x += 3 # Same as x = x + 3
```

<!-- #region id="0ylkvUcA_NbG" colab_type="text" -->
## 🎎 Comparison
These operators **compare** the values on either sides of them and decide the **relation** among them
<!-- #endregion -->

```python id="37gNaeb4_Psp" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="7d6f4281-4052-4fc8-9615-371b239b6fba"
x, y = 1, 2
print(x == y) # Equal
```

```python id="OF-Kb2Hk_SHp" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="f6bd821b-0784-461b-f030-8d430319a20c"
print(x != y) # Not equal
```

```python id="5H3FO2xj_TfB" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="43215215-1b24-43af-aeda-7a26ea9bab2f"
print(x > y) # Greater than
```

```python id="4GmGv1Bs_V3k" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="5e4165b4-1c30-44fc-ebe5-c670305f57e9"
print(x < y) # Less than
```

```python id="neN-lpCE_WjB" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="42fef44d-c60a-4675-a315-fa082022b651"
print(x >= y) # Greater than or equal to
```

```python id="Id3-i3_H_YQf" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="ee406863-8a93-44ad-c32a-c4e275267c37"
print(x <= y) # Less than or equal to
```

```python id="d4IsbMVB_aBo" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="81515b90-973b-490e-a944-1cc5f5fef656"
if x > y:
  print("x is greater than y")
else:
  print("x is not greater than y")
```

```python id="8yPvkkFR_ffj" colab_type="code" colab={}
# Assert is used when debugging code
assert x == 1 # AssertionError is not raised
```

<!-- #region id="Xv237JGs_rIR" colab_type="text" -->
## 🤖 Logical
<!-- #endregion -->

```python id="F-y7Eu03_umm" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="f858e155-1302-40c2-a9c7-953c194d5b7f"
x = 2
print(x == 2 and x > 42)
```

```python id="pgjElYHv_xp2" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="70812e4a-d096-44c3-caaf-62801fa3eced"
print(x == 2 or x > 42)
```

```python id="17sfKffz_zbf" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="0b717f15-c7bf-4fc1-dd26-ff559363a4c2"
print(not(True))
```

```python id="iohQxagh_1A-" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="87ab2def-fa4d-4cae-821d-85266434b6d6"
print(not(False))
```

<!-- #region id="jRhwXouzZvMD" colab_type="text" -->
## 🖩 Math
Python has a set of built-in math functions
<!-- #endregion -->

```python id="bI4Gc-a_Z9Pl" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="0a061f45-a8b9-4883-dbdf-8c2aeea4e76e"
min_value = min(5, 10, 25) # lowest value
max_value = max(5, 10, 25) # highest  value

print(min_value)
print(max_value)
```

```python id="EVT-lGa1areJ" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="90501f0b-3af4-4d44-85c2-13cce9fe695f"
print(abs(-7.25)) # returns the absolute (positive) value
print(pow(4, 3)) # returns the '4' to the power of '3'
```

```python id="dkalkx_EzmMG" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="4156440b-ca5f-43d6-eeae-2a1d303ce174"
# Takes two numbers and returns a pair of numbers (a tuple) 
# consisting of their quotient and remainder
divmod(2, 2) # same as (2 // b, x % y)
```

```python id="D1_T5q7jIVi5" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="70b85ce1-30f0-4cb9-ccf5-22e69108209a"
# Return number rounded to ndigits precision after the decimal point
print(round(0.5))
print(round(1.5))
```

<!-- #region id="kJGDfVPs_3Y7" colab_type="text" -->
## 🆔 Identity
<!-- #endregion -->

```python id="QURkrB-m_4wA" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="d9827e50-45a4-4f9c-efd2-b333b18e4e96"
x = 'Hello'
z = x
y = 'World'

print(x is z)
```

```python id="zG-0JuVK_9YQ" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="028dba90-28a9-4bf2-f16d-e7b178e0107c"
print(x is y)
```

```python id="zKiAbuDo_-4f" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="efbbea27-6328-4bad-bc39-95e6484c9ebd"
print(x == y)
```

<!-- #region id="GjMhGBAnRICt" colab_type="text" -->
## 👪 Lists

List is used to group together other values.

Built-in methods for lists
<!-- #endregion -->

```python id="p0saMqzFRMi4" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="0a9f2a6e-80e0-4849-a4ea-cee23f5f62fa"
mylist = ['hello', 'world']
print(mylist)
```

```python id="32kEXOv9RRoy" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="950c3c2a-d3c6-41c8-f168-0c077fa53529"
print(f'{mylist[0]} - {mylist[-1]} - {mylist[0:1]} - {mylist[:1]} - {mylist[0:]}')
```

```python id="USAzKvdGRUCU" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="aaece8d5-62ba-403e-818c-f3bf12d8a78e"
print(mylist[-1])
```

```python id="CpDL0pJTRVqp" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="7527083d-cf56-4037-cdd1-53ec6004858b"
print(mylist[0:1])
```

```python id="ORc2asvjRW4b" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="9b675ffa-2bf5-4f36-9871-63fc1ad871e5"
print(mylist[:1])
```

```python id="f6DdDedgRYEy" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="4897b216-e470-40aa-a8fb-37ead636e1d3"
print(mylist[0:])
```

```python id="IcIQXAwoRZgU" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="f18a0a8d-d25f-48e2-efd3-565ffdcad5fd"
mylist[1] = "!"
print(mylist)
```

```python id="LOZTSe4JRb8T" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="3a6324c6-4164-4899-cdc4-3640ba2126dd"
for item in mylist:
  print(item)
```

```python id="GUi9wAjnRh2L" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="ca3ccef9-ece4-4668-b008-d5ae7cb52552"
if "hello" in mylist:
  print("Yes, 'hello' is in the mylist")
```

```python id="5f37hAzyRrd-" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="bbff115d-791f-49b6-eae1-fccfb587dc87"
print(len(mylist))
```

```python id="iHRBvBC9RvnF" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="46e37980-e925-474c-e8a9-596003a225c7"
mylist.append("world") # Add an item to the end of the list
print(mylist)
```

```python id="PFyWeBpZR8Ay" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="d1ffb8ba-6574-4623-bf79-e5a07b073ca4"
mylist.clear() # Removes all the elements
print(mylist)
```

```python id="Xp5INxs4THqx" colab_type="code" colab={}
mylist = ['hello', 'world']
my_other_list = mylist.copy() # Returns a copy of the list
```

```python id="0cqFO19ETRbm" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="a448045b-eedb-426e-b78c-892734835d6a"
my_other_list.count('hello') # Return the number of times the value "hello" appears
```

```python id="_izGl5TKTnJw" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="b31b663d-baf0-4aac-e78a-85ac4a903aa4"
mylist.extend(['apple']) # Extend the list by appending all the items from the iterable
print(mylist)
```

```python id="JRs90BllTsCj" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="a8342440-5218-48f7-dbb4-e69ad60ef289"
mylist.index('world')
```

```python id="D0SCR4QeWo32" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="3d97098a-209d-4eca-bf8c-b664b5fce6b6"
mylist.insert(1, "cucumber") # Adds an element at the specified position
print(mylist)
```

```python id="wBiRn19fW-3b" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 35} outputId="fbfb94ad-9410-42d6-e4a7-8cd9e41dddbc"
mylist.pop() # Removes the last item from the list
```

```python id="7B017CYHXL4u" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="38f2687b-0159-4ee8-a5f0-aa774fb75692"
print(mylist)
mylist.remove("cucumber") # Remove the item at the given position in the list, and return it
print(mylist)
```

```python id="OPDPO0SqXTi1" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 68} outputId="ccac7883-467a-4b74-ec86-bdd0feb100db"
my_number_list = [ 1, 2, 3]
my_number_list.reverse()
print(my_number_list)
print(reversed(my_number_list))
my_number_list.sort()
print(my_number_list)
```

```python id="OMdsv501XjYZ" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="e35fe6b2-fc1f-4664-b2c8-6e2ca4a546f6"
del my_number_list[0]
print(my_number_list)
```

```python id="YRato6ioXpjp" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="39e327e7-fbd9-47b9-a38c-adb7a275e0e8"
all(my_number_list) # Return True if all elements of the iterable are true
```

```python id="viC2FjK0XvVU" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="db1675ae-dc36-4072-8058-f34f6a28bab7"
print(any(my_number_list)) # If the iterable is empty, return False
my_number_list.clear()
print(any(my_number_list))
```

```python id="yEQ2loNBYCmA" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="43ea72f6-7633-4d35-d3ed-986020b7a780"
letters = [ 'a', 'b', 'c' ]
numbers = [ 1, 2, 3 ]
print(letters + numbers)
```

```python id="_s2Zu5AyYPOG" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="653fff26-8850-4fbc-ccb4-4b6d739fe1c7"
mylist = list(("apple", "banana", "cherry"))
print(mylist)
```

```python id="JJHCvd1W1gtV" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="2bf9becc-8b74-42ee-9d7e-22dc428a0818"
my_other_list = [ 'a', 'b', 'c', 'd', 'e' ]

start = 0 # position to start the slicing
end = 5 # position to end the slicing
spet = 2 # step of the slicing
slice_obj = slice(start, end, spet)

my_other_list[slice_obj]
```

```python id="ShRfhx706it6" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="4e819f24-9f92-4beb-ef6c-63727cad0e97"
my_iterable = [ 1, 2, 3, 4, 5 ]

def bigger_than_three(number):
  return number > 3

output_list = filter(bigger_than_three, my_iterable)
print(list(output_list))
```

```python id="7KzRUtPrEdML" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="b3f202c7-5998-43c7-c75a-94d0f54d7df5"
my_iterable = [ 1, 2, 3, 4, 5 ]

def add_one(number):
  return number + 1

output_list = map(add_one, my_iterable)
print(list(output_list))
```

```python id="Z7YlfTaTJmRz" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="7d59ff3d-7bb3-400d-d8e4-0d59cc9a7fa3"
# Return a new sorted list from the items in iterable
my_sorted_list = sorted([5, 4, 3, 2, 1])
print(my_sorted_list)
```

```python id="BmNYzYCmLLpN" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="fb6c7224-39ee-4531-d6fe-0919876c045b"
my_reversed_list = reversed(my_sorted_list)
print(list(my_reversed_list))
```

<!-- #region id="3xLBKzHLudHz" colab_type="text" -->
## 🏷️ Sets
Unordered collections of unique elements
<!-- #endregion -->

```python id="gU_S08k3ufH8" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="cc114725-0dea-4b94-aae1-4a4c08cee60e"
my_set = {'python', 'is', 'awesome'}
print(my_set)
```

```python id="jxjvW5McwP9z" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="64889b68-6155-49bd-96c8-fe063a47e352"
len(my_set) # Return the number of elements in set
```

```python id="sDi8RoDVv_-_" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 68} outputId="dbb63a9c-a948-4f09-e0df-ce9a908e37fb"
for item in my_set:
  print(item)
```

```python id="XgsjbB-gwFQp" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="4806f5aa-2da8-4a95-e076-7661d57a1046"
print('python' in my_set) # Check if 'python' is present in the set
print('python' not in my_set) # Check if 'python' is not present in the set
```

```python id="CoSkE7vZwYFs" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="a2fa06eb-cb57-4231-fa24-a4c01be88ac5"
my_set.add('🐍')
print(my_set)
```

```python id="bfJ9n4_Zw5-X" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="3bcbb938-f5d4-4d92-d20c-e8712cc382a8"
my_set.update(['and', 'very', 'nice'])
print(my_set)
```

```python id="EEMyLrCaxEB9" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="677f6f50-14df-4c16-c905-08e714e4e534"
my_set.remove('🐍')
# If the item to remove does not exists, discart will not raise an error
my_set.discard('python') 
print(my_set)
```

```python id="2k4cDUE-xgsJ" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 35} outputId="675bd3d8-a8b0-425c-fb22-b02c66ba23ad"
my_set.pop() # Remove and return an arbitrary element from the set
```

```python id="AEOtQ_gFx1J5" colab_type="code" colab={}
my_set.clear() # Remove all elements from the set
```

<!-- #region id="cf7XH8kHCNOU" colab_type="text" -->
## 📙 Dictionaries
A dictionary is a collection which is unordered, changeable and indexed.
<!-- #endregion -->

```python id="z2Y0KsItCbyH" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="4de7de8e-d22f-41d4-c942-5c31d7ec6eb4"
my_dict = {
  'name': 'Python',
  'designed_by': 'Guido van Rossum',
  'first_released': 1991
}
print(my_dict)
```

```python id="XqKrhKpiEh42" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="5c382204-386e-4fd7-a0ed-c0dfea18ebdd"
print(my_dict['name'])
```

```python id="ZZ7HOuOhxJLr" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="32a15440-1ab6-4b84-c89b-2de662ab9d6d"
my_dict['first_released'] = 2077
print(my_dict)
```

```python id="p3fYGu8p2D81" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 68} outputId="9beac222-1c9d-4c0f-8159-cffb15d59c61"
for value in my_dict.values():
  print(value)
```

```python id="fqaHWfbc2U2o" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 68} outputId="a3b83da4-abaf-45b2-c642-067e3fcd332a"
for key, value in my_dict.items():
  print(key, value)
```

```python id="JnnLxMUD2dhG" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="dd968d1f-dfe9-4a38-b24e-9cb162eef606"
if 'name' in my_dict:
  print('The key "name" exists in my_dict')
```

```python id="TDA_xaoH32DR" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="ec6daefd-7665-4ae5-94c5-84dc648fac43"
my_dict['website'] = 'www.python.org' # Add a new item
print(my_dict)
```

```python id="2jcLDP104QW_" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="1266c856-0f72-404a-cc2b-f4432b46c027"
my_dict.pop('website')
print(my_dict)
```

```python id="-aAGX97O4ZZ7" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="7cd7bdba-b696-4c7a-b85e-3c7088e62beb"
my_dict.popitem()
print(my_dict)
```

<!-- #region id="VM12scNS4gXi" colab_type="text" -->
## ↪️ If ... Else
<!-- #endregion -->

```python id="ruc4mgev5LxO" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="0ce94d87-2e99-4d9a-b882-47e942f9420b"
x, y = 1, 2
if x > y:
  print('x is greater than y')
elif x == y:
  print('x and y are equal')
else:
  print('x is greater than y')
```

```python id="YmQy2CZX56a4" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="36d956f6-e9a5-4c9a-a7de-2a20c7a33b3b"
# Short Hand
if x > y: print('x is greater than y')
print('x') if x > y else print('y')
```

<!-- #region id="p4UGea5X6BKN" colab_type="text" -->
## 🔁 Loops
*'for' is used to iterate over the elements of a sequence (such as a string, tuple or list) or other iterable object*
<!-- #endregion -->

```python id="jYhCft1F7f5n" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 68} outputId="bc6bbbb4-b148-424c-9a6e-27db1d7a2c9b"
quote = ['Python', 'is', 'awesome']
for word in quote:
  print(word)
```

```python id="4gg9rsS38Ef0" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="99b22ac0-a511-4257-a211-43ed7cf27103"
for number in range(4):
  print(number, end=' ')
```

```python id="ZMYtbO5vx8tv" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 68} outputId="5becce08-e1f0-48c2-930a-9da87c09c63f"
for index, value in enumerate(quote):
  print(index, value)
```

```python id="OpUWJpyp8yET" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="5b33c513-cef0-43ae-b7ea-dfceb707002d"
# Function continues execution immediately 
# after the last yield run
def number_generator(): 
    yield 1
    yield 2
  
for number in number_generator():  
    print(number)
```

<!-- #region id="bAgB3h8Z7RlW" colab_type="text" -->
*'while' is used for repeated execution as long as an expression is true*
<!-- #endregion -->

```python id="btdERdbb6veG" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="74eb1604-3435-4a3c-dd50-c9998489a281"
counter = 0
while counter < 4:
  print(counter, end=' ')
  counter += 1
```

<!-- #region id="8c8HglBt90nl" colab_type="text" -->
## ☄️ Functions
A function is a block of code which only runs when it is called.
<!-- #endregion -->

```python id="c5nWFpLK_hUT" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="0f48cfb6-a4e4-43f5-8b98-2dbf6bcbb2b5"
def my_function():
  print("Hello, World from a function")

my_function() # Call a function
```

```python id="DD7NT7KMHvOy" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="1a53d72b-5664-4c82-bb00-1169b7a601f1"
# A function to add two numbers
def sum(number):
  return number + number

print(sum(2))
```

```python id="06RJApfW_yxD" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="35c19f69-38d6-4dec-87f5-8880d41f4dba"
def my_function(programming_language): 
  print(programming_language + ' is awesome!')

my_function('Python') # Pass parameters
```

```python id="ayfYHgglASnD" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="0482466a-f3f2-4016-f332-abc2370f16cb"
def my_function(*parameters):
  print("The third parameter is: " + parameters[2])

my_function('Python', 'is', 'easy', 'to', 'learn')
```

```python id="fRYHRKwwDvhs" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="eba8f8ad-c5b6-444c-d1fd-bbf2d454bd1a"
def my_function(name, surname):
  print(name, surname)

my_function(surname='van Rossum', name='Guido')
```

```python id="wUyUNpuRGaZq" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="5aa23efc-dba6-4d1f-e942-2542ffa923bd"
def my_function(programming_language="Python"): # Default parameter value
  print(programming_language + ' is awesome!')

my_function("Ruby")
my_function()
```

```python id="xSYSWZ49IQyW" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="f8897aa8-82d2-4f9b-8d68-b8f766e72e2a"
# True if the object argument appears callable
callable(my_function) # True
```

<!-- #region id="KVplOS2ZK02W" colab_type="text" -->
## 🛰️ Lambda Function
Is a small anonymous function
<!-- #endregion -->

```python id="xXgUxdhfN5IX" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="1609cb8d-67e3-4619-8b5e-024ffc727585"
# lambda arguments : expression
my_function = lambda x : x
print(my_function(2))
```

```python id="1rEzuWuwPNuf" colab_type="code" colab={}
# is equivalent to
def my_function(x):
  return x
```

```python id="cCNlhWjXOw6e" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="72cf6914-0efd-4106-98f7-8ace9812622a"
sum = lambda x, y : x + y # Two parameters
print(sum(2, 2))
```

```python id="9wRfXl_kPWnu" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="04d2cfa9-0d1e-471b-a827-10b140baa482"
def call_any_function(func):
  print(func(2, 2))

call_any_function(sum) # Pass the 'sum' lambda function as parameter
```

<!-- #region id="Ehq9NjVcOEVl" colab_type="text" -->
## 📦 Classes and Objects
A **class** is a blueprint for an **object**, and an **object** is simply a collection of variables and functions that act on those variables.
<!-- #endregion -->

```python id="xqUGjnCvOcLm" colab_type="code" colab={}
class Person:
  def __init__(self, name, age):
    # Instance attribute’s
    self.name = name
    self.age = age

  def show_name(self):
    print("My name is " + self.name)
```

```python id="PU8gQqqvPU8L" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="de159cca-88aa-4724-a3c9-724750ff3d99"
king_arthur = Person('Arthur', 26)
print(king_arthur)
```

```python id="Pt4BpvxZ3krZ" colab_type="code" colab={}
# King Arthur is a Person object at the memory address 0x7fb265f652b0
```

```python id="_s6HvmoYQQPr" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="30597df3-41dd-4043-b6eb-bf90c3664e73"
king_arthur.show_name()
```

```python id="yE2ayGcHQhAa" colab_type="code" colab={}
king_arthur.age = 27 # Modify object properties
```

```python id="KGo5JFQRQ49y" colab_type="code" colab={}
# Use inheritance to create child classes from a parent class
class Knight(Person):
  def speak(self):
    print('Ni!')
  
# Now the Knight class has the same properties 
# and methods as the Person class plus the 'speak()' method
```

```python id="XhWEGexuRWTS" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="2104c776-4b07-4ba6-c0ec-380531aea00c"
lancelot = Knight('Lancelot', 25)
lancelot.show_name()
```

```python id="9VTsF3KBSU0q" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="5b28b77e-ff7f-461f-c5d5-86e629e62895"
lancelot.speak()
```

```python id="f76VJfWSSy94" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="5cb41f4e-dcbe-4764-d7e8-116f904a877d"
vars(lancelot)
```

```python id="EVoRK_ArTBss" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="15cef0a3-aab3-4f0a-cdd4-306702f3e7fb"
# Return the 'identity' of an object
id(lancelot)
```

```python id="rvRmqFPK_N4c" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="f143ebb2-51da-416f-931b-5b9e93da5c08"
# Determine which class a given object belongs to
type(lancelot)
```

```python id="LQmBJHbKTHa8" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 68} outputId="db9f58c6-b62c-4ee7-c0e5-c0d4fef8dfe5"
print(isinstance(lancelot, Knight))
print(isinstance(king_arthur, Knight))
print(issubclass(Knight, Person))
```

```python id="LVfun59I1CaO" colab_type="code" colab={}
class Peasant(Person):
    # Class attributes are attributes that have the 
    # same value for all class instances.
    political_position = "We're an anarcho-syndicalist commune."
    
    # Friendlier output for print()
    def __str__(self):
      return f"{self.name} is {self.age} years old"

    # You can access the parent class from 
    # inside a method of a child class by using super()
    def show_name_using_super_method(self):
      super().show_name()

    # Static method it's not bound to instance or class and you 
    # can simply call that using class name
    @staticmethod
    def talk_about_politics():
      print(Peasant.political_position)

    # A class method receives the class as implicit first argument
    @classmethod
    def show_class(cls):
      print(cls)
```

```python id="siyQ-AJY8j-n" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="26e3c6b7-aba0-4703-a6c6-c80782bd25a3"
dennis = Peasant('Dennis', 37)
print(dennis)
```

```python id="CbkgoPgH_sJp" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="5bd35c70-13be-4714-c22c-4020e3ae9030"
dennis.show_name_using_super_method()
```

```python id="sN_i61SOB0ME" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="8b1c514d-517a-4bcc-a8fd-ea454473a3a8"
dennis.talk_about_politics() # Static method
```

```python id="2YpWrqqSDwvt" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="6ab7b08a-0b29-47c4-d78b-10c5071e7cb7"
Peasant.show_class() # class method
```

```python id="DFM4y8Jc-VWB" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 35} outputId="6825bf91-1e4f-48f4-945a-22bc4b5b064c"
getattr(dennis, 'name')
```

```python id="4Q2BDaoQJGI5" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="00a9dbec-99d5-487b-8156-624cc1568ada"
print(dennis.name)
# The function assigns the value to the attribute
setattr(dennis, 'name', 'Other Name') # same as dennis.name = 'Other Name'
print(dennis.name)
```

```python id="q31BrASmAPz3" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="35316d34-39c8-4805-f42a-0c9cef728493"
print(hasattr(dennis, 'name'))
print(hasattr(dennis, 'email'))
```

```python id="pjxcQsrTBKHn" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="73203d4f-17f6-4165-93e8-f1720918c97a"
# Return the hash value of the object (if it has one)
print(hash(dennis))

# They are used to quickly compare dictionary keys during a dictionary lookup
print(hash(dennis) == hash(dennis))
```

```python id="jlnUIGrZN3wd" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="eca065c2-762d-4d95-d1ba-96bbdc3be0d8"
# Return a string containing a printable representation of an object
print(repr(dennis))
```

```python id="RqhqhpLQEgKi" colab_type="code" colab={}
# The function deletes the named attribute
delattr(dennis, 'name')
```

```python id="bqE-HiZmL0nd" colab_type="code" colab={}
# 'property()' Return a property attribute
# class property(fget=None, fset=None, fdel=None, doc=None)
# - doc creates a docstring for the attribute

class C:
  def __init__(self):
      self._x = None

  # function for getting an attribute value
  def getx(self):
      return self._x

  # function for setting an attribute value
  def setx(self, value):
      self._x = value

  # function for deleting an attribute value
  def delx(self):
      del self._x

  x = property(getx, setx, delx, "I'm the 'x' property.")

c = C()
c.x # invoke the getter
c.x = 2 # invoke the setter
del c.x # invoke the deleter

# This code is exactly equivalent to the first example
class C:
    def __init__(self):
        self._x = None

    @property
    def x(self):
        """I'm the 'x' property."""
        return self._x

    @x.setter
    def x(self, value):
        self._x = value

    @x.deleter
    def x(self):
        del self._x
```

```python id="pThWhVeZ5O5B" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 54} outputId="c0e5289e-3029-4028-a6b5-789e4e449146"
# The object() function returns a featureless
# object which is a base for all classes
my_object = object()

# Get all the attributes
print(dir(my_object))
```

<!-- #region id="UQ7KOR12aqeq" colab_type="text" -->
# ➰ Iterators
An iterator is an object that can be **iterated** upon, meaning that you can traverse through all the values.
<!-- #endregion -->

```python id="rncFI-Gna0Vh" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 68} outputId="bcb4f651-1bb5-4abf-83ef-bced5455e41f"
# Lists, tuples, dictionaries, and sets are all iterable objects
my_list = [ 1, 2, 3 ]

# The 'for' takes the list iterator 
# and then moves through it using 
# the built-in 'next' iterator method
for number in my_list:
  print(number)
```

```python id="Uhrmi3klmVLD" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 68} outputId="d7801da1-c428-4a30-df30-f64065a97104"
# Let's repeat what the 'for' does, but now manually
my_list = [ 1, 2, 3 ] # The same list
list_iterator = iter(my_list) # Returns the iterator

print(next(list_iterator)) # Returns the next value of iterator
print(next(list_iterator))
print(next(list_iterator))
```

```python id="_erbjA76h-Qz" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 68} outputId="764aea5b-fe8a-4a43-b19b-2f79b3bca6ee"
# It is possible to do the same but with a 'while' loop
my_list = [ 1, 2, 3 ]
list_iterator = iter(my_list)

while True:
  try:
    current_value = next(list_iterator) 
    print(current_value)
  # The 'next' method returns an exception when the list ends
  except StopIteration:
    break # Stops the while loop
```

```python id="z26Ey6L7nWaB" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 68} outputId="24063068-e404-42af-f5fb-4f1be3ddb5eb"
# It is possible to create an iterator,
# is a class that has to have two methods, the 'iter' and the 'next'
class MyNumbers:
  # Return the iterator
  def __iter__(self):
    self.end = 3
    self.value = 1 # Start value
    return self # Return himself

  # It says how to get the next value
  def __next__(self):
    if self.value > self.end:
      # Stops the execution of the 'for' loop
      raise StopIteration
    
    current = self.value
    self.value += 1
    return current

my_numbers = MyNumbers()
for number in my_numbers:
  print(number)
```

<!-- #region id="1OY47wXd7EWG" colab_type="text" -->
## 🔗 Scope
Scope refers to the coding region from which particular object is **accessible**. 

LEGB rule (Local, Enclosing, Global, and Built-in):
- Built-in Python scope (Predefined names: **open**, **range**, **len**, **etc**)
- Global or module scope (Names assigned at top-level of a module or declared **global** in function)
- Enclosing or nonlocal scope (Only exists for nested functions)
- Local or function scope (Names assigned inside a function **def**)
<!-- #endregion -->

```python id="kS6yT-lZGoE9" colab_type="code" colab={}
len('len() is a built-in function') # built-in scope
number = 0 # global scope

def my_function_one():
  number = 1 # enclosed scope
  def my_function_two():
    number = 2 # local scope
```

```python id="H3ufOdn27ZXY" colab_type="code" colab={}
def my_function():
  number = 2

my_function()

# print(number) NameError: name 'number' is not defined
# The variable number cannot be accessed from outside the function
```

```python id="zR0plQ388DmS" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="301c4bc7-fce1-4eb3-879f-d53b1923c953"
def myfunction():
  global number # global variable
  number = 2

myfunction()

print(number) # can be accessed outside the function
```

```python id="3-N60Fb1891B" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="f73edde7-6926-4ebb-c1df-f89df4c0acd5"
number = 2 # can be used inside the function

def my_function():
  print(number)

print(number)
```

```python id="XOsWNdla9VV4" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="cd2e0564-fc9b-47a1-963e-54f4647142e9"
def my_function_one():
  name = "King Arthur"
  def my_function_two():
    # Update and return a dictionary representing the current local symbol table
    print(f'Local: {locals()}')

    nonlocal name # non local variable
    # sets the value of 'name' variable of the 'my_function_one()'
    name = "Black Knight" 
  my_function_two()
  return name

print(my_function_one())
```

<!-- #region id="SpAdGIu3JYcF" colab_type="text" -->
## 🧱 Modules
Simply, a module is a file consisting of Python code. A module can define **functions**, **classes** and **variables**.
<!-- #endregion -->

```python id="TEToniA5J5n0" colab_type="code" colab={}
# Save this code in a file named 'my_module.py'
def greeting(name):
  print('Hello, ' + name)
```

```python id="kxJ8b47UKCyM" colab_type="code" colab={}
# This code is commented out because it doesn't run on the jupyter notebook
# import my_module
# my_module.greeting('Rabbit of Caerbannog')
# output: Hello, Rabbit of Caerbannog
```

```python id="nhssiQqoLB3T" colab_type="code" colab={}
# Create an alias for my_module called my
# import my_module as my
# my.greeting('Rabbit of Caerbannog')
# output: Hello, Rabbit of Caerbannog
```

```python id="qboXVt4z_ZjI" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="4715b656-fcf4-4f9f-a99f-f2586117b049"
# Return a dictionary representing the current global symbol table
print(len(globals()))
globals()['my_iterable']
```

<!-- #region id="tZ4X5puebsL2" colab_type="text" -->
## Try Except
<!-- #endregion -->

```python id="A83gFZEkb0N1" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="95e590bc-2b90-4a97-d5ec-6f5bc156f6ac"
try:
  raise Exception("Sorry, no numbers below zero")
except:
  print("Something went wrong")
finally:
  print("The 'try except' is finished")
```

<!-- #region id="B2-qjeZAcKAQ" colab_type="text" -->
## File Handling
<!-- #endregion -->

```python id="GxTK3GigcL-Q" colab_type="code" colab={}
# This code is commented out because it doesn't run on the jupyter notebook
# file = open("hello.txt", "r")
# r - Read
# a - Append
# w - Write
# x - Create

# print(file.read())
# print(file.readline())
# file.close()

# Using with statement 
# with open('hello.txt', 'w') as file: 
#    file.write('hello world !')

# no need to call file.close() when using with
```

<!-- #region id="FsJlTI7Bcdtj" colab_type="text" -->
## Other built-in Functions
<!-- #endregion -->

```python id="_EVdZUs0cfHA" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 68} outputId="c30190b7-ae75-49ca-b19e-a29e03db9640"
# Returns a readable version of any object 
# (Strings, Tuples, Lists, etc)
ascii([ 1, 2, 3 ]) #  1, 2, 3
```

```python id="JzJ4iZ-OdN7i" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="b767060b-7d62-411e-b4bd-27fa2b837967"
# Compile the source into a code or AST object
ast = compile('print("Hello, World!")', 
              'test', 'eval')

# Code objects can be executed by:
exec(ast) # Hello, World!
eval(ast) # Hello, World!
```

```python id="71w235lLdSRq" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="e8751be5-78c1-44c2-b2dd-6d6b83b1905b"
# Convert the number 4 and imaginary 
# number 2 into a complex number
print(complex(4, 2)) # (4+2j)
```

```python id="MNahWISbdrMv" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 51} outputId="43c1cce9-70e2-4cec-9607-52ea99c8f893"
# The 'zip()' function takes in iterables as arguments and returns an iterator. 
numbers = [1, 2, 3]
letters = ['a', 'b', 'c']
zipped = zip(numbers, letters)
print(type(zipped))
print(list(zipped))
```

```python id="pq31R97lHkNr" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 68} outputId="41629680-53a6-481d-fa17-ac05a0b20e31"
for number, letter in zip(numbers, letters):
  print(number, letter)
```

<!-- #region id="VtShPlLje2tQ" colab_type="text" -->
## Other things
<!-- #endregion -->

```python id="CGPBRuE9e43_" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="60691dd7-ca6c-4b3f-f56d-4f19930f14ac"
# In interactive mode, the last printed expression 
# is assigned to the variable _
2 + 2
print(_)

# This function drops you into the debugger at the call site
breakpoint()
```

```python id="i9klY2O7ObwO" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="84f888c9-10b6-42a5-bb91-afd62478f540"
# '__main__' is the name of the scope in which top-level code executes
# A module’s __name__ is set equal to '__main__' when read from standard 
# input, a script, or from an interactive prompt
print(__name__)
```

```python id="BPI9drryT-8C" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 34} outputId="4ffb7128-c2b7-4bca-f7bb-8494ee1c086b"
if __name__ == "__main__":
    # execute only if run as a script
    print('Your Module Is the Main Program')
```

<!-- #region id="tKxvCVpCfCzs" colab_type="text" -->
## All keywords
<!-- #endregion -->

```python id="jnjYWkwIfD73" colab_type="code" colab={"base_uri": "https://localhost:8080/", "height": 54} outputId="61edab76-362f-4513-ed1d-9bcbb59a9d3c"
import keyword
print(keyword.kwlist, sep='')
```
