# ft_printf

## Overview
`ft_printf` is a custom implementation of the standard C `printf` function, developed as part of the 42 school curriculum. This project aims to replicate the behavior of `printf` while deepening the understanding of variadic functions, formatted output, and low-level manipulation in C.

## Features
- Supports the following format specifiers:
  - `%c` : Character
  - `%s` : String
  - `%p` : Pointer address
  - `%d` : Decimal integer
  - `%i` : Integer
  - `%u` : Unsigned integer
  - `%x` : Lowercase hexadecimal
  - `%X` : Uppercase hexadecimal
  - `%%` : Percent sign
- Handles variable-length arguments using `va_list`.
- Efficiently prints formatted output to the standard output.

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/mertcangur/ft_printf.git
   cd ft_printf
   ```
2. Compile the library:
   ```sh
   make
   ```
3. Include `ft_printf` in your project:
   - Compile with:
     ```sh
     gcc your_file.c libftprintf.a -o your_program
     ```
   - Include the header in your source code:
     ```c
     #include "ft_printf.h"
     ```

## Usage
Example usage of `ft_printf`:
```c
#include "ft_printf.h"

int main() {
    ft_printf("Hello, %s!\n", "world");
    ft_printf("Decimal: %d, Hex: %x\n", 42, 42);
    ft_printf("Pointer address: %p\n", (void*)&main);
    return 0;
}
```

## Project Structure
- `ft_printf.c` - Main implementation of `ft_printf`
- `ft_printf.h` - Header file containing function prototypes
- `Makefile` - Compilation rules
- `libft/` - Custom `libft` functions used in `ft_printf`
