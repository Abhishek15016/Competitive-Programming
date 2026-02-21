# 📘 C++ Basics – Beautiful & Structured Revision Notes
---

# 1️⃣ Introduction to C++

* C++ is a **powerful programming language**
* Used heavily in **Competitive Programming**, **DSA**, and **System Programming**
* You don’t need to know everything — focus on **important basics first**

---

# 2️⃣ Basic Structure of a C++ Program

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "Hello World";
    return 0;
}
```

### 🔹 Explanation

### 1. `#include <iostream>`

* This is a **header file**
* It allows us to use `cout`, `cin`
* Without it → Output/Input won't work

### 2. `using namespace std;`

* Allows us to write `cout` instead of `std::cout`
* Ignore deep details for now

### 3. `int main()`

* Program execution starts from `main()`
* It is mandatory

### 4. `return 0;`

* Ends the program

---

# 3️⃣ Header Files

Different tasks require different headers.

| Task                             | Header File       |
| -------------------------------- | ----------------- |
| Input/Output                     | `<iostream>`      |
| Square root                      | `<cmath>`         |
| Competitive Programming shortcut | `<bits/stdc++.h>` |

### Example:

```cpp
#include <cmath>

cout << sqrt(16);
```

Without `<cmath>` → Error
With `<cmath>` → Output: `4`

---

# 4️⃣ Output in C++

```cpp
cout << "Hello";
```

### New Line Options

```cpp
cout << "Hello\n";
cout << "Hello" << endl;
```

* `\n` → New line character
* `endl` → Inserts new line and flushes buffer

---

# 5️⃣ Variables in C++

Variables store data.

```cpp
int a = 5;
int b = 10;
int sum = a + b;
```

Think of variables as **boxes storing values**.

---

# 6️⃣ Data Types in C++

| Data Type | Stores               | Example |
| --------- | -------------------- | ------- |
| `char`    | Single character     | 'A'     |
| `int`     | Integer numbers      | 10      |
| `float`   | Decimal numbers      | 3.5     |
| `double`  | More precise decimal | 3.14159 |
| `bool`    | true / false         | true    |

---

## 🔹 6.1 Character (`char`)

```cpp
char c = 'A';
cout << c;
```

⚠ Only one character allowed.

---

### ASCII Concept

Internally every character has a number.

Example:

* 'A' → 65
* 'a' → 97

```cpp
char c = 'A';
cout << (int)c;   // prints 65
```

Typecasting converts one type into another.

---

## 🔹 6.2 Integer (`int`)

```cpp
int x = 10;
```

If you store decimal in int:

```cpp
int x = 4.5;
```

Output → `4`
👉 Decimal part gets removed (not rounded)

---

## 🔹 6.3 Double

```cpp
double d = 3.5;
```

Used for decimals with better precision.

---

## 🔹 6.4 Boolean (`bool`)

```cpp
bool flag = true;
```

Output:

* `true` → 1
* `false` → 0

Important:

* Only `0` is false
* Any non-zero number is true

---

# 7️⃣ Long & Long Long

For very large numbers:

```cpp
long long int x = 1234567890;
```

Used in Competitive Programming when `int` range is not enough.

---

# 8️⃣ Operators in C++

---

## 🔹 8.1 Arithmetic Operators

| Operator | Meaning             |
| -------- | ------------------- |
| +        | Addition            |
| -        | Subtraction         |
| *        | Multiplication      |
| /        | Division            |
| %        | Modulus (Remainder) |

### Example:

```cpp
cout << 10 % 3;  // Output: 1
```

---

## 🔹 8.2 Increment & Decrement

This confuses many beginners.

### Post-Increment

```cpp
a++;
```

* Use value first
* Then increase

### Pre-Increment

```cpp
++a;
```

* Increase first
* Then use value

---

### Example

```cpp
int a = 5;
cout << a++;   // prints 5
cout << a;     // prints 6
```

```cpp
int a = 5;
cout << ++a;   // prints 6
```

---

### Same logic for `--`

* `a--`
* `--a`

---

# 9️⃣ Relational Operators

Used in conditions.

| Operator | Meaning       |
| -------- | ------------- |
| ==       | Equal to      |
| !=       | Not equal     |
| >        | Greater than  |
| <        | Less than     |
| >=       | Greater equal |
| <=       | Less equal    |

---

# 🔟 Input in C++

```cpp
int a;
cin >> a;
```

Multiple inputs:

```cpp
int a;
double b;
cin >> a >> b;
```

---

## Important About `cin`

* It ignores:

  * Spaces
  * New lines
* Reads until space/newline

---

# 1️⃣1️⃣ Character Input Behavior

```cpp
char c;
cin >> c;
```

If input:

```
12345
```

It will store:

```
'1'
```

Remaining input stays in buffer.

---

# 1️⃣2️⃣ Difference Between Single & Double Quotes

| Symbol    | Used For  |
| --------- | --------- |
| `'A'`     | Character |
| `"Hello"` | String    |

---

# 1️⃣3️⃣ Type Casting

Convert one type to another:

```cpp
char c = 'A';
cout << (int)c;  // ASCII value
```

---

# 1️⃣4️⃣ Important Competitive Programming Tip

Instead of writing many headers:

```cpp
#include <bits/stdc++.h>
```

Includes almost everything.

---

# 🧠 Quick Revision Summary

✔ Program starts from `main()`
✔ Use `#include` for libraries
✔ `cout` → Output
✔ `cin` → Input
✔ `int` removes decimal
✔ `bool` → 0 is false, others true
✔ `%` gives remainder
✔ `a++` vs `++a` difference
✔ Characters have ASCII values

---

