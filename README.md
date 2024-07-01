![42 beirut](https://media.licdn.com/dms/image/D4E3DAQGxvimpQQFi_A/image-scale_191_1128/0/1695893480399/42_beirut_cover?e=2147483647&v=beta&t=oNrMR2IXjtfu3XXV-uSUW8wI98g19yUUHZ0XuhtX2NE)
---

# Custom `printf` Function

This project implements a custom `printf` function in C. The goal is to create a versatile and efficient version of the standard `printf` function, which allows formatted output to the console.

## Features

- Supports various format specifiers such as `%d`, `%s`, `%c`,`%u`,`%X`,`%x` and `%p`.
- Handles variable arguments.
- Provides similar functionality to the standard `printf` function.

## Getting Started

### Prerequisites

- C compiler (e.g., `gcc` or `cc`).
- `make` utility.

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/ahmadmnsur/42_printf.git
    cd 42_printf
    ```

2. Compile the code using `make`:
    ```sh
    make
    ```

3. The `libftprintf.a` library will be generated.

## Usage

Include the header file `ft_printf.h` in your C program and link against the `libftprintf.a` library:

```c
#include "ft_printf.h"

int main() {
    ft_printf("Hello, World!\n");
    ft_printf("Number: %d\n", 42);
    ft_printf("String: %s\n", "example");
    return 0;
}
```

Compile your program with the custom `ft_printf` library:
```sh
cc -o my_program my_program.c libftprintf.a
```

## Project Structure

- `printf.h`: Header file containing the function declaration.
- `ft_hex.c`: Source file handling hexadecimal format.
- `ft_pointer.c`: Source file handling pointer format.
- `ft_printf.c`: Source file containing the main implementation of the custom `ft_printf` function.
- `ft_putchr.c`: Source file for character output.
- `ft_putnbr.c`: Source file for number output.
- `ft_putstr.c`: Source file for string output.
- `ft_unbr.c`: Source file for unsigned number output.
- `Makefile`: Makefile for building the project.

## Makefile Targets

- `all`: Default target. Compiles the library.
- `clean`: Removes object files.
- `fclean`: Removes object files and the library.
- `re`: Rebuilds the project by running `fclean` and then `all`.

---

