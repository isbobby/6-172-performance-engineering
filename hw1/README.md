# Homework 1 Notes
## Preprocessing with clang -E <br>
## Macros in C <br>
A macro is defined with the pre-processor directive, which means all macros will be pre-processed before the program compiles. Unlike macros, a normal function will not be pre-processed. <br>

|Macro      | Functions | 
| ----------- | ----------- |
|Pre-processed|Compiled|
|No type checking 🧐| Type checking 😀|
|Does not check for compile time errors|Checks for error during compile time|
|Speed of execution is faster 😇|Slower execution due to function call overheads🥲|

Macros used in `sizes.c` are <br>
```
// Object-like macro
#define DEBUG 1

// Function-like macro
#define PRINT_SIZE(string, type) if (DEBUG) \
        printf("size of %s : %zu bytes \n", string, sizeof(type))

// Calling the Macro
PRINT_SIZE("short", short);
```
## Data Types in C <br>
To see the sizes of each data type, run `make sizes && ./sizes`

