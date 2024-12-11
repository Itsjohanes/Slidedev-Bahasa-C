---
theme: seriph
background: https://source.unsplash.com/collection/94734566/1920x1080
class: 'text-center'
highlighter: shiki
lineNumbers: true
info: |
  ## The C Programming Language
  A comprehensive overview from history to modern usage.
drawings:
  persist: false
css: unocss
---

# The C Programming Language

From History to Modern Development

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

---
layout: default
---

# History of C

- Developed by Dennis Ritchie at Bell Labs between 1969 and 1973
- Created to develop the UNIX operating system
- Evolved from earlier languages: BCPL and B
- Designed for systems programming
- Influenced countless programming languages

<div class="mt-8">
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/23/Dennis_Ritchie_2011.jpg/220px-Dennis_Ritchie_2011.jpg" class="rounded shadow" width="200" />
<p class="text-sm text-gray-500">Dennis Ritchie - Creator of C</p>
</div>

---
layout: two-cols
---

# Key Features of C

- Structured programming language
- Low-level memory access
- Simple and efficient
- Portable across platforms
- Small standard library
- Static type system

::right::

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

---
layout: default
---

# Basic Syntax Elements

```c {all|1|3|4-6|8}
#include <stdio.h>  // Header inclusion

int main() {       // Main function
    // Variables
    int number = 42;
    char letter = 'A';
    
    return 0;      // Return statement
}
```

- Headers provide access to library functions
- Every C program starts from main()
- Variables must be declared with types
- Functions return values (usually)

---
layout: default
---

# Data Types in C

| Type | Description | Example |
|------|-------------|---------|
| int | Integer numbers | int x = 42; |
| float | Single precision floating point | float pi = 3.14f; |
| double | Double precision floating point | double e = 2.71828; |
| char | Single character | char grade = 'A'; |
| void | No type | void function(); |

```c
// Example of different data types
int count = 100;
float price = 99.99f;
char initial = 'J';
double precise = 3.14159265359;
```

---
layout: default
---

# Control Structures: If Statement

```c
if (condition) {
    // code if condition is true
} else if (another_condition) {
    // code if another_condition is true
} else {
    // code if no condition is true
}
```

Example:
```c
int age = 18;

if (age >= 18) {
    printf("You can vote!\n");
} else {
    printf("Too young to vote.\n");
}
```

---
layout: default
---

# Loops in C

### For Loop
```c
for (int i = 0; i < 5; i++) {
    printf("%d ", i);
}  // Output: 0 1 2 3 4
```

### While Loop
```c
int i = 0;
while (i < 5) {
    printf("%d ", i);
    i++;
}
```

### Do-While Loop
```c
int i = 0;
do {
    printf("%d ", i);
    i++;
} while (i < 5);
```

---
layout: default
---

# Functions in C

```c
// Function declaration
return_type function_name(parameters) {
    // function body
    return value;
}
```

Example:
```c
int add(int a, int b) {
    return a + b;
}

int main() {
    int result = add(5, 3);
    printf("5 + 3 = %d\n", result);
    return 0;
}
```

---
layout: center
class: text-center
---

# Thank You!

C remains one of the most influential programming languages, powering operating systems, embedded systems, and more.

[Learn More about C](https://en.cppreference.com/w/c)