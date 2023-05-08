# [2. Bash Scripting Fundamentals](#2-bash-scripting-fundamentals)

## [2.1 Variables and Data Types](#21-variables-and-data-types)

### [2.1.1 Variable Declaration](#211-variable-declaration)

In Bash, you can declare and initialize variables as follows:

```bash
variable_name="value"
```

Here,
`variable_name` is the name of the variable, and
`"value"` is the value you want to assign to it.

Bash _doesn't require_ explicit data type declarations; it determines the data type based on the value you assign.

#### Naming conventions for variable names:

- Variable names should consist of letters, numbers, and underscores.
- They cannot start with a number.
- Variable names are case-sensitive, so `myVar` and `myvar` are treated as different variables.
- Variables declared outside of functions are global and inside a function are local.

### [2.1.2 String Variables](#212-string-variables)

#### 1. Concatenation

Concatenates `str1` and `str2` with a space in between.

```bash
str1="Hello"
str2="World"
result="$str1 $str2"
```

#### 2. Length

To find the length of a string, use the `${#variable_name}` syntax.

```bash
str="Bash"
length=${#str}
```

Stores the length of the string `"Bash"` in the variable `"length"`.

#### 3. Extraction

To extract a substring, you can use `${variable_name:start: length}` syntax.

```bash
str="Hello, World"
substring="${str:7:5}"
```

Extracts `"World"` from the string.

## [2.1.3 Numeric Variables](#213-numeric-variables)

Performing basic arithmetic operations in Bash:

##### Addition, Subtraction, multiplication, and division:

```bash
num1=5
num2=3

sum=$((num1 + num2))
sub=$((num1 - num2))
mul=$((num1 * num2))
div=$((num1 / num2))
```

## [2.2 Input and Output](#22-input-and-output)

### [2.2.1 Command-Line Arguments](#221-command-line-arguments)

- `$0` - The name of the Bash script.
- `$1` - `$9` - The first 9 arguments to the Bash script. (As mentioned above.)
- `$#` - How many arguments were passed to the Bash script.
- `$@` - All the arguments supplied to the Bash script.
- `$?` - The exit status of the most recently run process.
- `$$` - The process ID of the current script.
- `$USER` - The username of the user running the script.
- `$HOSTNAME` - The hostname of the machine the script is running on.
- `$SECONDS` - The number of seconds since the script was started.
- `$RANDOM` - Returns a different random number each time is it referred to.
- `$LINENO` - Returns the current line number in the Bash script.
