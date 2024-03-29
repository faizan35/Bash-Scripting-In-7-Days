# 5. Bash Scripting Fundamentals 2

## 5.1 Strings

Bash String is a data type such as as an integer or floating-point unit. It is used to represent text rather than numbers. It is a combination of a set of characters that may also contain numbers.

**For example** the word "bashScripting" and the phrase "Welcome to Bash" are the strings. Even "65756" could be considered as a string, if specified correctly.

### 5.1.1 Length of a string

To calculate the length of a string, we can use any of the following syntax:

```bash
1.  ${#string}
2.  expr length "$string"
3.  expr "$string" :'.*'
4.  $str | wc -c
5.  $str |awk '{print length}'
```

**Example**

```bash
#!/bin/bash

string="Bash is very easy"
len=${#string}

echo "Length of '$string' is $len"
```

### 5.1.2 Split a String

--------/////////------------------------
Array

Regular Expressions and Pattern Matching

Real-World Bash Scripting
