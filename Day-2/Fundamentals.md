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

### [2.1.2 String Variables]()
