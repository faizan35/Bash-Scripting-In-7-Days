# [3. Operators](#3-operators)

## [3.1 Arithmetic Operators](#31-arithmetic-operators)

```bash
num1=5
num2=3
```

| Operator | Description    | Example                 |
| -------- | -------------- | ----------------------- |
| `+`      | Addition       | `sum=$((num1 + num2))`  |
| `-`      | Subtraction    | `sub=$((num1 - num2))`  |
| `*`      | Multiplication | `mul=$((num1 * num2))`  |
| `/`      | Division       | `div=$((num1 / num2))`  |
| `%`      | Modulus        | `mod=$((num1 % num2))`  |
| `**`     | Exponentiation | `exp=$((num1 ** num2))` |

## [3.2 Comparison Operators](#32-comparison-operators)

| Operator | Description                   | Example               |
| -------- | ----------------------------- | --------------------- |
| `==`     | Equal                         | `$result = $a == $b`  |
| `!=`     | Not Equal                     | `$result = $a != $b`  |
| `<`      | Less Than                     | `$result = $a < $b`   |
| `>`      | Greater Than                  | `$result = $a > $b`   |
| `-eq`    | Numeric Equal                 | `$result = $a -eq $b` |
| `-ne`    | Numeric Not Equal             | `$result = $a -ne $b` |
| `-lt`    | Numeric Less Than             | `$result = $a -lt $b` |
| `-le`    | Numeric Less Than or Equal    | `$result = $a -le $b` |
| `-gt`    | Numeric Greater Than          | `$result = $a -gt $b` |
| `-ge`    | Numeric Greater Than or Equal | `$result = $a -ge $b` |
| `-z`     | Zero Length String            | `$result = -z $str`   |
| `-n`     | Non-Zero Length String        | `$result = -n $str`   |

## [3.3 Logical Operators](#33-logical-operators)

| Operator | Description | Example                           |
| -------- | ----------- | --------------------------------- |
| `&&`     | Logical AND | `if ($a -eq 1 -and $b -eq 2) { }` |
| `\|\|`   | Logical OR  | `if ($a -eq 1 -or $b -eq 2) { }`  |
| `!`      | Logical NOT | `if (-not $condition) { }`        |

## [3.4 Assignment Operators](#34-assignment-operators)

| Operator | Description         | Example   |
| -------- | ------------------- | --------- |
| `=`      | Assignment          | `$a = 10` |
| `+=`     | Add and Assign      | `$a += 5` |
| `-=`     | Subtract and Assign | `$a -= 3` |
| `*=`     | Multiply and Assign | `$a *= 2` |
| `/=`     | Divide and Assign   | `$a /= 4` |

## [3.5 Bitwise Operators](#35-bitwise-operators)

| Operator | Description | Example                 |
| -------- | ----------- | ----------------------- |
| `&`      | Bitwise AND | `$result = $a -band $b` |
| `\|`     | Bitwise OR  | `$result = $a -bor $b`  |
| `^`      | Bitwise XOR | `$result = $a -bxor $b` |
| `~`      | Bitwise NOT | `$result = -bnot $a`    |
| `<<`     | Left Shift  | `$result = $a -shl $b`  |
| `>>`     | Right Shift | `$result = $a -shr $b`  |

## [3.6 String Concatenation](#36-string-concatenation)

| Operator | Description   | Example                   |
| -------- | ------------- | ------------------------- |
| `.`      | Concatenation | `$result = $str1 + $str2` |

## [3.7 Array Operators](#37-array-operators)

| Operator | Description      | Example                                 |
| -------- | ---------------- | --------------------------------------- |
| `+=`     | Array Append     | `$array += $value`                      |
| `=`      | Array Assignment | `$array = @($value1, $value2, $value3)` |

## [3.8 Other Operators](#38-other-operators)

| Operator | Description        | Example                                                   |
| -------- | ------------------ | --------------------------------------------------------- |
| `::`     | Indirect Reference | `$variable = "PropertyName"; $value = $object::$variable` |
| `? :`    | Ternary Operator   | `$result = ($condition) ? $valueIfTrue : $valueIfFalse`   |
| `,`      | Comma Operator     | `$result = command1, command2, command3`                  |

[← Previous Day]() || [Index](../README.md) || [Next Day →]()
