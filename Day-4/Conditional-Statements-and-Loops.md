# 4. Conditionals and Loops

## 4.1 if-elif-else

### if Statements

```bash
if [ expression ];
then
statements
fi
```

**Example:**

```bash
if [ 200 -gt 177 ]  # 200 > 177
then
echo "Greater than 177"
fi
```

### If Else Statements

```bash
if [ condition ];
then
   <if block commands>
else
  <else block commands>
fi
```

**Example:**

```bash
if [ 100 -gt 30 ];
then
  echo "100 is greater than 30."
else
  echo "100 is not greater than 30."
fi
```

### Else If (elif)

```bash
if [ condition ];
then
<commands>
elif [ condition ];
then
<commands>
else
<commands>
fi
```

## 4.2 Switch Case (case statements)

```bash
case expression in
    pattern_1)
        statements
        ;;
    pattern_2)
        statements
        ;;
    pattern_3|pattern_4|pattern_5)
        statements
        ;;
    pattern-n)
        statements
        ;;
    *)
        statements
        ;;
esac
```

**Example:**

```bash
#!/bin/bash

echo "Do you know Bash?"
read -p "Yes / No? => " Ans
case $Ans in
    Yes|yes|y|Y)
        echo "Awesome."
        echo
        ;;
    No|no|N|n)
        echo "Start learning."
        ;;
esac
```

## 4.3 Loops

### 4.3.1 For loops

A `for` loop in Bash is used to iterate over a list of items, such as an array or a sequence of numbers, and perform a set of commands for each item in the list.

```bash
for item in list
do
  # Commands to be executed for each item
done
```

- Loop through an array of strings:
  ```bash
  fruits=("apple" "banana" "cherry" "date")
  for fruit in "${fruits[@]}"
  do
  echo "I like $fruit"
  done
  ```
- Loop through a sequence of numbers:
  ```bash
  for number in {1..5}
  do
  echo "Number: $number"
  done
  ```
- Traditional for loop:
  ```bash
  for ((initialization; condition; increment))
  do
  # Commands to be executed for each iteration
  done
  ```
  Example of for loop that counts from 1 to 5:
  ```bash
  for ((i=1; i<=5; i++))
  do
  echo "Iteration $i"
  done
  ```

### 4.3.2 While Loop

A while loop in Bash is used to repeatedly execute a set of commands as long as a specified condition is true.

```bash
while [condition]
do
  # Commands to be executed as long as the condition is true
done
```

Here's a breakdown of how to use a while loop in Bash:

- `while`: The keyword that starts the loop.

- `[condition]`: The condition that is checked before each iteration of the loop. If true, loop's continue or if false, the loop terminates.

- `do`: Marks the beginning of the block of commands to be executed while the condition is true.

- `done`: Marks the end of the loop.

Here's an example of a while loop in Bash:

```bash
count=1
while [ $count -le 5 ]
do
  echo "Count: $count"
  count=$((count + 1))
done
```

### 4.3.2 Until Loop

It is **opposite** to `while` loop.

| While Loop                                                          | Until Loop                                                           |
| ------------------------------------------------------------------- | -------------------------------------------------------------------- |
| `while` loops continue to execute as long as the condition is true. | `until` loops continue to execute as long as the condition is false. |
| Loop stops when the condition becomes false.                        | Loop stops when the condition becomes true.                          |

```bash
until [ condition ]; do
    # Code to execute while the condition is false
done
```

**Example**

```bash
# Using an until loop to print numbers from 1 to 5
n=1
until [ $n -gt 5 ]; do
    echo $n
    n=$((n+1))
done
```

[← Previous Day]() || [Index](../README.md) || [Next Day →]()
