# ft_printf - 42 Project
### Introduction
ft_printf is a project at 42 that involves recreating the well-known printf function from the C standard library. This function is widely used for formatted output in C programs, and the goal of this project is to deepen the understanding of variadic functions, formatting, and low-level I/O operations.

The task requires implementing a custom version of printf, called ft_printf, that handles various format specifiers and behaves similarly to the original function.

### Features
The custom ft_printf function must support:

Format Specifiers:

* %c - Character
* %s - String
* %p - Pointer (memory address)
* %d / %i - Integer (decimal)
* %u - Unsigned integer
* %x / %X - Hexadecimal (lowercase/uppercase)
* %% - Literal percent sign

### Usage
To compile and use the ft_printf function, follow these steps:

Clone the repository and navigate to the project folder.

```bash
git clone https://github.com/fclaus-g/ft_printf.git
cd ft_printf
```
Compile the library by running:

```bash
make
```
Include the ft_printf header in your project:

```c
#include "ft_printf.h"
```
Link the compiled library when compiling your project:

```bash
gcc -Wall -Wextra -Werror -L. -lftprintf your_file.c -o your_program
```
Use ft_printf like the standard printf:

```c
ft_printf("Hello, %s!\n", "world");
```
### Project Structure
* **src/:** Contains the source files implementing the core logic of ft_printf.
* **includes/:** Contains the ft_printf.h header file.
* **Makefile:** Automates the compilation process and generates the libftprintf.a static library.
Example
```c
#include "ft_printf.h"

int main(void)
{
    ft_printf("Character: %c\n", 'A');
    ft_printf("String: %s\n", "Hello, 42!");
    ft_printf("Pointer: %p\n", &main);
    ft_printf("Integer: %d\n", 42);
    ft_printf("Unsigned: %u\n", 12345);
    ft_printf("Hexadecimal: %x\n", 255);
    ft_printf("Percentage: %%\n");

    return 0;
}
```
### License
This project is part of the 42 curriculum and is meant for educational purposes. Feel free to use it for learning, but be mindful of 42's collaboration policies.
